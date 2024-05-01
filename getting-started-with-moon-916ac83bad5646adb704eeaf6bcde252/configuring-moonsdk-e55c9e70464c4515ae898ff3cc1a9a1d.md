# Configuring MoonSDK

Configuring the Moon SDK involves setting up various modules and authentication parameters to ensure smooth communication with Moon APIs.

When leveraging React, the Moon SDK seamlessly integrates with a project's codebase through two primary interfaces:

1. **Moon SDK React Component:** A React Component that loads the SDK and manages state.
2. **useMoonHook:** a React Hook that returns the SDK's key methods and state variables.

## **MoonSDK React Component**

Import into a React project with the following import statement:

```jsx
import { MoonSDK } from '@moonup/moon-sdk';
```

The Moon SDK houses numerous modules for handling blockchain transactions, accounts, authentication, and specific blockchain protocols like Ethereum, Bitcoin, Solana, etc.

Below is an example MoonSDK initialization function showcasing authentication, storage, and network setup. It utilizes the Sepolia testnet, defined within the Chain array. The moonInstance variable, responsible for setting up the new MoonSDK, references this network configuration alongside authentication and storage parameters.

```tsx

const initialize = async () => {
	const moonInstance = new MoonSDK();

	setMoon(moonInstance);
	moonInstance.login();
};
```

## **useMoonHook**

The Moon SDK class defines methods for performing various tasks related to blockchain operations. These methods encompass functions for logging in, refreshing tokens, listing accounts, signing transactions/messages/typed data, sending transactions, and updating configurations.

The useMoonHook can utilize these functions from the SDK to import into various components of a project.

Below is an example of a useMoonHook that includes functions from the API library such as creating an account, listing accounts, updating tokens, etc.:

```jsx
export const useMoonHook = () => {

  const [moon, setMoon] = useState<MoonSDK | null>(null);

  const initialize = async () => {

    const moonInstance = new MoonSDK(;
    setMoon(moonInstance);
    moonInstance.login();
  };

  useEffect(() => {
    initialize();
  }, []);

  const updateToken = async (token: string, refreshToken: string) => {
    if (moon) {
      moon.updateToken(token);
      moon.updateRefreshToken(refreshToken);

      moon.connect();
    }
  };

  const createAccount = async () => {
    if (moon) {
      const data: CreateAccountInput = {};
      const newAccount = await moon?.getAccountsSDK().createAccount(data);
      return newAccount;
    }
  };

  const listAccounts = async () => {
    if (moon) {
      return moon.listAccounts();
    }
  };

    const disconnect = async () => {
      if (moon) {
        await moon.disconnect();
        setMoon(null);
      }
    };

    return {
      moon,
      initialize,
      updateToken,
      createAccount,
      listAccounts,
    }

  }
```

The useMoonHook can be imported into various components of the React project:

```jsx
import { useMoonHook } from '@moonup/react';

const { moon, updateToken, createAccount, listAccounts } = useMoonHook();
```

> 💡It's worth noting that while this guide focuses on integrating the Moon SDK within the React/Next.js Moon Create boilerplate environment, using TypeScript as a default language, there are numerous alternative methods for incorporating the SDK into projects.
