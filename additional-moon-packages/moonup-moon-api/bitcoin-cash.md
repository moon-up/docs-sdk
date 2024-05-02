# Bitcoin Cash

### Usage

```typescript
import { HttpClient, RequestParams } from '@moonup/moon-api';
import { Bitcoincash } from '@moonup/moon-api';

// Initialize HttpClient
const httpClient = new HttpClient();

// Initialize Bitcoincash
const bitcoincash = new Bitcoincash(httpClient);

// Example data
const accountName = 'myBitcoinCashAccount';
const bitcoinCashInput = { /* your data here */ };
const bitcoinCashTransactionInput = { /* your data here */ };

// Use createBitcoinCashAccount
bitcoincash.createBitcoinCashAccount(bitcoinCashInput);

// Use getBitcoinCashAccount
bitcoincash.getBitcoinCashAccount(accountName);

// Use listBitcoinCashAccounts
bitcoincash.listBitcoinCashAccounts();

// Use signBitcoinCashTransaction
bitcoincash.signBitcoinCashTransaction(accountName, bitcoinCashTransactionInput);
```

### Bitcoincash Class

This class provides methods to interact with Bitcoin Cash accounts.

#### `constructor(http: HttpClient<SecurityDataType>)`

Creates a new instance of the Bitcoincash class.

#### `createBitcoinCashAccount(data: BitcoinCashInput, params: RequestParams = {})`

Creates a new Bitcoin Cash account.

#### `getBitcoinCashAccount(accountName: string, params: RequestParams = {})`

Fetches details of a specific Bitcoin Cash account.

#### `listBitcoinCashAccounts(params: RequestParams = {})`

Lists all Bitcoin Cash accounts.

#### `signBitcoinCashTransaction(accountName: string, data: BitcoinCashTransactionInput, params: RequestParams = {})`

Signs a Bitcoin Cash transaction.

Please note that this is a basic documentation. For a complete and useful documentation, each method should have a detailed description, including its parameters, return value, and any side effects or errors it might produce.
