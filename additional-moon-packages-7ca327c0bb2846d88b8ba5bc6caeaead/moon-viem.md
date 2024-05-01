# Moon viem

### @moonup/viem



Viem library

#### usage



Install the package

```
npm install @moonup/viem
```

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
