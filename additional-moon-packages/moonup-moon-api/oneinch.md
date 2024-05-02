# OneInch

### Usage

```typescript
import { HttpClient, RequestParams } from '@moonup/moon-api';
import { Oneinch } from '@moonup/moon-api';
import { ApproveCallDataPayload, ApproveSpenderPayload, ProtocolsPayload, QuotePayload, GetSwapDto, TokensPayload } from '@moonup/moon-api';

// Initialize HttpClient
const httpClient = new HttpClient// Initialize Oneinch
const oneinch = new Oneinch(httpClient);

// Example data
const approveCallDataPayload: ApproveCallDataPayload = { /* your data here */ };
const approveSpenderPayload: ApproveSpenderPayload = { /* your data here */ };
const protocolsPayload: ProtocolsPayload = { /* your data here */ };
const quotePayload: QuotePayload = { /* your data here */ };
const getSwapDto: GetSwapDto = { /* your data here */ };
const tokensPayload: TokensPayload = { /* your data here */ };
const accountName = 'myAccount';

// Use approveCallData
oneinch.approveCallData(approveCallDataPayload);

// Use approveSpender
oneinch.approveSpender(approveSpenderPayload);

// Use protocols
oneinch.protocols(protocolsPayload);

// Use quote
oneinch.quote(quotePayload);

// Use swap
oneinch.swap(accountName, getSwapDto);

// Use tokens
oneinch.tokens(tokensPayload);
```

### Oneinch Class

This class provides methods to interact with the Oneinch API.

#### `constructor(http: HttpClient<SecurityDataType>)`

Creates a new instance of the Oneinch class.

#### `approveCallData(data: ApproveCallDataPayload, params: RequestParams = {})`

Sends a POST request to `/oneinch/approve-call-data`.

#### `approveSpender(data: ApproveSpenderPayload, params: RequestParams = {})`

Sends a POST request to `/oneinch/approve-spender`.

#### `protocols(data: ProtocolsPayload, params: RequestParams = {})`

Sends a POST request to `/oneinch/protocols`.

#### `quote(data: QuotePayload, params: RequestParams = {})`

Sends a POST request to `/oneinch/quote`.

#### `swap(accountName: string, data: GetSwapDto, params: RequestParams = {})`

Sends a POST request to `/oneinch/{accountName}/swap`.

#### `tokens(data: TokensPayload, params: RequestParams = {})`

Sends a POST request to `/oneinch/tokens`.
