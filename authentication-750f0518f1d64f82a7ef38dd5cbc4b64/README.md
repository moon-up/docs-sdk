# Authentication

## Supported Authentication Methods

Usemoon.ai supports various authentication methods to ensure a secure and convenient user experience. These methods include:

### Email and Password

A user can log in with their email and password. This method is a traditional way to authenticate users and is widely used.

[#email-and-password](./#email-and-password "mention")

### OAuth2 Login with Moon

This method allows users to log in using OAuth2, which is a standard protocol for authorization. It provides a secure and efficient way to authenticate users without sharing their passwords.

[oauth-2-0-bb827a25ff8f4952abd36548961d97be.md](oauth-2-0-bb827a25ff8f4952abd36548961d97be.md "mention")

### OAuth2 with Custom Providers

In addition to Moon's OAuth2 login, usemoon.ai also supports OAuth2 with custom providers. This means you can integrate with your existing authentication system or use a third-party provider to authenticate users.

[oauth-2.0.md](oauth-2.0.md "mention")

### Sign In with Ethereum (SIWE)

Usemoon.ai supports Ethereum address login using SIWE. This method allows users to log in using their Ethereum address and a signature, which is a secure and decentralized way to authenticate users.

[siwe-d911f742cd684feca1f334c41c785602.md](siwe-d911f742cd684feca1f334c41c785602.md "mention")

### WebAuthn/Passkey Authentication

Usemoon.ai supports WebAuthn/Passkey authentication, which is a standard for passwordless authentication using public key cryptography. This method provides a secure and convenient way to authenticate users without the need for passwords.

[passkey.md](../authentication/passkey.md "mention")

### API Key Authentication

Usemoon.ai also offers an authentication method that provides an infinite expiry token. This method uses an API key and is ideal for scenarios requiring sustained access without the need for session renewal. This is particularly useful for developer-facing applications where automation processes may be necessary.

[api-key.md](api-key.md "mention")

### Embedded Accounts

Usemoon.ai supports embedded accounts, which allow users to create an account within another application. This method provides a seamless user experience and eliminates the need for users to create a separate account.

[embedded-accounts.md](embedded-accounts.md "mention")

### Token Refreshing

Usemoon.ai supports token refreshing, which allows users to obtain a new access token without having to re-authenticate. This method provides a convenient way to maintain access to protected resources without the need for users to re-enter their credentials.

[token-refreshing.md](../authentication/token-refreshing.md "mention")
