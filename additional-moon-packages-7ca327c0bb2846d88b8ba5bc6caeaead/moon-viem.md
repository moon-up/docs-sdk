# @moonup/viem

### @moonup/viem



Viem library

#### usage



Install the package



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



import the provider

```typescript
import { MoonSDK } from '@moonup/moon-sdk'
import { createAccount } from '@moonup/viem'
const sdk = new MoonSDK()
const config = {
    SDK: sdk,
    ethereumAddress: '0x000',
}
const viem = createAccount(config)
const account = await viem.getAccount()
```
