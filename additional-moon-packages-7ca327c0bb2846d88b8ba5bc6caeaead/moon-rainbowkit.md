# Moon Rainbowkit

Rainbow kit library

#### usage



Install the package

```
npm install @moonup/moon-rainbowkit
```

import the provider

```typescript
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
