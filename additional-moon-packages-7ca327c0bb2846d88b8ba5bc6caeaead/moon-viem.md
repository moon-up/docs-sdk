# @moonup/viem

## @moonup/viem Package Documentation

The `@moonup/viem` package is a utility package that allows for the creation of a local account using the MoonSDK from the `@moonup/moon-sdk` package. This local account can be used with the `viem` library for signing messages, transactions, and typed data.=

## **Installing Moon Viem:**

To utilize the Moon Viem package, first install it to the desired directory of the project:

#### To install Moon Viem:

{% tabs %}
{% tab title="npm" %}
```bash
npm install @moonup/viem
```
{% endtab %}

{% tab title="yarn" %}
```bash
yarn install @moonup/viem
```
{% endtab %}

{% tab title="pnpm" %}
```bash
pnpm add @moonup/viem
```
{% endtab %}
{% endtabs %}

### Usage Examples

Here's a basic example of how to use the `createMoonAccount` function:

```javascript
import { MoonSDK } from '@moonup/moon-sdk';
import { createMoonAccount } from '@moonup/viem';

const sdk = new MoonSDK({ /* your configuration */ });
const ethereumAddress = '0xYourEthereumAddress';

const account = await createMoonAccount({ sdk, ethereumAddress });

// Now you can use the account with viem
```

### API Reference

#### `createMoonAccount`

Creates a local account using the MoonSDK.

**Parameters**

* `input` (Object)
  * `sdk` (MoonSDK): An instance of the MoonSDK.
  * `ethereumAddress` (string): The Ethereum address of the account.

**Returns**

A promise that resolves to a `LocalAccount` object.

**Example**

```javascript
const account = await createMoonAccount({ sdk, ethereumAddress });
```
