# @moonup/moon-api

\
\
Installation

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
npm install @moonup/moon-api
```
{% endtab %}
{% endtabs %}



Usage

```typescript
import { Accounts, ContentType } from '@moonup/moon-api'
const baseApiParams: ApiConfig = {
    baseUrl:
    'https://beta.usemoon.ai',
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
            Authorization: `Bearer ${securityData.token}`,
        },
    });
    },
};
const accounts = new Accounts(baseApiParams);
accounts.setSecurityData({
    token: token,
});
const newAccount = await accounts.createAccount({})
const accounts = await accounts.listAccounts()
```
