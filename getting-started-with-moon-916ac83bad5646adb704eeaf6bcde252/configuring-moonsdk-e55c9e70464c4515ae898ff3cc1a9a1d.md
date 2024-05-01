# Configuring MoonSDK

Configuring the Moon SDK involves setting up various modules and authentication parameters to ensure smooth communication with Moon APIs.

When leveraging React, the Moon SDK seamlessly integrates with a project's codebase through two primary interfaces:

1. **Moon SDK React Component:** A React Component that loads the SDK and manages state. 
2.  **useMoonHook:** a React Hook that returns the SDK's key methods and state variables.

## 🌚**MoonSDK React Component**

Import into a React project with the following import statement:

```jsx
import { MoonSDK } from '@moonup/moon-sdk';
```

The Moon SDK houses numerous modules for handling blockchain transactions, accounts, authentication, and specific blockchain protocols like Ethereum, Bitcoin, Solana, etc.

The MoonSDK class is defined with a constructor that takes a configuration object as a parameter. This configuration object, known as MoonSDKConfig, encapsulates essential setup parameters required for initializing the Moon SDK. It encompasses authentication settings which specify the type of authentication token and any associated credentials, storage options dictating how data is stored locally or remotely, and a list of supported networks detailing blockchain networks compatible with the SDK. The MoonSDKConfig structure code below is composed of three key components: 

1. **Auth:** defines authentication-related configurations through the MoonToken interface
2. **Storage:** specifies storage settings through the MoonStorage interface
3. **Networks:** an array of Chain objects representing supported blockchain networks.

```jsx
export interface MoonSDKConfig {
	Auth: MoonToken;
	Storage: MoonStorage;
	Networks: Chain[];
}
```

Below is an example MoonSDK initialization function showcasing authentication, storage, and network setup. It utilizes the Sepolia testnet, defined within the Chain array. The moonInstance variable, responsible for setting up the new MoonSDK, references this network configuration alongside authentication and storage parameters.

```tsx

const initialize = async () => {
	const chains: Chain[] = [{
		chainId: "11155111",	
		chainName: "Sepolia Testnet (Ethereum)",
		nativeCurrency: {	
		name: "ETH",	
		symbol: "ETH",	
		decimals: 18,
	},
	rpcUrls: ['wss://ethereum-sepolia.publicnode.com'],
	blockExplorerUrls: ['https://sepolia.etherscan.io/'],
	}];
	
const moonInstance = new MoonSDK({
	Storage: {
		key: MOON_SESSION_KEY,
		type: Storage.SESSION,
	},
	Auth: {
		AuthType: AUTH.JWT,
	},
		Networks: 
		chains,
	});

	setMoon(moonInstance);
	moonInstance.login();
};
```

## 🪝**useMoonHook**

The Moon SDK class defines methods for performing various tasks related to blockchain operations. These methods encompass functions for logging in, refreshing tokens, listing accounts, signing transactions/messages/typed data, sending transactions, and updating configurations.

The useMoonHook can utilize these functions from the SDK to import into various components of a project.

Below is an example of a useMoonHook that includes functions from the API library such as creating an account, listing accounts, updating tokens, etc.:

```jsx
export const useMoonHook = () => {

  const [moon, setMoon] = useState<MoonSDK | null>(null);

  const initialize = async () => {

    const chains: Chain[] = [{
      chainId: "11155111",
      chainName: "Sepolia Testnet (Ethereum)",
      nativeCurrency: {
        name: "ETH",
        symbol: "ETH",
        decimals: 18,
      },
      rpcUrls: ['wss://ethereum-sepolia.publicnode.com'],
      blockExplorerUrls: ['https://sepolia.etherscan.io/'],
    }];

    const moonInstance = new MoonSDK({
      Storage: {
        key: MOON_SESSION_KEY,
        type: Storage.SESSION,
      },
      Auth: {
        AuthType: AUTH.JWT,
      },
      Networks: chains,
    });
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
        sessionStorage.removeItem(MOON_SESSION_KEY);
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
import { useMoonHook } from './usemoonhook';
.....
  const { moon, updateToken, createAccount, listAccounts } = useMoonHook();
```

> 💡It's worth noting that while this guide focuses on integrating the Moon SDK within the React/Next.js Moon Create boilerplate environment, using TypeScript as a default language, there are numerous alternative methods for incorporating the SDK into projects.
>