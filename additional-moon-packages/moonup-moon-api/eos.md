# EOS



### Usage

```typescript
import { HttpClient, RequestParams } from '@moonup/moon-api';
import { Eos } from '@moonup/moon-api';

// Initialize HttpClient
const httpClient = new HttpClient();

// Initialize Eos
const eos = new Eos(httpClient);

// Example data
const accountName = 'myEosAccount';
const eosInput = { /* your data here */ };
const eosTransactionInput = { /* your data here */ };

// Use createEosAccount
eos.createEosAccount(eosInput);

// Use getEosAccount
eos.getEosAccount(accountName);

// Use listEosAccounts
eos.listEosAccounts();

// Use signEosTransaction
eos.signEosTransaction(accountName, eosTransactionInput);
```

### Eos Class

This class provides methods to interact with EOS accounts.

#### `constructor(http: HttpClient<SecurityDataType>)`

Creates a new instance of the Eos class.

#### `createEosAccount(data: EosInput, params: RequestParams = {})`

Creates a new EOS account.

#### `getEosAccount(accountName: string, params: RequestParams = {})`

Fetches details of a specific EOS account.

#### `listEosAccounts(params: RequestParams = {})`

Lists all EOS accounts.

#### `signEosTransaction(accountName: string, data: EosTransactionInput, params: RequestParams = {})`

Signs an EOS transaction.

Please note that this is a basic documentation. For a complete and useful documentation, each method should have a detailed description, including its parameters, return value, and any side effects or errors it might produce.
