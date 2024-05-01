# Langchain

```typescript
import { ChatOpenAI } from 'langchain/chat_models/openai';
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
