# OnRamper

### Usage

```typescript
import { HttpClient, RequestParams } from '@moonup/moon-api';
import { Onramper } from '@moonup/moon-api';
import { TransactionInput, OnRamperGetQuotesBuyParams, OnRamperGetQuotesSellParams, OnRamperGetSupportedAssetsParams, OnRamperGetSupportedCurrenciesParams, OnRamperGetSupportedDefaultsAllParams, OnRamperGetSupportedPaymentTypesParams, OnRamperGetSupportedPaymentTypesFiatParams } from '@moonup/moon-api';

// Initialize HttpClient
const httpClient = new HttpClient// Initialize Onramper
const onramper = new Onramper(httpClient);

// Example data
const transactionInput: TransactionInput = { /* your data here */ };
const onRamperGetQuotesBuyParams: OnRamperGetQuotesBuyParams = { /* your data here */ };
const onRamperGetQuotesSellParams: OnRamperGetQuotesSellParams = { /* your data here */ };
const onRamperGetSupportedAssetsParams: OnRamperGetSupportedAssetsParams = { /* your data here */ };
const onRamperGetSupportedCurrenciesParams: OnRamperGetSupportedCurrenciesParams = { /* your data here */ };
const onRamperGetSupportedDefaultsAllParams: OnRamperGetSupportedDefaultsAllParams = { /* your data here */ };
const onRamperGetSupportedPaymentTypesParams: OnRamperGetSupportedPaymentTypesParams = { /* your data here */ };
const onRamperGetSupportedPaymentTypesFiatParams: OnRamperGetSupportedPaymentTypesFiatParams = { /* your data here */ };
const accountName = 'myAccount';

// Use onRamperCheckout
onramper.onRamperCheckout(accountName, transactionInput);

// Use onRamperGetQuotesBuy
onramper.onRamperGetQuotesBuy(onRamperGetQuotesBuyParams);

// Use onRamperGetQuotesSell
onramper.onRamperGetQuotesSell(onRamperGetQuotesSellParams);

// Use onRamperGetSupportedAssets
onramper.onRamperGetSupportedAssets(onRamperGetSupportedAssetsParams);

// Use onRamperGetSupportedCurrencies
onramper.onRamperGetSupportedCurrencies(onRamperGetSupportedCurrenciesParams);

// Use onRamperGetSupportedDefaultsAll
onramper.onRamperGetSupportedDefaultsAll(onRamperGetSupportedDefaultsAllParams);

// Use onRamperGetSupportedOnRampsAll
onramper.onRamperGetSupportedOnRampsAll();

// Use onRamperGetSupportedPaymentTypes
onramper.onRamperGetSupportedPaymentTypes(onRamperGetSupportedPaymentTypesParams);

// Use onRamperGetSupportedPaymentTypesFiat
onramper.onRamperGetSupportedPaymentTypesFiat(onRamperGetSupportedPaymentTypesFiatParams);
```

### Onramper Class

This class provides methods to interact with the Onramper API.

#### `constructor(http: HttpClient<SecurityDataType>)`

Creates a new instance of the Onramper class.

#### `onRamperCheckout(accountName: string, data: TransactionInput, params: RequestParams = {})`

Sends a POST request to `/onramper/fund/${accountName}`.

#### `onRamperGetQuotesBuy(query: OnRamperGetQuotesBuyParams, params: RequestParams = {})`

Sends a GET request to `/onramper/quotes/buy`.

#### `onRamperGetQuotesSell(query: OnRamperGetQuotesSellParams, params: RequestParams = {})`

Sends a GET request to `/onramper/quotes/sell`.

#### `onRamperGetSupportedAssets(query: OnRamperGetSupportedAssetsParams, params: RequestParams = {})`

Sends a GET request to `/onramper/assets`.

#### `onRamperGetSupportedCurrencies(query: OnRamperGetSupportedCurrenciesParams, params: RequestParams = {})`

Sends a GET request to `/onramper/currencies`.

#### `onRamperGetSupportedDefaultsAll(query: OnRamperGetSupportedDefaultsAllParams, params: RequestParams = {})`

Sends a GET request to `/onramper/defaults`.

#### `onRamperGetSupportedOnRampsAll(params: RequestParams = {})`

Sends a GET request to `/onramper/onramps`.

#### `onRamperGetSupportedPaymentTypes(query: OnRamperGetSupportedPaymentTypesParams, params: RequestParams = {})`

Sends a GET request to `/onramper/payment-types`.

#### `onRamperGetSupportedPaymentTypesFiat(query: OnRamperGetSupportedPaymentTypesFiatParams, params: RequestParams = {})`

Sends a GET request to `/onramper/payment-types/fiat`.

