# Bitcoin

### Usage

```typescript
import { HttpClient, RequestParams } from '@moonup/moon-api';
import { Bitcoin } from '@moonup/moon-api';

// Initialize HttpClient
const httpClient = new HttpClient();

// Initialize Bitcoin
const bitcoin = new Bitcoin(httpClient);

// Example data
const accountName = 'myBitcoinAccount';
const bitcoinInput = { /* your data here */ };
const bitcoinTransactionInput = { /* your data here */ };

// Use createBitcoinAccount
bitcoin.createBitcoinAccount(bitcoinInput);

// Use getBitcoinAccount
bitcoin.getBitcoinAccount(accountName);

// Use listBitcoinAccounts
bitcoin.listBitcoinAccounts();

// Use signBitcoinTransaction
bitcoin.signBitcoinTransaction(accountName, bitcoinTransactionInput);
```

### Functions

This class provides methods to interact with Bitcoin accounts.

#### `constructor(http: HttpClient<SecurityDataType>)`

Creates a new instance of the Bitcoin class.

#### `createBitcoinAccount(data: BitcoinInput, params: RequestParams = {})`

Creates a new Bitcoin account.

#### `getBitcoinAccount(accountName: string, params: RequestParams = {})`

Fetches details of a specific Bitcoin account.

#### `listBitcoinAccounts(params: RequestParams = {})`

Lists all Bitcoin accounts.

#### `signBitcoinTransaction(accountName: string, data: BitcoinTransactionInput, params: RequestParams = {})`

Signs a Bitcoin transaction.

Please note that this is a basic documentation. For a complete and useful documentation, each method should have a detailed description, including its parameters, return value, and any side effects or errors it might produce.
