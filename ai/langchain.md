# Langchain

## Langchain Documentation: Integrating with Moon API

The `langchain` library is a powerful tool for building applications that leverage language models to perform tasks such as text generation, summarization, and question answering. One of the ways to enhance the capabilities of a language model is to integrate it with external APIs that provide additional data or functionality. The `createOpenAPIChain` function in `langchain` allows you to easily integrate with an API that is described by an OpenAPI specification.

In this documentation page, we will show you how to use the `createOpenAPIChain` function to integrate with the OpenAPI specification provided by Moon API. Moon API is a comprehensive library that provides a set of APIs for interacting with various blockchain networks and decentralized finance (DeFi) protocols. By integrating with Moon API, you can build applications that leverage language models to perform tasks such as managing blockchain accounts, interacting with DeFi protocols, and more.

### Installation

To use the `createOpenAPIChain` function, you will need to install the `langchain` and `@langchain/openai` packages. You can install these packages using npm, Yarn, or pnpm:

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

Here is an example of how to use the `createOpenAPIChain` function to integrate with the OpenAPI specification provided by Moon API:

```javascript
import { ChatOpenAI } from '@langchain/openai';
import { createOpenAPIChain } from 'langchain/chains';

// Initialize the chat model using OpenAI's GPT-4
const chatModel = new ChatOpenAI({
  modelName: 'gpt-4-1106-preview',
  temperature: 0,
  openAIApiKey: process.env.OPENAI_API_KEY,
});

// Create an OpenAPI chain using the Moon API OpenAPI specification
const chain = await createOpenAPIChain('https://beta.usemoon.ai/.well-known/swagger.json', {
  llm: chatModel,
  headers: {
    Authorization: `Bearer ${MOON_API_KEY}`,
  },
});

// Run a message through the chain and log the result
const message = 'Create a new Ethereum account';
const result = await chain.run(message);
console.log(JSON.stringify(result, null, 2));
```

In this example, we first import the `ChatOpenAI` class from `@langchain/openai` and the `createOpenAPIChain` function from `langchain/chains`. We then initialize a chat model using OpenAI's GPT-4 and create an OpenAPI chain using the Moon API OpenAPI specification. We pass the chat model and an authorization header to the `createOpenAPIChain` function.

We then define a message that we want to run through the chain, which in this case is 'Create a new Ethereum account'. We call the `run` method on the chain with the message as an argument, which sends the message to the chat model and the OpenAPI chain, and returns the result. We log the result to the console.

The `createOpenAPIChain` function automatically generates a prompt that describes the API endpoints and their input and output schemas, and uses the chat model to generate a request that matches the API specification. The function then sends the request to the API and returns the response.

By integrating with Moon API using the `createOpenAPIChain` function, you can build applications that leverage language models to perform a wide range of tasks related to blockchain networks and DeFi protocols. Whether you're building a simple wallet application or a complex decentralized finance platform, Moon API and `langchain` have the tools you need to get the job done.

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
