# Utilizing Moon Wallets with Ethers & Wagmi

## 🌙Utilizing Moon Wallets with Ethers

Ethers.js provides robust functionality for creating wallets on various blockchain networks, including Ethereum, Bitcoin, Solana, Ripple, Litecoin, and more. Moon can leverage Ethers.js to generate new wallet instances with unique public-private key pairs for each user request.

Ethers.js facilitates secure communication between the Moon backend and blockchain networks by providing encryption and authentication mechanisms. Moon can utilize Ethers.js to establish secure channels for transferring JWT tokens between backend servers and external services like HashCorpVault for wallet creation authorization.

<aside>
👀 **More info on Moon Ethers:**

[Moon Ethers](../Additional%20Moon%20packages%207ca327c0bb2846d88b8ba5bc6caeaead/Moon%20Ethers%20f381fbf881c647e1aab3d43fb4ad0600.md)

</aside>

## 🌙Utilizing Moon Wallets with Wagmi

Moon can leverage Wagmi's context provider for React applications to seamlessly integrate wallet creation functionalities into its frontend interface. By wrapping the Moon application with Wagmi's context provider, developers can ensure that the application is aware of Wagmi's state and caching mechanisms, enhancing user experience and performance.

Wagmi simplifies the process of displaying wallet options to users by providing components like WalletOptions, which can render a list of available connectors retrieved from Wagmi. Moon can integrate Wagmi's components into its frontend interface to allow users to select their desired blockchain network for wallet creation easily.

<aside>
👀 **More info on Moon Wagmi:**

[Moon Wagmi](../Additional%20Moon%20packages%207ca327c0bb2846d88b8ba5bc6caeaead/Moon%20Wagmi%203d44fd4699594c2397129482dc52589f.md)

</aside>