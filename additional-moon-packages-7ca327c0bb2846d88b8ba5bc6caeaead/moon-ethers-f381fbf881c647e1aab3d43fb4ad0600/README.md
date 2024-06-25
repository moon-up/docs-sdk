# @moonup/ethers

## @moonup/ethers Package Documentation

### Summary

The `@moonup/ethers` package is a utility package that provides a `MoonProvider` class and a `MoonSigner` class for interacting with Ethereum-based blockchains using the MoonSDK from the `@moonup/moon-sdk` package. The `MoonProvider` class implements the `Provider` and `IEthereumProvider` interfaces from the `ethers` library, while the `MoonSigner` class implements the `Signer` and `TypedDataSigner` interfaces from the `ethers` library.

### Setup

To use the `@moonup/ethers` package, you need to install it and import the `MoonProvider` and `MoonSigner` classes.

#### To install Moon Ethers:

{% tabs %}
{% tab title="npm" %}
```bash
npm install @moonup/ethers
```
{% endtab %}

{% tab title="yarn" %}
```bash
yarn add @moonup/ethers
```
{% endtab %}

{% tab title="pnpm" %}
```bash
pnpm add @moonup/ethers
```
{% endtab %}
{% endtabs %}

#### Importing the classes

To import the `MoonProvider` and `MoonSigner` classes, you can use the following code:

```javascript
import { MoonProvider, MoonSigner } from '@moonup/ethers';
```

### Usage

#### MoonProvider

The `MoonProvider` class is a provider for interacting with Ethereum-based blockchains using the MoonSDK. It can be used to sign messages, transactions, and typed data using the MoonSDK, and it implements the `Provider` and `IEthereumProvider` interfaces from the `ethers` library.

To create a new instance of the `MoonProvider` class, you need to provide a configuration object that contains the following properties:

* `SDK` (MoonSDK): An instance of the MoonSDK.
* `address` (string): The Ethereum address of the account.
* `chainId` (number): The ID of the Ethereum chain.

Here's an example of how to create a new instance of the `MoonProvider` class:

```javascript
import { MoonSDK } from '@moonup/moon-sdk';
import { MoonProvider } from '@moonup/ethers';

const SDK = new MoonSDK({ /* your configuration */ });
const address = '0xYourEthereumAddress';
const chainId = 1; // mainnet

const provider = new MoonProvider({ SDK, address, chainId });
```

Documentation here:

[`MoonProvider`](moonprovider-98424fc361554e529b42c6618739e9be.md)

#### MoonSigner

The `MoonSigner` class is a signer for signing messages, transactions, and typed data using the MoonSDK. It implements the `Signer` and `TypedDataSigner` interfaces from the `ethers` library.

To create a new instance of the `MoonSigner` class, you need to provide a configuration object that contains the following properties:

* `SDK` (MoonSDK): An instance of the MoonSDK.
* `address` (string): The Ethereum address of the account.
* `chainId` (number): The ID of the Ethereum chain.

Here's an example of how to create a new instance of the `MoonSigner` class:

```javascript
import { MoonSDK } from '@moonup/moon-sdk';
import { MoonSigner } from '@moonup/ethers';

const SDK = new MoonSDK({ /* your configuration */ });
const address = '0xYourEthereumAddress';
const chainId = 1; // mainnet

const signer = new MoonSigner({ SDK, address, chainId });
```

Documentation here:

[MoonSigner](moonsigner-48c2980a33ab459b98198d189f18f641.md)

### Additional notes

* The `MoonProvider` class can be connected to a `MoonSigner` instance using the `getSigner` method.
* The `MoonSigner` class can be connected to a `MoonProvider` instance using the `connect` method.
* The `MoonProvider` class and the `MoonSigner` class can be used with other `ethers` classes and functions, such as `Contract`, `Wallet`, and `utils`.
* The `MoonProvider` class and the `MoonSigner` class are compatible with the Ethereum JSON-RPC API, which means that they can be used with other Ethereum clients and tools that support JSON-RPC.
* The `MoonProvider` class and the `MoonSigner` class are designed to be used with the MoonSDK, which is a software development kit for building decentralized applications on the Moonbeam and Moonriver networks. However, they can also be used with other Ethereum-based blockchains that support the Ethereum JSON-RPC API.

