# Utilizing Moon Wallets with Ethers & Wagmi

## Utilizing Moon Wallets with Ethers

Ethers.js provides robust functionality for creating wallets on various blockchain networks, including Ethereum, Bitcoin, Solana, Ripple, Litecoin, and more. Moon can leverage Ethers.js to generate new wallet instances with unique public-private key pairs for each user request.

Ethers.js facilitates secure communication between the Moon backend and blockchain networks by providing encryption and authentication mechanisms. Moon can utilize Ethers.js to establish secure channels for transferring JWT tokens between backend servers and external services like HashCorpVault for wallet creation authorization.

**More info on Moon Ethers:**

[Moon Ethers](../additional-moon-packages/moon-ethers/)

## 🌙Utilizing Moon Wallets with Wagmi

Moon can leverage Wagmi's context provider for React applications to seamlessly integrate wallet creation functionalities into its frontend interface. By wrapping the Moon application with Wagmi's context provider, developers can ensure that the application is aware of Wagmi's state and caching mechanisms, enhancing user experience and performance.

Wagmi simplifies the process of displaying wallet options to users by providing components like WalletOptions, which can render a list of available connectors retrieved from Wagmi. Moon can integrate Wagmi's components into its frontend interface to allow users to select their desired blockchain network for wallet creation easily.

**More info on Moon Wagmi:**

[Moon Wagmi](../additional-moon-packages/moon-wagmi.md)
