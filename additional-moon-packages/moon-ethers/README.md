# @moonup/ethers

## Moon Ethers

## **About Moon Ethers:**

**Moon Ethers** bridges the powerful capabilities of the **Ethers.js** library with the **MoonSDK**, streamlining the development of Moon integrated projects.

#### 💡 What is Ethers.js?

[Ethers.js](https://docs.ethers.org/v5/) is the most popular and powerful library for interacting with the Ethereum blockchain. It enables developers to build decentralized applications without the hassle of directly managing blockchain connections or the intricacies of smart contract interactions, streamlining the development process with its comprehensive suite of tools and utilities

## **Installing Moon Ethers:**

To utilize the Moon Ethers package, first install it to the desired directory of the project:

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

{% tab title="Untitled" %}
```bash
pnpm install @moonup/ethers
```
{% endtab %}
{% endtabs %}



This will add an “ethers” package to the project’s @moonup node module.

## **Moon Ethers Provider and Signer:**

Like [**Ethers.js**](https://docs.ethers.org/v5/), **Moon Ethers** organizes its functionalities into two abstractions: **provider** and **signer**:

**The Provider:** MoonProvider\`

* offers functions that are **read-only**
*   Documentation here:

    [`MoonProvider`](moonprovider.md)

**The Signer:** \`MoonSigner\`

* offers functions that handle **signing**, **creating**, and **sending transactions**
*   Documentation here:

    [MoonSigner](moonsigner.md)
