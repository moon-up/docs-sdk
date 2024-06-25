# Hooks

## Moon SDK Hooks Documentation

The `@moonup/moon-react-native` package provides a set of hooks that allow you to easily interact with the Moon SDK in your React Native project. This documentation page will guide you through the basics of using these hooks.

### Table of Contents

* Installation
* Usage
* Hooks
* Examples

### Installation

To use the Moon SDK hooks in your project, you'll need to install the `@moonup/moon-react-native` package. You can install it using npm:

```bash
npm install @moonup/moon-react-native
```

### Usage

To use the Moon SDK hooks, you'll need to wrap your application with the `MoonContextProvider`. Here's an example of how to do this:

```javascript
import React from 'react';
import { MoonContextProvider } from '@moonup/moon-react-native';
import App from './App';

export default function Main() {
  return (
    <MoonContextProvider>
      <App />
    </MoonContextProvider>
  );
}
```

### Hooks

The `@moonup/moon-react-native` package provides the following hooks:

* `useMoonConnect`: A hook that returns the `connect` function from the Moon SDK context.
* `useMoonDisconnect`: A hook that returns the `disconnect` function from the Moon SDK context.
* `useUserSession`: A hook that returns the `getUserSession` function from the Moon SDK context.
* `useSolanaSDK`: A hook that returns the Solana SDK instance from the Moon SDK context.
* `useBitcoinSDK`: A hook that returns the Bitcoin SDK instance from the Moon SDK context.
* `useCosmosSDK`: A hook that returns the Cosmos SDK instance from the Moon SDK context.
* `useEosSDK`: A hook that returns the EOS SDK instance from the Moon SDK context.
* `useLitecoinSDK`: A hook that returns the Litecoin SDK instance from the Moon SDK context.
* `useRippleSDK`: A hook that returns the Ripple SDK instance from the Moon SDK context.
* `useTronSDK`: A hook that returns the Tron SDK instance from the Moon SDK context.
* `useBitcoincashSDK`: A hook that returns the Bitcoin Cash SDK instance from the Moon SDK context.
* `useDogecoinSDK`: A hook that returns the Dogecoin SDK instance from the Moon SDK context.
* `useAccountsSDK`: A hook that returns the Accounts SDK instance from the Moon SDK context.
* `useAaveSDK`: A hook that returns the Aave SDK instance from the Moon SDK context.
* `useConveyorfinanceSDK`: A hook that returns the Conveyor Finance SDK instance from the Moon SDK context.
* `useENSSDK`: A hook that returns the ENS SDK instance from the Moon SDK context.
* `useErc20SDK`: A hook that returns the ERC-20 SDK instance from the Moon SDK context.
* `useErc1155SDK`: A hook that returns the ERC-1155 SDK instance from the Moon SDK context.
* `useErc721SDK`: A hook that returns the ERC-721 SDK instance from the Moon SDK context.
* `useOneinchSDK`: A hook that returns the 1inch SDK instance from the Moon SDK context.
* `useUniswapSDK`: A hook that returns the Uniswap SDK instance from the Moon SDK context.
* `useYearnSDK`: A hook that returns the Yearn SDK instance from the Moon SDK context.

### Examples

Here are examples of how to use each of the Moon SDK hooks:

#### `useMoonConnect`

```javascript
import React from 'react';
import { Button } from 'react-native';
import { useMoonConnect } from '@moonup/moon-react-native';

export default function ConnectButton() {
  const connect = useMoonConnect();

  const handleConnect = async () => {
    try {
      await connect();
    } catch (error) {
      console.error(error);
    }
  };

  return (
    <Button title="Connect" onPress={handleConnect} />
  );
}
```

#### `useMoonDisconnect`

```javascript
import React from 'react';
import { Button } from 'react-native';
import { useMoonDisconnect } from '@moonup/moon-react-native';

export default function DisconnectButton() {
  const disconnect = useMoonDisconnect();

  const handleDisconnect = async () => {
    try {
      await disconnect();
    } catch (error) {
      console.error(error);
    }
  };

  return (
    <Button title="Disconnect" onPress={handleDisconnect} />
  );
}
```

#### `useUserSession`

```javascript
import React from 'react';
import { Button, Text } from 'react-native';
import { useUserSession } from '@moonup/moon-react-native';

export default function UserSession() {
  const getUserSession = useUserSession();
  const [session, setSession] = React.useState(null);

  const handleGetUserSession = async () => {
    try {
      const { data } = await getUserSession();
      setSession(data.session);
    } catch (error) {
      console.error(error);
    }
  };

  return (
    <>
      <Button title="Get User Session" onPress={handleGetUserSession} />
      {session && <Text>User Session: {JSON.stringify(session)}</Text>}
    </>
  );
}
```

#### `useSolanaSDK`

```javascript
import React from 'react';
import { Button, Text } from 'react-native';
import { useSolanaSDK } from '@moonup/moon-react-native';

export default function SolanaBalance() {
  const solanaSDK = useSolanaSDK();
  const [balance, setBalance] = React.useState(null);

  const handleGetBalance = async () => {
    try {
      const response = await solanaSDK.getBalance('your-solana-address');
      setBalance(response.data.balance);
    } catch (error) {
      console.error(error);
    }
  };

  return (
    <>
      <Button title="Get Balance" onPress={handleGetBalance} />
      {balance && <Text>Balance: {balance}</Text>}
    </>
  );
}
```

The other hooks can be used in a similar way, by replacing `useSolanaSDK` with the appropriate hook name and calling the appropriate SDK method.
