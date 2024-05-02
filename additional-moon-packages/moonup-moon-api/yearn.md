# Yearn

### Usage

```typescript
import { HttpClient, RequestParams } from '@moonup/moon-api';
import { Yearn } from '@moonup/moon-api';
import { InputBody } from '@moonup/moon-api';

// Initialize HttpClient
const httpClient = new HttpClient// Initialize Yearn
const yearn = new Yearn(httpClient);

// Example data
const inputBody: InputBody = { /* your data here */ };
const poolName = 'myPool';

// Use addLiquidity
yearn.addLiquidity(poolName, inputBody);

// Use addLiquidityWeth
yearn.addLiquidityWeth(poolName, inputBody);

// Use removeLiquidity
yearn.removeLiquidity(poolName, inputBody);

// Use removeLiquidityWeth
yearn.removeLiquidityWeth(poolName, inputBody);
```

### Yearn Class

This class provides methods to interact with Yearn liquidity pools and transactions.

#### `constructor(http: HttpClient<SecurityDataType>)`

Creates a new instance of the Yearn class.

#### `addLiquidity(name: string, data: InputBody, params: RequestParams = {})`

Adds liquidity to a Yearn pool.

#### `addLiquidityWeth(name: string, data: InputBody, params: RequestParams = {})`

Adds liquidity to a Yearn pool with WETH.

#### `removeLiquidity(name: string, data: InputBody, params: RequestParams = {})`

Removes liquidity from a Yearn pool.

#### `removeLiquidityWeth(name: string, data: InputBody, params: RequestParams = {})`

Removes liquidity from a Yearn pool with WETH.
