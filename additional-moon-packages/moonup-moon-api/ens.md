# Ens



### Usage

```typescript
import { HttpClient, RequestParams } from '@moonup/moon-api';
import { Ens } from '@moonup/moon-api';
import { EnsResolveInput } from '@moonup/moon-api';

// Initialize HttpClient
const httpClient = new HttpClient();

// Initialize Ens
const ens = new Ens(httpClient);

// Example data
const ensResolveInput: EnsResolveInput = { /* your data here */ };

// Use resolve
ens.resolve(ensResolveInput);
```

### Ens Class

This class provides methods to interact with Ethereum Name Service (ENS).

#### `constructor(http: HttpClient<SecurityDataType>)`

Creates a new instance of the Ens class.

#### `resolve(data: EnsResolveInput, params: RequestParams = {})`

Resolves an ENS name to its corresponding address.

Please note that this is a basic documentation. For a complete and useful documentation, each method should have a detailed description, including its parameters, return value, and any side effects or errors it might produce.
