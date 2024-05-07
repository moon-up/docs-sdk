# OnramperApi

## moonsdk.api.OnramperApi

### Load the API package

```dart
import 'package:moonsdk/api.dart';
```

All URIs are relative to _https://beta.usemoon.ai_

| Method                                                                                          | HTTP request                           | Description |
| ----------------------------------------------------------------------------------------------- | -------------------------------------- | ----------- |
| [**onRamperCheckout**](onramperapi.md#onrampercheckout)                                         | **POST** /onramper/fund/${accountName} |             |
| [**onRamperGetQuotesBuy**](onramperapi.md#onrampergetquotesbuy)                                 | **GET** /onramper/quotes/buy           |             |
| [**onRamperGetQuotesSell**](onramperapi.md#onrampergetquotessell)                               | **GET** /onramper/quotes/sell          |             |
| [**onRamperGetSupportedAssets**](onramperapi.md#onrampergetsupportedassets)                     | **GET** /onramper/assets               |             |
| [**onRamperGetSupportedCurrencies**](onramperapi.md#onrampergetsupportedcurrencies)             | **GET** /onramper/currencies           |             |
| [**onRamperGetSupportedDefaultsAll**](onramperapi.md#onrampergetsupporteddefaultsall)           | **GET** /onramper/defaults             |             |
| [**onRamperGetSupportedOnRampsAll**](onramperapi.md#onrampergetsupportedonrampsall)             | **GET** /onramper/onramps              |             |
| [**onRamperGetSupportedPaymentTypes**](onramperapi.md#onrampergetsupportedpaymenttypes)         | **GET** /onramper/payment-types        |             |
| [**onRamperGetSupportedPaymentTypesFiat**](onramperapi.md#onrampergetsupportedpaymenttypesfiat) | **GET** /onramper/payment-types/fiat   |             |

## **onRamperCheckout**

> JsonObject onRamperCheckout(authorization, accountName, transactionInput)

#### Example

```dart
import 'package:moonsdk/api.dart';
// TODO Configure API key authorization: ApiKeyAuth
//defaultApiClient.getAuthentication<ApiKeyAuth>('ApiKeyAuth').apiKey = 'YOUR_API_KEY';
// uncomment below to setup prefix (e.g. Bearer) for API key, if needed
//defaultApiClient.getAuthentication<ApiKeyAuth>('ApiKeyAuth').apiKeyPrefix = 'Bearer';
// TODO Configure API key authorization: BearerAuth
//defaultApiClient.getAuthentication<ApiKeyAuth>('BearerAuth').apiKey = 'YOUR_API_KEY';
// uncomment below to setup prefix (e.g. Bearer) for API key, if needed
//defaultApiClient.getAuthentication<ApiKeyAuth>('BearerAuth').apiKeyPrefix = 'Bearer';

final api = Moonsdk().getOnramperApi();
final String authorization = authorization_example; // String | 
final String accountName = accountName_example; // String | 
final TransactionInput transactionInput = ; // TransactionInput | 

try {
    final response = api.onRamperCheckout(authorization, accountName, transactionInput);
    print(response);
} catch on DioException (e) {
    print('Exception when calling OnramperApi->onRamperCheckout: $e\n');
}
```

#### Parameters

| Name                 | Type                                        | Description | Notes |
| -------------------- | ------------------------------------------- | ----------- | ----- |
| **authorization**    | **String**                                  |             |       |
| **accountName**      | **String**                                  |             |       |
| **transactionInput** | [**TransactionInput**](transactioninput.md) |             |       |

#### Return type

[**JsonObject**](../../dart/doc/JsonObject.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](onramperapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## **onRamperGetQuotesBuy**

> BuiltList onRamperGetQuotesBuy(authorization, fiat, crypto, amount, paymentMethod, uuid, clientName, country)

#### Example

```dart
import 'package:moonsdk/api.dart';
// TODO Configure API key authorization: ApiKeyAuth
//defaultApiClient.getAuthentication<ApiKeyAuth>('ApiKeyAuth').apiKey = 'YOUR_API_KEY';
// uncomment below to setup prefix (e.g. Bearer) for API key, if needed
//defaultApiClient.getAuthentication<ApiKeyAuth>('ApiKeyAuth').apiKeyPrefix = 'Bearer';
// TODO Configure API key authorization: BearerAuth
//defaultApiClient.getAuthentication<ApiKeyAuth>('BearerAuth').apiKey = 'YOUR_API_KEY';
// uncomment below to setup prefix (e.g. Bearer) for API key, if needed
//defaultApiClient.getAuthentication<ApiKeyAuth>('BearerAuth').apiKeyPrefix = 'Bearer';

final api = Moonsdk().getOnramperApi();
final String authorization = authorization_example; // String | 
final String fiat = fiat_example; // String | 
final String crypto = crypto_example; // String | 
final double amount = 1.2; // double | 
final String paymentMethod = paymentMethod_example; // String | 
final String uuid = uuid_example; // String | 
final String clientName = clientName_example; // String | 
final String country = country_example; // String | 

try {
    final response = api.onRamperGetQuotesBuy(authorization, fiat, crypto, amount, paymentMethod, uuid, clientName, country);
    print(response);
} catch on DioException (e) {
    print('Exception when calling OnramperApi->onRamperGetQuotesBuy: $e\n');
}
```

#### Parameters

| Name              | Type       | Description | Notes                                  |
| ----------------- | ---------- | ----------- | -------------------------------------- |
| **authorization** | **String** |             |                                        |
| **fiat**          | **String** |             |                                        |
| **crypto**        | **String** |             |                                        |
| **amount**        | **double** |             |                                        |
| **paymentMethod** | **String** |             | \[optional] \[default to 'creditcard'] |
| **uuid**          | **String** |             | \[optional] \[default to '']           |
| **clientName**    | **String** |             | \[optional] \[default to '']           |
| **country**       | **String** |             | \[optional] \[default to '']           |

#### Return type

[**BuiltList\<Quote>**](quote.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: Not defined
* **Accept**: application/json

[\[Back to top\]](onramperapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## **onRamperGetQuotesSell**

> BuiltList onRamperGetQuotesSell(authorization, fiat, crypto, amount, paymentMethod, uuid, clientName, country)

#### Example

```dart
import 'package:moonsdk/api.dart';
// TODO Configure API key authorization: ApiKeyAuth
//defaultApiClient.getAuthentication<ApiKeyAuth>('ApiKeyAuth').apiKey = 'YOUR_API_KEY';
// uncomment below to setup prefix (e.g. Bearer) for API key, if needed
//defaultApiClient.getAuthentication<ApiKeyAuth>('ApiKeyAuth').apiKeyPrefix = 'Bearer';
// TODO Configure API key authorization: BearerAuth
//defaultApiClient.getAuthentication<ApiKeyAuth>('BearerAuth').apiKey = 'YOUR_API_KEY';
// uncomment below to setup prefix (e.g. Bearer) for API key, if needed
//defaultApiClient.getAuthentication<ApiKeyAuth>('BearerAuth').apiKeyPrefix = 'Bearer';

final api = Moonsdk().getOnramperApi();
final String authorization = authorization_example; // String | 
final String fiat = fiat_example; // String | 
final String crypto = crypto_example; // String | 
final double amount = 1.2; // double | 
final String paymentMethod = paymentMethod_example; // String | 
final String uuid = uuid_example; // String | 
final String clientName = clientName_example; // String | 
final String country = country_example; // String | 

try {
    final response = api.onRamperGetQuotesSell(authorization, fiat, crypto, amount, paymentMethod, uuid, clientName, country);
    print(response);
} catch on DioException (e) {
    print('Exception when calling OnramperApi->onRamperGetQuotesSell: $e\n');
}
```

#### Parameters

| Name              | Type       | Description | Notes                                  |
| ----------------- | ---------- | ----------- | -------------------------------------- |
| **authorization** | **String** |             |                                        |
| **fiat**          | **String** |             |                                        |
| **crypto**        | **String** |             |                                        |
| **amount**        | **double** |             |                                        |
| **paymentMethod** | **String** |             | \[optional] \[default to 'creditcard'] |
| **uuid**          | **String** |             | \[optional] \[default to '']           |
| **clientName**    | **String** |             | \[optional] \[default to '']           |
| **country**       | **String** |             | \[optional] \[default to '']           |

#### Return type

[**BuiltList\<SellQuote>**](sellquote.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: Not defined
* **Accept**: application/json

[\[Back to top\]](onramperapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## **onRamperGetSupportedAssets**

> SupportedAssetResponse onRamperGetSupportedAssets(authorization, source\_, country)

#### Example

```dart
import 'package:moonsdk/api.dart';
// TODO Configure API key authorization: ApiKeyAuth
//defaultApiClient.getAuthentication<ApiKeyAuth>('ApiKeyAuth').apiKey = 'YOUR_API_KEY';
// uncomment below to setup prefix (e.g. Bearer) for API key, if needed
//defaultApiClient.getAuthentication<ApiKeyAuth>('ApiKeyAuth').apiKeyPrefix = 'Bearer';
// TODO Configure API key authorization: BearerAuth
//defaultApiClient.getAuthentication<ApiKeyAuth>('BearerAuth').apiKey = 'YOUR_API_KEY';
// uncomment below to setup prefix (e.g. Bearer) for API key, if needed
//defaultApiClient.getAuthentication<ApiKeyAuth>('BearerAuth').apiKeyPrefix = 'Bearer';

final api = Moonsdk().getOnramperApi();
final String authorization = authorization_example; // String | 
final String source_ = source__example; // String | 
final String country = country_example; // String | 

try {
    final response = api.onRamperGetSupportedAssets(authorization, source_, country);
    print(response);
} catch on DioException (e) {
    print('Exception when calling OnramperApi->onRamperGetSupportedAssets: $e\n');
}
```

#### Parameters

| Name              | Type       | Description | Notes |
| ----------------- | ---------- | ----------- | ----- |
| **authorization** | **String** |             |       |
| **source\_**      | **String** |             |       |
| **country**       | **String** |             |       |

#### Return type

[**SupportedAssetResponse**](supportedassetresponse.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: Not defined
* **Accept**: application/json

[\[Back to top\]](onramperapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## **onRamperGetSupportedCurrencies**

> SupportedCurrenciesResponse onRamperGetSupportedCurrencies(authorization, type)

#### Example

```dart
import 'package:moonsdk/api.dart';
// TODO Configure API key authorization: ApiKeyAuth
//defaultApiClient.getAuthentication<ApiKeyAuth>('ApiKeyAuth').apiKey = 'YOUR_API_KEY';
// uncomment below to setup prefix (e.g. Bearer) for API key, if needed
//defaultApiClient.getAuthentication<ApiKeyAuth>('ApiKeyAuth').apiKeyPrefix = 'Bearer';
// TODO Configure API key authorization: BearerAuth
//defaultApiClient.getAuthentication<ApiKeyAuth>('BearerAuth').apiKey = 'YOUR_API_KEY';
// uncomment below to setup prefix (e.g. Bearer) for API key, if needed
//defaultApiClient.getAuthentication<ApiKeyAuth>('BearerAuth').apiKeyPrefix = 'Bearer';

final api = Moonsdk().getOnramperApi();
final String authorization = authorization_example; // String | 
final String type = type_example; // String | 

try {
    final response = api.onRamperGetSupportedCurrencies(authorization, type);
    print(response);
} catch on DioException (e) {
    print('Exception when calling OnramperApi->onRamperGetSupportedCurrencies: $e\n');
}
```

#### Parameters

| Name              | Type       | Description | Notes |
| ----------------- | ---------- | ----------- | ----- |
| **authorization** | **String** |             |       |
| **type**          | **String** |             |       |

#### Return type

[**SupportedCurrenciesResponse**](supportedcurrenciesresponse.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: Not defined
* **Accept**: application/json

[\[Back to top\]](onramperapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## **onRamperGetSupportedDefaultsAll**

> SupportedDefaultResponse onRamperGetSupportedDefaultsAll(authorization, country, type)

#### Example

```dart
import 'package:moonsdk/api.dart';
// TODO Configure API key authorization: ApiKeyAuth
//defaultApiClient.getAuthentication<ApiKeyAuth>('ApiKeyAuth').apiKey = 'YOUR_API_KEY';
// uncomment below to setup prefix (e.g. Bearer) for API key, if needed
//defaultApiClient.getAuthentication<ApiKeyAuth>('ApiKeyAuth').apiKeyPrefix = 'Bearer';
// TODO Configure API key authorization: BearerAuth
//defaultApiClient.getAuthentication<ApiKeyAuth>('BearerAuth').apiKey = 'YOUR_API_KEY';
// uncomment below to setup prefix (e.g. Bearer) for API key, if needed
//defaultApiClient.getAuthentication<ApiKeyAuth>('BearerAuth').apiKeyPrefix = 'Bearer';

final api = Moonsdk().getOnramperApi();
final String authorization = authorization_example; // String | 
final String country = country_example; // String | 
final String type = type_example; // String | 

try {
    final response = api.onRamperGetSupportedDefaultsAll(authorization, country, type);
    print(response);
} catch on DioException (e) {
    print('Exception when calling OnramperApi->onRamperGetSupportedDefaultsAll: $e\n');
}
```

#### Parameters

| Name              | Type       | Description | Notes |
| ----------------- | ---------- | ----------- | ----- |
| **authorization** | **String** |             |       |
| **country**       | **String** |             |       |
| **type**          | **String** |             |       |

#### Return type

[**SupportedDefaultResponse**](supporteddefaultresponse.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: Not defined
* **Accept**: application/json

[\[Back to top\]](onramperapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## **onRamperGetSupportedOnRampsAll**

> GetSupportedOnRampsResponse onRamperGetSupportedOnRampsAll(authorization)

#### Example

```dart
import 'package:moonsdk/api.dart';
// TODO Configure API key authorization: ApiKeyAuth
//defaultApiClient.getAuthentication<ApiKeyAuth>('ApiKeyAuth').apiKey = 'YOUR_API_KEY';
// uncomment below to setup prefix (e.g. Bearer) for API key, if needed
//defaultApiClient.getAuthentication<ApiKeyAuth>('ApiKeyAuth').apiKeyPrefix = 'Bearer';
// TODO Configure API key authorization: BearerAuth
//defaultApiClient.getAuthentication<ApiKeyAuth>('BearerAuth').apiKey = 'YOUR_API_KEY';
// uncomment below to setup prefix (e.g. Bearer) for API key, if needed
//defaultApiClient.getAuthentication<ApiKeyAuth>('BearerAuth').apiKeyPrefix = 'Bearer';

final api = Moonsdk().getOnramperApi();
final String authorization = authorization_example; // String | 

try {
    final response = api.onRamperGetSupportedOnRampsAll(authorization);
    print(response);
} catch on DioException (e) {
    print('Exception when calling OnramperApi->onRamperGetSupportedOnRampsAll: $e\n');
}
```

#### Parameters

| Name              | Type       | Description | Notes |
| ----------------- | ---------- | ----------- | ----- |
| **authorization** | **String** |             |       |

#### Return type

[**GetSupportedOnRampsResponse**](getsupportedonrampsresponse.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: Not defined
* **Accept**: application/json

[\[Back to top\]](onramperapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## **onRamperGetSupportedPaymentTypes**

> SupportedPaymentTypesCurrencyResponse onRamperGetSupportedPaymentTypes(authorization, fiat, country, type)

#### Example

```dart
import 'package:moonsdk/api.dart';
// TODO Configure API key authorization: ApiKeyAuth
//defaultApiClient.getAuthentication<ApiKeyAuth>('ApiKeyAuth').apiKey = 'YOUR_API_KEY';
// uncomment below to setup prefix (e.g. Bearer) for API key, if needed
//defaultApiClient.getAuthentication<ApiKeyAuth>('ApiKeyAuth').apiKeyPrefix = 'Bearer';
// TODO Configure API key authorization: BearerAuth
//defaultApiClient.getAuthentication<ApiKeyAuth>('BearerAuth').apiKey = 'YOUR_API_KEY';
// uncomment below to setup prefix (e.g. Bearer) for API key, if needed
//defaultApiClient.getAuthentication<ApiKeyAuth>('BearerAuth').apiKeyPrefix = 'Bearer';

final api = Moonsdk().getOnramperApi();
final String authorization = authorization_example; // String | 
final String fiat = fiat_example; // String | 
final String country = country_example; // String | 
final String type = type_example; // String | 

try {
    final response = api.onRamperGetSupportedPaymentTypes(authorization, fiat, country, type);
    print(response);
} catch on DioException (e) {
    print('Exception when calling OnramperApi->onRamperGetSupportedPaymentTypes: $e\n');
}
```

#### Parameters

| Name              | Type       | Description | Notes |
| ----------------- | ---------- | ----------- | ----- |
| **authorization** | **String** |             |       |
| **fiat**          | **String** |             |       |
| **country**       | **String** |             |       |
| **type**          | **String** |             |       |

#### Return type

[**SupportedPaymentTypesCurrencyResponse**](supportedpaymenttypescurrencyresponse.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: Not defined
* **Accept**: application/json

[\[Back to top\]](onramperapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## **onRamperGetSupportedPaymentTypesFiat**

> SupportedPaymentTypesCurrencyResponse onRamperGetSupportedPaymentTypesFiat(authorization, fiat, country)

#### Example

```dart
import 'package:moonsdk/api.dart';
// TODO Configure API key authorization: ApiKeyAuth
//defaultApiClient.getAuthentication<ApiKeyAuth>('ApiKeyAuth').apiKey = 'YOUR_API_KEY';
// uncomment below to setup prefix (e.g. Bearer) for API key, if needed
//defaultApiClient.getAuthentication<ApiKeyAuth>('ApiKeyAuth').apiKeyPrefix = 'Bearer';
// TODO Configure API key authorization: BearerAuth
//defaultApiClient.getAuthentication<ApiKeyAuth>('BearerAuth').apiKey = 'YOUR_API_KEY';
// uncomment below to setup prefix (e.g. Bearer) for API key, if needed
//defaultApiClient.getAuthentication<ApiKeyAuth>('BearerAuth').apiKeyPrefix = 'Bearer';

final api = Moonsdk().getOnramperApi();
final String authorization = authorization_example; // String | 
final String fiat = fiat_example; // String | 
final String country = country_example; // String | 

try {
    final response = api.onRamperGetSupportedPaymentTypesFiat(authorization, fiat, country);
    print(response);
} catch on DioException (e) {
    print('Exception when calling OnramperApi->onRamperGetSupportedPaymentTypesFiat: $e\n');
}
```

#### Parameters

| Name              | Type       | Description | Notes |
| ----------------- | ---------- | ----------- | ----- |
| **authorization** | **String** |             |       |
| **fiat**          | **String** |             |       |
| **country**       | **String** |             |       |

#### Return type

[**SupportedPaymentTypesCurrencyResponse**](supportedpaymenttypescurrencyresponse.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: Not defined
* **Accept**: application/json

[\[Back to top\]](onramperapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)
