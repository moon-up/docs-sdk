# @moonup/moon-api

## @moonup/moon-api Package Documentation

The `@moonup/moon-api` package is a comprehensive library that provides a set of APIs for interacting with various blockchain networks and decentralized finance (DeFi) protocols. This package includes support for Ethereum, Bitcoin, Bitcoin Cash, Dogecoin, Litecoin, EOS, Solana, Cosmos, Tron, and more.



## **Installing Moon API:**

To use the Moon API package, first install it to a project:

#### To install Moon **API**:

{% tabs %}
{% tab title="npm" %}
```bash
npm install @moonup/moon-api
```
{% endtab %}

{% tab title="yarn" %}
```bash
yarn add @moonup/moon-api
```
{% endtab %}

{% tab title="pnpm" %}
```bash
pnpm add @moonup/moon-api
```
{% endtab %}
{% endtabs %}

### Usage

To use the `@moonup/moon-api` package, you'll first need to install it using a package manager like npm or Yarn. Once you've installed the package, you can import the classes and methods you need into your project.

Here's an example of how to use the `Accounts` class to create a new Ethereum account and transfer ETH:

```javascript
import { HttpClient, Accounts } from '@moonup/moon-api';

// Initialize the HttpClient with your API base URL and security worker
const http = new HttpClient({
  baseUrl: 'https://beta.usemoon.ai',
  securityWorker: async (securityData) => {
    return {
      headers: {
        Authorization: `Bearer ${securityData.token}`,
      },
    };
  },
});

// Create an instance of the Accounts class
const accounts = new Accounts(http);

// Create a new Ethereum account
const createAccountData = await accounts.createAccount({ private_key: 'your_private_key' });
console.log('New account created:', createAccountData.address);

// Transfer ETH from the new account to another account
const transferEthData = await accounts.transferEth(createAccountData.name, {
  to: '0xAnotherAccountAddress',
  value: '1000000000000000000', // 1 ETH in wei
});
console.log('Transfer successful:', transferEthData.transactionHash);
```

This example demonstrates how to use the `Accounts` class to create a new Ethereum account and transfer ETH to another account. The `HttpClient` class is used to make HTTP requests to the API, and the `securityWorker` function is used to add an authorization header to the requests.

### Initialization

To use the `@moonup/moon-api` package, you'll first need to initialize an `HttpClient` object with your API base URL and security worker. The security worker is a function that returns the headers to be included in the API requests. In this case, it returns an authorization header with a bearer token.

Here's an example of how to initialize the `HttpClient` object:

```javascript
import { HttpClient } from '@moonup/moon-api';

const http = new HttpClient({
  baseUrl: 'https://beta.usemoon.ai',
  securityWorker: async (securityData) => {
    return {
      headers: {
        Authorization: `Bearer ${securityData.token}`,
      },
    };
  },
});
```

In this example, the `baseUrl` property is set to the URL of the API, and the `securityWorker` property is set to a function that returns an authorization header with a bearer token. The `securityData` object is passed to the `securityWorker` function, which can be used to retrieve the bearer token.

Once you've initialized the `HttpClient` object, you can use it to create instances of the classes provided by the `@moonup/moon-api` package. For example:

```javascript
import { Accounts } from '@moonup/moon-api';

const accounts = new Accounts(http);
```

In this example, the `Accounts` class is imported from the `@moonup/moon-api` package, and an instance of the class is created using the `HttpClient` object.

## Classes

The package is organized into several files, each containing a class that provides methods for interacting with a specific blockchain network or DeFi protocol. The main files in the package are:

\
[aave.md](../additional-moon-packages/moonup-moon-api/aave.md "mention")

Provides methods for interacting with the Aave decentralized lending protocol, including borrowing, lending, and repaying assets.

[accounts.md](../additional-moon-packages/moonup-moon-api/accounts.md "mention")

Provides methods for creating and managing Ethereum accounts, deploying contracts, signing messages and transactions, and transferring ETH.

[bitcoin.md](../additional-moon-packages/moonup-moon-api/bitcoin.md "mention")

Provide methods for creating and managing Bitcoin accounts, and signing transactions

[bitcoin-cash.md](../additional-moon-packages/moonup-moon-api/bitcoin-cash.md "mention")

Provide methods for creating and managing Bitcoin Cash accounts, and signing transactions

[conveyorfinance.md](../additional-moon-packages/moonup-moon-api/conveyorfinance.md "mention")

Provide methods for interacting with the ConveyorFinance decentralized exchange (DEX) protocols, including swapping tokens and checking prices

[cosmos.md](../additional-moon-packages/moonup-moon-api/cosmos.md "mention")

Provide methods for interacting with the Cosmos  blockchain networks, including creating and managing accounts, and signing transactions.

[dogecoin.md](../additional-moon-packages/moonup-moon-api/dogecoin.md "mention")

Provide methods for creating and managing Dogecoin accounts, and signing transactions

[ens.md](../additional-moon-packages/moonup-moon-api/ens.md "mention")

Provides methods for interacting with the Ethereum Name Service (ENS), including registering and resolving domain names.

[eos.md](../additional-moon-packages/moonup-moon-api/eos.md "mention")

Provide methods for interacting with the EOS blockchain networks, including creating and managing accounts, and signing transactions.

[erc20.md](../additional-moon-packages/moonup-moon-api/erc20.md "mention")

Provide methods for interacting with Ethereum-based tokens, including transferring tokens, checking balances, and approving contracts.

[erc721.md](../additional-moon-packages/moonup-moon-api/erc721.md "mention")

Provide methods for interacting with Ethereum-based tokens, including transferring tokens, checking balances, and approving contracts.

[erc1155.md](../additional-moon-packages/moonup-moon-api/erc1155.md "mention")

Provide methods for interacting with Ethereum-based tokens, including transferring tokens, checking balances, and approving contracts.

[litecoin.md](../additional-moon-packages/moonup-moon-api/litecoin.md "mention")

Provide methods for creating and managing Litecoin accounts, and signing transactions

[oneinch.md](../additional-moon-packages/moonup-moon-api/oneinch.md "mention")

Provide methods for interacting with the 1inch decentralized exchange (DEX) protocols, including swapping tokens and checking prices

[onramper.md](../additional-moon-packages/moonup-moon-api/onramper.md "mention")

Provides methods for interacting with the Onramper fiat onramp service, allowing users to buy cryptocurrencies with fiat currency.

[ripple.md](../additional-moon-packages/moonup-moon-api/ripple.md "mention")

Provides methods for interacting with the Ripple blockchain network, including creating and managing accounts, and sending and receiving payments.

[solana.md](../additional-moon-packages/moonup-moon-api/solana.md "mention")

Provides methods for interacting with the Solana blockchain network, including creating and managing accounts, and sending and receiving tokens.

[tron.md](../additional-moon-packages/moonup-moon-api/tron.md "mention")

Provides methods for interacting with the TRON blockchain network, including creating and managing accounts, and sending and receiving tokens.

[uniswap.md](../additional-moon-packages/moonup-moon-api/uniswap.md "mention")

Provide methods for interacting with the Uniswap decentralized exchange (DEX) protocols, including swapping tokens and checking prices

[yearn.md](../additional-moon-packages/moonup-moon-api/yearn.md "mention")

Provides methods for interacting with the Yearn decentralized finance (DeFi) protocol, including depositing, withdrawing, and earning yield on assets.

Overall, the `@moonup/moon-api` package is a powerful and flexible library that provides a wide range of APIs for interacting with various blockchain networks and DeFi protocols. Whether you're building a simple wallet application or a complex decentralized finance platform, this package has the tools you need to get the job done.
