# BitcoinApi

## moonsdk.api.BitcoinApi

### Load the API package

```dart
import 'package:moonsdk/api.dart';
```

All URIs are relative to _https://beta.usemoon.ai_

| Method                                                             | HTTP request                            | Description |
| ------------------------------------------------------------------ | --------------------------------------- | ----------- |
| [**createBitcoinAccount**](bitcoinapi.md#createbitcoinaccount)     | **POST** /bitcoin                       |             |
| [**getBitcoinAccount**](bitcoinapi.md#getbitcoinaccount)           | **GET** /bitcoin/{accountName}          |             |
| [**listBitcoinAccounts**](bitcoinapi.md#listbitcoinaccounts)       | **GET** /bitcoin                        |             |
| [**signBitcoinTransaction**](bitcoinapi.md#signbitcointransaction) | **POST** /bitcoin/{accountName}/sign-tx |             |

## **createBitcoinAccount**

> AccountAPIResponse createBitcoinAccount(authorization, bitcoinInput)

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

final api = Moonsdk().getBitcoinApi();
final String authorization = authorization_example; // String | 
final BitcoinInput bitcoinInput = ; // BitcoinInput | 

try {
    final response = api.createBitcoinAccount(authorization, bitcoinInput);
    print(response);
} catch on DioException (e) {
    print('Exception when calling BitcoinApi->createBitcoinAccount: $e\n');
}
```

#### Parameters

| Name              | Type                                | Description | Notes |
| ----------------- | ----------------------------------- | ----------- | ----- |
| **authorization** | **String**                          |             |       |
| **bitcoinInput**  | [**BitcoinInput**](bitcoininput.md) |             |       |

#### Return type

[**AccountAPIResponse**](accountapiresponse.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](bitcoinapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## **getBitcoinAccount**

> AccountAPIResponse getBitcoinAccount(authorization, accountName)

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

final api = Moonsdk().getBitcoinApi();
final String authorization = authorization_example; // String | 
final String accountName = accountName_example; // String | 

try {
    final response = api.getBitcoinAccount(authorization, accountName);
    print(response);
} catch on DioException (e) {
    print('Exception when calling BitcoinApi->getBitcoinAccount: $e\n');
}
```

#### Parameters

| Name              | Type       | Description | Notes |
| ----------------- | ---------- | ----------- | ----- |
| **authorization** | **String** |             |       |
| **accountName**   | **String** |             |       |

#### Return type

[**AccountAPIResponse**](accountapiresponse.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: Not defined
* **Accept**: application/json

[\[Back to top\]](bitcoinapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## **listBitcoinAccounts**

> AccountAPIResponse listBitcoinAccounts(authorization)

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

final api = Moonsdk().getBitcoinApi();
final String authorization = authorization_example; // String | 

try {
    final response = api.listBitcoinAccounts(authorization);
    print(response);
} catch on DioException (e) {
    print('Exception when calling BitcoinApi->listBitcoinAccounts: $e\n');
}
```

#### Parameters

| Name              | Type       | Description | Notes |
| ----------------- | ---------- | ----------- | ----- |
| **authorization** | **String** |             |       |

#### Return type

[**AccountAPIResponse**](accountapiresponse.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: Not defined
* **Accept**: application/json

[\[Back to top\]](bitcoinapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## **signBitcoinTransaction**

> BitcoinAPIResponse signBitcoinTransaction(authorization, accountName, bitcoinTransactionInput)

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

final api = Moonsdk().getBitcoinApi();
final String authorization = authorization_example; // String | 
final String accountName = accountName_example; // String | 
final BitcoinTransactionInput bitcoinTransactionInput = ; // BitcoinTransactionInput | 

try {
    final response = api.signBitcoinTransaction(authorization, accountName, bitcoinTransactionInput);
    print(response);
} catch on DioException (e) {
    print('Exception when calling BitcoinApi->signBitcoinTransaction: $e\n');
}
```

#### Parameters

| Name                        | Type                                                      | Description | Notes |
| --------------------------- | --------------------------------------------------------- | ----------- | ----- |
| **authorization**           | **String**                                                |             |       |
| **accountName**             | **String**                                                |             |       |
| **bitcoinTransactionInput** | [**BitcoinTransactionInput**](bitcointransactioninput.md) |             |       |

#### Return type

[**BitcoinAPIResponse**](bitcoinapiresponse.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](bitcoinapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)
