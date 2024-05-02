# Accounts

### Usage

```typescript
import { HttpClient, RequestParams } from '@moonup/moon-api';
import { Accounts } from '@moonup/moon-api';

// Initialize HttpClient
const httpClient = new HttpClient();

// Initialize Accounts
const accounts = new Accounts(httpClient);

// Example data
const accountName = 'myAccount';
const broadcastInput = { /* your data here */ };
const createAccountInput = { /* your data here */ };
const deployInput = { /* your data here */ };
const getBalanceParams = { accountName };
const signMessage = { /* your data here */ };
const inputBody = { /* your data here */ };
const signTypedData = { /* your data here */ };

// Use broadcastTx
accounts.broadcastTx(accountName, broadcastInput);

// Use createAccount
accounts.createAccount(createAccountInput);

// Use deleteAccount
accounts.deleteAccount(accountName);

// Use deployContract
accounts.deployContract(accountName, deployInput);

// Use getAccount
accounts.getAccount(accountName);

// Use getBalance
accounts.getBalance(getBalanceParams);

// Use getNonce
accounts.getNonce(accountName);

// Use listAccounts
accounts.listAccounts();

// Use signMessage
accounts.signMessage(accountName, signMessage);

// Use signTransaction
accounts.signTransaction(accountName, inputBody);

// Use signTypedData
accounts.signTypedData(accountName, signTypedData);

// Use transferEth
accounts.transferEth(accountName, inputBody);
```

### Accounts Class

This class provides methods to interact with accounts.

#### `constructor(http: HttpClient<SecurityDataType>)`

Creates a new instance of the Accounts class.

#### `broadcastTx(accountName: string, data: BroadcastInput, params: RequestParams = {})`

Broadcasts a transaction.

#### `createAccount(data: CreateAccountInput, params: RequestParams = {})`

Creates a new account.

#### `deleteAccount(accountName: string, params: RequestParams = {})`

Deletes an account.

#### `deployContract(accountName: string, data: DeployInput, params: RequestParams = {})`

Deploys a contract.

#### `getAccount(accountName: string, params: RequestParams = {})`

Gets account details.

#### `getBalance({ accountName, ...query }: GetBalanceParams, params: RequestParams = {})`

Gets the balance of an account.

#### `getNonce(accountName: string, params: RequestParams = {})`

Gets the nonce of an account.

#### `listAccounts(params: RequestParams = {})`

Lists all accounts.

#### `signMessage(accountName: string, data: SignMessage, params: RequestParams = {})`

Signs a message.

#### `signTransaction(accountName: string, data: InputBody, params: RequestParams = {})`

Signs a transaction.

#### `signTypedData(accountName: string, data: SignTypedData, params: RequestParams = {})`

Signs typed data.

#### `transferEth(accountName: string, data: InputBody, params: RequestParams = {})`

Transfers ETH from an account.

