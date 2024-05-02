# Dogecoin



### Usage

```typescript
import { HttpClient, RequestParams } from './http-client';
import { Dogecoin } from './Dogecoin';

// Initialize HttpClient
const httpClient = new HttpClient();

// Initialize Dogecoin
const dogecoin = new Dogecoin(httpClient);

// Example data
const accountName = 'myDogecoinAccount';
const dogeCoinInput = { /* your data here */ };
const dogeCoinTransactionInput = { /* your data here */ };

// Use createDogeCoinAccount
dogecoin.createDogeCoinAccount(dogeCoinInput);

// Use getDogeCoinAccount
dogecoin.getDogeCoinAccount(accountName);

// Use listDogeCoinAccounts
dogecoin.listDogeCoinAccounts();

// Use signDogeCoinTransaction
dogecoin.signDogeCoinTransaction(accountName, dogeCoinTransactionInput);
```

### Dogecoin Class

This class provides methods to interact with Dogecoin accounts.

#### `constructor(http: HttpClient<SecurityDataType>)`

Creates a new instance of the Dogecoin class.

#### `createDogeCoinAccount(data: DogeCoinInput, params: RequestParams = {})`

Creates a new Dogecoin account.

#### `getDogeCoinAccount(accountName: string, params: RequestParams = {})`

Fetches details of a specific Dogecoin account.

#### `listDogeCoinAccounts(params: RequestParams = {})`

Lists all Dogecoin accounts.

#### `signDogeCoinTransaction(accountName: string, data: DogeCoinTransactionInput, params: RequestParams = {})`

Signs a Dogecoin transaction.

Please note that this is a basic documentation. For a complete and useful documentation, each method should have a detailed description, including its parameters, return value, and any side effects or errors it might produce.
