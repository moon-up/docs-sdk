# Cosmos



### Usage

```typescript
import { HttpClient, RequestParams } from './http-client';
import { Cosmos } from './Cosmos';

// Initialize HttpClient
const httpClient = new HttpClient();

// Initialize Cosmos
const cosmos = new Cosmos(httpClient);

// Example data
const accountName = 'myCosmosAccount';
const cosmosInput = { /* your data here */ };
const cosmosTransactionInput = { /* your data here */ };

// Use createCosmosAccount
cosmos.createCosmosAccount(cosmosInput);

// Use getCosmosAccount
cosmos.getCosmosAccount(accountName);

// Use listCosmosAccounts
cosmos.listCosmosAccounts();

// Use signCosmosTransaction
cosmos.signCosmosTransaction(accountName, cosmosTransactionInput);
```



### Cosmos Class

This class provides methods to interact with Cosmos accounts.

#### `constructor(http: HttpClient<SecurityDataType>)`

Creates a new instance of the Cosmos class.

#### `createCosmosAccount(data: CosmosInput, params: RequestParams = {})`

Creates a new Cosmos account.

#### `getCosmosAccount(accountName: string, params: RequestParams = {})`

Fetches details of a specific Cosmos account.

#### `listCosmosAccounts(params: RequestParams = {})`

Lists all Cosmos accounts.

#### `signCosmosTransaction(accountName: string, data: CosmosTransactionInput, params: RequestParams = {})`

Signs a Cosmos transaction.

Please note that this is a basic documentation. For a complete and useful documentation, each method should have a detailed description, including its parameters, return value, and any side effects or errors it might produce.
