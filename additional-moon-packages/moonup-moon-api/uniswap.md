# Uniswap

### Usage

```typescript
import { HttpClient, RequestParams } from '@moonup/moon-api';
import { Uniswap } from '@moonup/moon-api';
import { UniswapInput } from '@moonup/moon-api';

// Initialize HttpClient
const httpClient = new HttpClient// Initialize Uniswap
const uniswap = new Uniswap(httpClient);

// Example data
const uniswapInput: UniswapInput = { /* your data here */ };
const poolName = 'myPool';

// Use addLiquidity
uniswap.addLiquidity(poolName, uniswapInput);

// Use removeLiquidity
uniswap.removeLiquidity(poolName, uniswapInput);

// Use swapExactEthForTokens
uniswap.swapExactEthForTokens(poolName, uniswapInput);

// Use swapExactTokensForTokens
uniswap.swapExactTokensForTokens(poolName, uniswapInput);
```

### Uniswap Class

This class provides methods to interact with Uniswap liquidity pools and transactions.

#### `constructor(http: HttpClient<SecurityDataType>)`

Creates a new instance of the Uniswap class.

#### `addLiquidity(name: string, data: UniswapInput, params: RequestParams = {})`

Adds liquidity to a Uniswap pool.

#### `removeLiquidity(name: string, data: UniswapInput, params: RequestParams = {})`

Removes liquidity from a Uniswap pool.

#### `swapExactEthForTokens(name: string, data: UniswapInput, params: RequestParams = {})`

Swaps an exact amount of Ether for tokens.

#### `swapExactTokensForTokens(name: string, data: UniswapInput, params: RequestParams = {})`

Swaps an exact amount of one token for another token.
