# Tron

### Usage

```typescript
import { HttpClient, RequestParams } from './http-client';
import { Tron } from './Tron';
import { TronInput, TronTransactionInput } from './data-contracts';

// Initialize HttpClient
const httpClient = new HttpClient// Initialize Tron
const tron = new Tron(httpClient);

// Example data
const tronInput: TronInput = { /* your data here */ };
const tronTransactionInput: TronTransactionInput = { /* your data here */ };
const accountName = 'myAccount';

// Use createTronAccount
tron.createTronAccount(tronInput);

// Use getTronAccount
tron.getTronAccount(accountName);

// Use listTronAccounts
tron.listTronAccounts();

// Use signTronTransaction
tron.signTronTransaction(accountName, tronTransactionInput);
```

### Tron Class

This class provides methods to interact with Tron accounts and transactions.

#### `constructor(http: HttpClient<SecurityDataType>)`

Creates a new instance of the Tron class.

#### `createTronAccount(data: TronInput, params: RequestParams = {})`

Creates a new Tron account.

#### `getTronAccount(accountName: string, params: RequestParams = {})`

Fetches data for a specific Tron account.

#### `listTronAccounts(params: RequestParams = {})`

Lists all Tron accounts.

#### `signTronTransaction(accountName: string, data: TronTransactionInput, params: RequestParams = {})`

Signs a Tron transaction.
