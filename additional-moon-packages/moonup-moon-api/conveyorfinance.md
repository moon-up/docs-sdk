# ConveyorFinance



### Usage

```typescript
import { HttpClient, RequestParams } from '@moonup/moon-api'';
import { Conveyorfinance } from '@moonup/moon-api';
import { TokenSwapParams } from '@moonup/moon-api';

// Initialize HttpClient
const httpClient = new HttpClient();

// Initialize Conveyorfinance
const conveyorfinance = new Conveyorfinance(httpClient);

// Example data
const name = 'myName';
const tokenSwapParams: TokenSwapParams = { /* your data here */ };

// Use swap
conveyorfinance.swap(name, tokenSwapParams);
```

### Conveyorfinance Class

This class provides methods to interact with the Conveyor Finance protocol.

#### `constructor(http: HttpClient<SecurityDataType>)`

Creates a new instance of the Conveyorfinance class.

#### `swap(name: string, data: TokenSwapParams, params: RequestParams = {})`

Initiates a token swap operation in the Conveyor Finance protocol.

Please note that this is a basic documentation. For a complete and useful documentation, each method should have a detailed description, including its parameters, return value, and any side effects or errors it might produce.
