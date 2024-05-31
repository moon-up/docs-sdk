# Whisper

### Summary

This documentation provides a guide on how to use the `useWhisper` function to integrate with the OpenAPI specification provided by Moon API. The `useWhisper` function facilitates audio recording and transcription using OpenAI's Whisper model, which can then be processed through the LangChain API.

### Installation

To get started, ensure you have the necessary dependencies installed. You can add them to your project using npm, yarn, or pnpm:

### Installation

{% tabs %}
{% tab title="npm" %}
```bash
npm install -S langchain @langchain/openai @chengsokdara/use-whisper
```
{% endtab %}

{% tab title="yarn" %}
```bash
yarn add langchain @langchain/openai @chengsokdara/use-whisper
```
{% endtab %}

{% tab title="pnpm" %}
```bash
pnpm add langchain @langchain/openai @chengsokdara/use-whisper
```
{% endtab %}
{% endtabs %}

### Usage

```typescript
import { ChatOpenAI } from '@langchain/openai';
import { createOpenAPIChain } from 'langchain/chains';
import { useWhisper } from '@chengsokdara/use-whisper'
import { useEffect, useState } from 'react';

function Whisper() {
  const [chain, setChain] = useState<any>(null);
  const [results, setResults] = useState<any[]>([]);
  const {
    recording,
    speaking,
    transcribing,
    transcript,
    pauseRecording,
    startRecording,
    stopRecording,
  } = useWhisper({
    apiKey: process.env.REACT_APP_OPENAI_API_KEY
  });
  useEffect(() => {
    const initializeChat = async () => {
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
      setChain(chain);
    };
    initializeChat();
  }, []);
  const sendMessage = async () => {
    if (chain) {
      const result = await chain.run(transcript.text);
      console.log(JSON.stringify(result, null, 2));
      setResults((prevResults) => [...prevResults, result]);
    }
  };
  return (
    <div>
      <p>Recording: {recording}</p>
      <p>Speaking: {speaking}</p>
      <p>Transcribing: {transcribing}</p>
      <p>Transcribed Text: {transcript.text}</p>
      <button onClick={() => startRecording()}>Start</button>
      <button onClick={() => pauseRecording()}>Pause</button>
      <button onClick={() => stopRecording()}>Stop</button>
      <button onClick={sendMessage}>Send</button>
      {results.map((result, index) => (
        <p key={index}>{JSON.stringify(result)}</p>
      ))}
    </div>
  );
}

export default Whisper;
 
```

This code snippet demonstrates how to:

1. Initialize a chat model using OpenAI's GPT-4.
2. Create an OpenAPI chain using the LangChain API.
3. Use the `useWhisper` hook to handle audio recording and transcription.
4. Send the transcribed text to the Moon API and display the results.

By following this example, you can leverage OpenAI's Whisper for audio input and integrate it seamlessly with various API endpoints using LangChain.

