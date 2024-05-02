# Ripple

### Usage

```typescript
import { HttpClient, RequestParams } from '@moonup/moon-api';
import { Ripple } from '@moonup/moon-api';
import { RippleInput, RippleTransactionInput } from '@moonup/moon-api';

// Initialize HttpClient
const httpClient = new HttpClient// Initialize Ripple
const ripple = new Ripple(httpClient);

// Example data
const rippleInput: RippleInput = { /* your data here */ };
const rippleTransactionInput: RippleTransactionInput = { /* your data here */ };
const accountName = 'myAccount';

// Use createRippleAccount
ripple.createRippleAccount(rippleInput);

// Use getRippleAccount
ripple.getRippleAccount(accountName);

// Use listRippleAccounts
ripple.listRippleAccounts();

// Use signRippleTransaction
ripple.signRippleTransaction(accountName, rippleTransactionInput);
```

### Ripple Class

This class provides methods to interact with Ripple accounts and transactions.

#### `constructor(http: HttpClient<SecurityDataType>)`

Creates a new instance of the Ripple class.

#### `createRippleAccount(data: RippleInput, params: RequestParams = {})`

Creates a new Ripple account.

#### `getRippleAccount(accountName: string, params: RequestParams = {})`

Fetches data for a specific Ripple account.

#### `listRippleAccounts(params: RequestParams = {})`

Lists all Ripple accounts.

#### `signRippleTransaction(accountName: string, data: RippleTransactionInput, params: RequestParams = {})`

Signs a Ripple transaction.
