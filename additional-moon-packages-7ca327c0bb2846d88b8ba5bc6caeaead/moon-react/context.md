# Context

## MoonSDKProvider Documentation

The `MoonSDKProvider` is a React context provider that provides access to the Moon SDK and other related functionality to its child components. This documentation page will guide you through the basics of using the `MoonSDKProvider` in your React project.

### Table of Contents

* Installation
* Usage
* Context Values
* Example

### Installation

To use the `MoonSDKProvider` in your project, you'll need to install the `@moonup/moon-react` package. You can install it using npm:

```bash
npm install @moonup/moon-react
```

### Usage

To use the `MoonSDKProvider`, you'll need to wrap your application with it. Here's an example of how to do this:

```javascript
import React from 'react';
import { MoonSDKProvider } from '@moonup/moon-react';
import App from './App';

export default function Main() {
  return (
    <MoonSDKProvider>
      <App />
    </MoonSDKProvider>
  );
}
```

### `MoonSDKProvider` context:

#### `connect(accessToken?: string, refreshToken?: string)`

Connects to the Moon API using the provided access and refresh tokens.

Example:

```javascript
import React from 'react';
import { Button } from 'react-native';
import { useMoonSDK } from '@moonup/moon-react';

export default function Connect() {
  const { connect } = useMoonSDK();

  const handleConnect = async () => {
    try {
      await connect('access-token', 'refresh-token');
    } catch (error) {
      console.error(error);
    }
  };

  return (
    <Button title="Connect" onPress={handleConnect} />
  );
}
```

#### `disconnect()`

Disconnects from the Moon API.

Example:

```javascript
import React from 'react';
import { Button } from 'react-native';
import { useMoonSDK } from '@moonup/moon-react';

export default function Disconnect() {
  const { disconnect } = useMoonSDK();

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

#### `getUserSession()`

Retrieves the current user session.

Example:

```javascript
import React from 'react';
import { Button, Text } from 'react-native';
import { useMoonSDK } from '@moonup/moon-react';

export default function UserSession() {
  const { session, getUserSession } = useMoonSDK();

  const handleGetUserSession = async () => {
    try {
      await getUserSession();
    } catch (error) {
      console.error(error);
    }
  };

  return (
    <>
      <Button title="Get User Session" onPress={handleGetUserSession} />
      <Text>{JSON.stringify(session)}</Text>
    </>
  );
}
```

#### `connectEthers()`

Connects to the Moon Ethers provider.

Example:

```javascript
import React from 'react';
import { Button } from 'react-native';
import { useMoonSDK } from '@moonup/moon-react';

export default function ConnectEthers() {
  const { connectEthers } = useMoonSDK();

  const handleConnectEthers = async () => {
    try {
      await connectEthers();
    } catch (error) {
      console.error(error);
    }
  };

  return (
    <Button title="Connect Ethers" onPress={handleConnectEthers} />
  );
}
```

#### `disconnectEthers()`

Disconnects from the Moon Ethers provider.

Example:

```javascript
import React from 'react';
import { Button } from 'react-native';
import { useMoonSDK } from '@moonup/moon-react';

export default function DisconnectEthers() {
  const { disconnectEthers } = useMoonSDK();

  const handleDisconnectEthers = async () => {
    try {
      await disconnectEthers();
    } catch (error) {
      console.error(error);
    }
  };

  return (
    <Button title="Disconnect Ethers" onPress={handleDisconnectEthers} />
  );
}
```

#### `request(args: any)`

Sends a request to the Moon Ethers provider.

Example:

```javascript
import React from 'react';
import { Button, Text } from 'react-native';
import { useMoonSDK } from '@moonup/moon-react';

export default function Request() {
  const { request } = useMoonSDK();
  const [result, setResult] = React.useState(null);

  const handleRequest = async () => {
    try {
      const response = await request({ method: 'eth_accounts' });
      setResult(response);
    } catch (error) {
      console.error(error);
    }
  };

  return (
    <>
      <Button title="Request" onPress={handleRequest} />
      <Text>{JSON.stringify(result)}</Text>
    </>
  );
}
```

#### `signOut()`

Signs out the current user.

Example:

```javascript
import React from 'react';
import { Button } from 'react-native';
import { useMoonSDK } from '@moonup/moon-react';

export default function SignOut() {
  const { signOut } = useMoonSDK();

  const handleSignOut = async () => {
    try {
      await signOut();
    } catch (error) {
      console.error(error);
    }
  };

  return (
    <Button title="Sign Out" onPress={handleSignOut} />
  );
}
```

#### `createWallet()`

Creates a new Ethereum wallet and adds it to the Moon SDK.

Example:

```javascript
import React from 'react';
import { Button, Text } from 'react-native';
import { useMoonSDK } from '@moonup/moon-react';

export default function CreateWallet() {
  const { wallets, createWallet } = useMoonSDK();

  const handleCreateWallet = async () => {
    try {
      await createWallet();
    } catch (error) {
      console.error(error);
    }
  };

  return (
    <>
      <Button title="Create Wallet" onPress={handleCreateWallet} />
      {wallets.map((wallet) => (
        <Text key={wallet}>{wallet}</Text>
      ))}
    </>
  );
}
```

#### `listWallets()`

Retrieves the list of Ethereum wallets managed by the Moon SDK.

Example:

```javascript
import React from 'react';
import { Button, Text } from 'react-native';
import { useMoonSDK } from '@moonup/moon-react';

export default function WalletList() {
  const { wallets, listWallets } = useMoonSDK();

  const handleListWallets = async () => {
    try {
      await listWallets();
    } catch (error) {
      console.error(error);
    }
  };

  return (
    <>
      <Button title="List Wallets" onPress={handleListWallets} />
      {wallets.map((wallet) => (
        <Text key={wallet}>{wallet}</Text>
      ))}
    </>
  );
}
```

#### `setWallet(wallet: string)`

Sets the currently selected Ethereum wallet address.

Example:

```javascript
import React from 'react';
import { Button, Text } from 'react-native';
import { useMoonSDK } from '@moonup/moon-react';

export default function SetWallet() {
  const { wallet, setWallet } = useMoonSDK();

  const handleSetWallet = async () => {
    try {
      await setWallet('0x1234567890abcdef');
    } catch (error) {
      console.error(error);
    }
  };

  return (
    <>
      <Button title="Set Wallet" onPress={handleSetWallet} />
      <Text>{wallet}</Text>
    </>
  );
}
```

#### `getChains()`

Retrieves the list of supported blockchain networks.

Example:

```javascript
import React from 'react';
import { Button, Text } from 'react-native';
import { useMoonSDK } from '@moonup/moon-react';

export default function ChainList() {
  const { chains, getChains } = useMoonSDK();

  const handleGetChains = async () => {
    try {
      await getChains();
    } catch (error) {
      console.error(error);
    }
  };

  return (
    <>
      <Button title="Get Chains" onPress={handleGetChains} />
      {chains.map((chain) => (
        <Text key={chain.chain_id}>{chain.name}</Text>
      ))}
    </>
  );
}
```

### Example

Here's an example of how to use the `MoonSDKProvider` to retrieve the list of Ethereum wallets managed by the Moon SDK:

```javascript
import React from 'react';
import { Button, Text } from 'react-native';
import { useMoonSDK } from '@moonup/moon-react';

export default function WalletList() {
  const { wallets, listWallets } = useMoonSDK();

  const handleListWallets = async () => {
    try {
      await listWallets();
    } catch (error) {
      console.error(error);
    }
  };

  return (
    <>
      <Button title="List Wallets" onPress={handleListWallets} />
      {wallets.map((wallet) => (
        <Text key={wallet}>{wallet}</Text>
      ))}
    </>
  );
}
```

In this example, we import the `useMoonSDK` hook from the `@moonup/moon-react` package and use it to access the `wallets` and `listWallets` context values. We then use these values to retrieve the list of Ethereum wallets managed by the Moon SDK and display them in a list
