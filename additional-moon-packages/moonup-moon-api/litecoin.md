# Litecoin

### Usage

```typescript
import { HttpClient, RequestParams } from '@moonup/moon-api';
import { Litecoin } from '@moonup/moon-api';
import { LitecoinInput, LitecoinTransactionInput } from '@moonup/moon-api';

// Initialize HttpClient
const httpClient = new HttpClient// Initialize Litecoin
const litecoin = new Litecoin(httpClient);

// Example data
const litecoinInput: LitecoinInput = { /* your data here */ };
const litecoinTransactionInput: LitecoinTransactionInput = { /* your data here */ };
const accountName = 'myAccount';

// Use createLitecoinAccount
litecoin.createLitecoinAccount(litecoinInput);

// Use getLitecoinAccount
litecoin.getLitecoinAccount(accountName);

// Use listLitecoinAccounts
litecoin.listLitecoinAccounts();

// Use signLitecoinTransaction
litecoin.signLitecoinTransaction(accountName, litecoinTransactionInput);
```

### Litecoin Class

This class provides methods to interact with Litecoin accounts and transactions.

#### `constructor(http: HttpClient<SecurityDataType>)`

Creates a new instance of the Litecoin class.

#### `createLitecoinAccount(data: LitecoinInput, params: RequestParams = {})`

Creates a new Litecoin account.

#### `getLitecoinAccount(accountName: string, params: RequestParams = {})`

Fetches data for a specific Litecoin account.

#### `listLitecoinAccounts(params: RequestParams = {})`

Lists all Litecoin accounts.

#### `signLitecoinTransaction(accountName: string, data: LitecoinTransactionInput, params: RequestParams = {})`

Signs a Litecoin transaction.
