# Authentication



## Authenticating a user

Moon users can be authenticated using an **email and password** or **Ethereum address**.

#### Email and Password login using OAuth 2.0:

A user can login with their email and password using OAuth 2.0.

More details here:

[OAuth 2.0](oauth-2-0.md)

#### Ethereum Address login using SIWE (Sign In With Ethereum):

You can log a user in with their Ethereum address using SIWE.

More details here:

[SIWE](siwe.md)

## **Authentication for Development and Automation**

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
