# Solana

### Usage

```typescript
import { HttpClient, RequestParams } from '@moonup/moon-api';
import { Solana } from '@moonup/moon-api';
import { SolanaInput, SolanaTransactionInput } from '@moonup/moon-api';

// Initialize HttpClient
const httpClient = new HttpClient// Initialize Solana
const solana = new Solana(httpClient);

// Example data
const solanaInput: SolanaInput = { /* your data here */ };
const solanaTransactionInput: SolanaTransactionInput = { /* your data here */ };
const accountName = 'myAccount';

// Use createSolanaAccount
solana.createSolanaAccount(solanaInput);

// Use getSolanaAccount
solana.getSolanaAccount(accountName);

// Use listSolanaAccounts
solana.listSolanaAccounts();

// Use signSolanaTransaction
solana.signSolanaTransaction(accountName, solanaTransactionInput);
```

### Solana Class

This class provides methods to interact with Solana accounts and transactions.

#### `constructor(http: HttpClient<SecurityDataType>)`

Creates a new instance of the Solana class.

#### `createSolanaAccount(data: SolanaInput, params: RequestParams = {})`

Creates a new Solana account.

#### `getSolanaAccount(accountName: string, params: RequestParams = {})`

Fetches data for a specific Solana account.

#### `listSolanaAccounts(params: RequestParams = {})`

Lists all Solana accounts.

#### `signSolanaTransaction(accountName: string, data: SolanaTransactionInput, params: RequestParams = {})`

Signs a Solana transaction.
