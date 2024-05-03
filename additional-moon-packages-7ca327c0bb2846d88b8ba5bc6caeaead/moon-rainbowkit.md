# @moonup/moon-rainbowkit

## Moon **Rainbowkit**

## **About Moon Rainbowkit:**

Moon rainbowkit provides a siwe functionality for rainbowkit using moon.

## **Installing Moon Rainbowkit:**

To utilize the Moon Viem package, first install it to the desired directory of the project:

#### To install Moon Viem

{% tabs %}
{% tab title="npm" %}
```bash
npm install @moonup/moon-rainbowkit
```
{% endtab %}

{% tab title="yarn" %}
```bash
yarn add @moonup/moon-rainbowkit
```
{% endtab %}

{% tab title="pnpm" %}
```bash
pnpm add @moonup/moon-rainbowkit
```
{% endtab %}
{% endtabs %}

### Usage

import the provider

```tsx
import {RainbowKitUseMoonProvider} from '@moonup/moon-rainbowkit';
import {
  RainbowKitProvider,
} from '@rainbow-me/rainbowkit';
import { AppProps } from 'next/app';
import { WagmiConfig } from 'wagmi';

export default function App({ Component, pageProps }: AppProps) {
  // You'll need to resolve AUTHENTICATION_STATUS here
  // using your application's authentication system.
  // It needs to be either 'loading' (during initial load),
  // 'unauthenticated' or 'authenticated'.

  return (
    <WagmiConfig {...etc}>
      <RainbowKitUseMoonProvider
       onSignIn={onSignIn} onSignOut={onSignOut}
      >
        <RainbowKitProvider {...etc}>
          <Component {...pageProps} />
        </RainbowKitProvider>
      </RainbowKitAuthenticationProvider>
    </WagmiConfig>
  );
}
```

## Example Project

[https://github.com/moon-up/moon-sdk/tree/main/examples/moon-sdk-rainbowkit-next-example](https://github.com/moon-up/moon-sdk/tree/main/examples/moon-sdk-rainbowkit-next-example)
