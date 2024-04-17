# Authentication

# Authenticating a user

Moon users can be authenticated using an **email and password** or **Ethereum address**. 

<aside>
📧 **Email and Password login using OAuth 2.0:**

A user can login with their email and password using OAuth 2.0. 

More details here:

[OAuth 2.0](Authentication%20750f0518f1d64f82a7ef38dd5cbc4b64/OAuth%202%200%20bb827a25ff8f4952abd36548961d97be.md)

</aside>

<aside>
⛓️ **Ethereum Address login using SIWE (Sign In With Ethereum):**

You can log a user in with their Ethereum address using SIWE.

More details here:

[SIWE](Authentication%20750f0518f1d64f82a7ef38dd5cbc4b64/SIWE%20d911f742cd684feca1f334c41c785602.md)

</aside>

# **Authentication for Development and Automation**

The Moon SDK also offers an authentication method that provides an **infinite expiry** token. This authentication approach uses an **API key** and is ideal for scenarios requiring sustained access without the need for session renewal, catering specifically to developer-facing applications where automation processes may be necessary.

**Below is an example illustrating how to use an API key within a developer application to generate a non-expiring API Token:**

```tsx
import { Accounts, ContentType } from '@moonup/moon-api'
const baseApiParams: ApiConfig = {
    baseUrl:
    'https://moon-vault-api-git-ew-supabase-migration-moonup.vercel.app',
    baseApiParams: {
        secure: true,
        type: ContentType.Json,
        format: 'json',
    }
},
// eslint-disable-next-line @typescript-eslint/no-explicit-any
securityWorker: async (securityData: any) => {
    return Promise.resolve({
        headers: {
            'X-API-KEY: `${securityData.token}`,
        },
    });
    },
};
const accounts = new Accounts(baseApiParams);
accounts..setSecurityData({
    token: token,
});
const newAccount = await accounts.createAccount({})
const accounts = await accounts.listAccounts()
```