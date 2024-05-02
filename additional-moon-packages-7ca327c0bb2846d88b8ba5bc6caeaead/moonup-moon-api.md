# @moonup/moon-api

## Moon API

## **About Moon API:**

**Moon API provides low level API endpoint wrappers with expected input and output data types.**

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

```

## Classes

\
[aave.md](../additional-moon-packages/moonup-moon-api/aave.md "mention")

[accounts.md](../additional-moon-packages/moonup-moon-api/accounts.md "mention")

[bitcoin.md](../additional-moon-packages/moonup-moon-api/bitcoin.md "mention")

[bitcoin-cash.md](../additional-moon-packages/moonup-moon-api/bitcoin-cash.md "mention")

[conveyorfinance.md](../additional-moon-packages/moonup-moon-api/conveyorfinance.md "mention")

[cosmos.md](../additional-moon-packages/moonup-moon-api/cosmos.md "mention")

[ens.md](../additional-moon-packages/moonup-moon-api/ens.md "mention")

[eos.md](../additional-moon-packages/moonup-moon-api/eos.md "mention")

[erc20.md](../additional-moon-packages/moonup-moon-api/erc20.md "mention")

[erc721.md](../additional-moon-packages/moonup-moon-api/erc721.md "mention")

[erc1155.md](../additional-moon-packages/moonup-moon-api/erc1155.md "mention")

[litecoin.md](../additional-moon-packages/moonup-moon-api/litecoin.md "mention")

[oneinch.md](../additional-moon-packages/moonup-moon-api/oneinch.md "mention")

[onramper.md](../additional-moon-packages/moonup-moon-api/onramper.md "mention")

[ripple.md](../additional-moon-packages/moonup-moon-api/ripple.md "mention")

[solana.md](../additional-moon-packages/moonup-moon-api/solana.md "mention")

[tron.md](../additional-moon-packages/moonup-moon-api/tron.md "mention")

[uniswap.md](../additional-moon-packages/moonup-moon-api/uniswap.md "mention")

[yearn.md](../additional-moon-packages/moonup-moon-api/yearn.md "mention")
