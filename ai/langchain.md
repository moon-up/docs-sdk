# Langchain

### Summary

Here is an example of how to use the `createOpenAPIChain` function to integrate with the OpenAPI specification provided by Moon API.

### Installation

{% tabs %}
{% tab title="npm" %}
```bash
npm install -S langchain @langchain/openai
```
{% endtab %}

{% tab title="yarn" %}
```bash
yarn add langchain @langchain/openai
```
{% endtab %}

{% tab title="pnpm" %}
```bash
pnpm add langchain @langchain/openai
```
{% endtab %}
{% endtabs %}

### Usage

```typescript
import { ChatOpenAI } from '@langchain/openai';
import { createOpenAPIChain } from 'langchain/chains';

const chatModel = new ChatOpenAI({
  modelName: 'gpt-4-1106-preview',
  temperature: 0,
  openAIApiKey: process.env.OPENAI_API_KEY,
});
const chain = await createOpenAPIChain('https://beta.usemoon.ai/.well-known/swagger.json', {
  llm: chatModel,
  headers: {
    Authorization: `Bearer ${MOON_API_KEY}`,
  },
});
  
const result = await chain.run(message);
console.log(JSON.stringify(result, null, 2));
 
```

This code snippet initializes a chat model using OpenAI's GPT-4, creates an OpenAPI chain, and runs a message through the chain, logging the result.

### Swagger Definitions

We chunk the swagger definition into route-

* [Swagger](https://beta.usemoon.ai/.well-known/swagger.json)
* [Accounts](https://beta.usemoon.ai/.well-known/Accounts.json)
* [Aave](https://beta.usemoon.ai/.well-known/Aave.json)
* [AI Plugin](https://beta.usemoon.ai/.well-known/ai-plugin.json)
* [Bitcoin Cash](https://beta.usemoon.ai/.well-known/bitcoincash.json)
* [Bitcoin](https://beta.usemoon.ai/.well-known/Bitcoin.json)
* [Conveyor Finance](https://beta.usemoon.ai/.well-known/ConveyorFinance.json)
* [Cosmos](https://beta.usemoon.ai/.well-known/Cosmos.json)
* [DogeCoin](https://beta.usemoon.ai/.well-known/DogeCoin.json)
* [ENS](https://beta.usemoon.ai/.well-known/ENS.json)
* [EOS](https://beta.usemoon.ai/.well-known/eos.json)
* [ERC1155](https://beta.usemoon.ai/.well-known/ERC1155.json)
* [ERC20](https://beta.usemoon.ai/.well-known/Erc20.json)
* [ERC4337](https://beta.usemoon.ai/.well-known/Erc4337.json)
* [ERC721](https://beta.usemoon.ai/.well-known/Erc721.json)
* [Litecoin](https://beta.usemoon.ai/.well-known/Litecoin.json)
* [1inch](https://beta.usemoon.ai/.well-known/oneinch.json)
* [Onramper](https://beta.usemoon.ai/.well-known/onramper.json)
* [OpenAPI](https://beta.usemoon.ai/.well-known/openapi.json)
* [Payment](https://beta.usemoon.ai/.well-known/payment.json)
* [Ripple](https://beta.usemoon.ai/.well-known/ripple.json)
* [Solana](https://beta.usemoon.ai/.well-known/Solana.json)
* [Tron](https://beta.usemoon.ai/.well-known/Tron.json)
* [UniSwap](https://beta.usemoon.ai/.well-known/UniSwap.json)
* [Yearn](https://beta.usemoon.ai/.well-known/yearn.json)
