# Aave



## Usage

```typescript
import { HttpClient, RequestParams } from '@moonup/moon-api';
import { Aave } from '@moonup/moon-api';

// Initialize HttpClient
const httpClient = new HttpClient();

// Initialize Aave
const aave = new Aave(httpClient);

// Example data
const name = 'myName';
const aaveInput = { /* your data here */ };

// Use borrow
aave.borrow(name, aaveInput);

// Use lend
aave.lend(name, aaveInput);

// Use repay
aave.repay(name, aaveInput);

// Use userReserveData
aave.userReserveData(name, aaveInput);

```



## Aave Class

This class provides methods to interact with the Aave protocol.

#### `constructor(http: HttpClient<SecurityDataType>)`

Creates a new instance of the Aave class.

#### `borrow(name: string, data: AaveInput, params: RequestParams = {})`

Initiates a borrow operation in the Aave protocol.

#### `lend(name: string, data: AaveInput, params: RequestParams = {})`

Initiates a lend operation in the Aave protocol.

#### `repay(name: string, data: AaveInput, params: RequestParams = {})`

Initiates a repay operation in the Aave protocol.

#### `userReserveData(name: string, data: AaveInput, params: RequestParams = {})`

Fetches user reserve data from the Aave protocol.
