# @moonup/moon-rainbowkit

## @moonup/moon-rainbowkit Package Documentation**:**

The `@moonup/moon-rainbowkit` package is a React component that provides authentication functionality using the Moon SDK and RainbowKit. This package allows users to sign in with Ethereum to the app using SIWE (Sign-In with Ethereum) and manages the authentication state.

\


## **Installing Moon Rainbowkit:**

To utilize the Moon rainbowkit package, first install it to the desired directory of the project:

#### To install Moon rainbowkit

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

Import the `RainbowMoonProvider` component from the package and wrap your application with it.



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
