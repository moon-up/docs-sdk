# Erc20



### Usage

```typescript
import { HttpClient, RequestParams } from '@moonup/moon-api';
import { Erc20 } from '@moonup/moon-api';
import { InputBody } from '@moonup/moon-api';

// Initialize HttpClient
const httpClient = new HttpClient();

// Initialize Erc20
const erc20 = new Erc20(httpClient);

// Example data
const name = 'myErc20Token';
const inputBody: InputBody = { /* your data here */ };

// Use allowanceErc20
erc20.allowanceErc20(name, inputBody);

// Use approveErc20
erc20.approveErc20(name, inputBody);

// Use balanceOfErc20
erc20.balanceOfErc20(name, inputBody);

// Use decimalsErc20
erc20.decimalsErc20(name, inputBody);

// Use nameErc20
erc20.nameErc20(name, inputBody);

// Use symbolErc20
erc20.symbolErc20(name, inputBody);

// Use totalSupplyErc20
erc20.totalSupplyErc20(name, inputBody);

// Use transferErc20
erc20.transferErc20(name, inputBody);

// Use transferFromErc20
erc20.transferFromErc20(name, inputBody);
```



### Erc20 Class

This class provides methods to interact with ERC20 tokens.

#### `constructor(http: HttpClient<SecurityDataType>)`

Creates a new instance of the Erc20 class.

#### `allowanceErc20(name: string, data: InputBody, params: RequestParams = {})`

Fetches the amount of tokens that an owner allowed to a spender.

#### `approveErc20(name: string, data: InputBody, params: RequestParams = {})`

Approves to spend a certain amount of tokens from the owner to another address.

#### `balanceOfErc20(name: string, data: InputBody, params: RequestParams = {})`

Fetches the token balance of an account.

#### `decimalsErc20(name: string, data: InputBody, params: RequestParams = {})`

Fetches the number of decimals the token uses.

#### `nameErc20(name: string, data: InputBody, params: RequestParams = {})`

Fetches the name of the token.

#### `symbolErc20(name: string, data: InputBody, params: RequestParams = {})`

Fetches the symbol of the token.

#### `totalSupplyErc20(name: string, data: InputBody, params: RequestParams = {})`

Fetches the total token supply.

#### `transferErc20(name: string, data: InputBody, params: RequestParams = {})`

Transfers a certain amount of tokens to another address.

#### `transferFromErc20(name: string, data: InputBody, params: RequestParams = {})`

Transfers a certain amount of tokens from one address to another.
