# @moonup/moon-api

## Moon API

## **About Moon API:**

**Moon API provides low level API endpoint wrappers with expected input and output data types**



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





## Configuration

```typescript
import { Accounts, ContentType, HttpClient } from '@moonup/moon-api'
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



const http = new HttpClient(baseApiParams);
http.setSecurityData({
    token: token,
});
const accounts = new Accounts(http)
const newAccount = await accounts.createAccount({})
const accounts = await accounts.listAccounts()
```
