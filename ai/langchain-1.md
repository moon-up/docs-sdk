# Whisper

### Summary

The `langchain` library is a powerful tool for building applications that leverage language models to perform tasks such as text generation, summarization, and question answering. One of the ways to enhance the capabilities of a language model is to integrate it with external APIs that provide additional data or functionality. The `createOpenAPIChain` function in `langchain` allows you to easily integrate with an API that is described by an OpenAPI specification.

In this documentation page, we will show you how to use the `useWhisper` function from the `@chengsokdara/use-whisper` package to integrate with the OpenAPI specification provided by Moon API. Moon API is a comprehensive library that provides a set of APIs for interacting with various blockchain networks and decentralized finance (DeFi) protocols. By integrating with Moon API using Whisper, you can build applications that leverage audio input to perform tasks such as managing blockchain accounts, interacting with DeFi protocols, and more.

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

Here is an example of how to use the `useWhisper` function to integrate with the OpenAPI specification provided by Moon API:

```typescript
import { ChatOpenAI } from '@langchain/openai';
import { createOpenAPIChain } from 'langchain/chains';
import { useWhisper } from '@chengsokdara/use-whisper';
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

In this example, we first import the `ChatOpenAI` class from `@langchain/openai`, the `createOpenAPIChain` function from `langchain/chains`, and the `useWhisper` function from `@chengsokdara/use-whisper`. We then define a functional component `Whisper` that uses the `useWhisper` hook to handle audio recording and transcription.

We initialize a chat model using OpenAI's GPT-4 and create an OpenAPI chain using the Moon API OpenAPI specification in the `useEffect` hook. We then define a `sendMessage` function that sends the transcribed text to the Moon API and displays the results.

The component renders the recording, speaking, and transcribing status, the transcribed text, and buttons to start, pause, and stop recording, as well as a button to send the transcribed text to the Moon API. The results are displayed below the buttons.

By integrating with Moon API using the `useWhisper` function, you can build applications that leverage audio input to perform a wide range of tasks related to blockchain networks and DeFi protocols. Whether you're building a simple wallet application or a complex decentralized finance platform, Moon API and `langchain` have the tools you need to get the job done.

