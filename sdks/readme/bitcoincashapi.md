# BitcoincashApi

## moonsdk.api.BitcoincashApi

### Load the API package

```dart
import 'package:moonsdk/api.dart';
```

All URIs are relative to _https://beta.usemoon.ai_

| Method                                                                         | HTTP request                                | Description |
| ------------------------------------------------------------------------------ | ------------------------------------------- | ----------- |
| [**createBitcoinCashAccount**](bitcoincashapi.md#createbitcoincashaccount)     | **POST** /bitcoincash                       |             |
| [**getBitcoinCashAccount**](bitcoincashapi.md#getbitcoincashaccount)           | **GET** /bitcoincash/{accountName}          |             |
| [**listBitcoinCashAccounts**](bitcoincashapi.md#listbitcoincashaccounts)       | **GET** /bitcoincash                        |             |
| [**signBitcoinCashTransaction**](bitcoincashapi.md#signbitcoincashtransaction) | **POST** /bitcoincash/{accountName}/sign-tx |             |

## **createBitcoinCashAccount**

> AccountAPIResponse createBitcoinCashAccount(authorization, bitcoinCashInput)

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

final api = Moonsdk().getBitcoincashApi();
final String authorization = authorization_example; // String | 
final BitcoinCashInput bitcoinCashInput = ; // BitcoinCashInput | 

try {
    final response = api.createBitcoinCashAccount(authorization, bitcoinCashInput);
    print(response);
} catch on DioException (e) {
    print('Exception when calling BitcoincashApi->createBitcoinCashAccount: $e\n');
}
```

#### Parameters

| Name                 | Type                                        | Description | Notes |
| -------------------- | ------------------------------------------- | ----------- | ----- |
| **authorization**    | **String**                                  |             |       |
| **bitcoinCashInput** | [**BitcoinCashInput**](bitcoincashinput.md) |             |       |

#### Return type

[**AccountAPIResponse**](accountapiresponse.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](bitcoincashapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## **getBitcoinCashAccount**

> AccountAPIResponse getBitcoinCashAccount(authorization, accountName)

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

final api = Moonsdk().getBitcoincashApi();
final String authorization = authorization_example; // String | 
final String accountName = accountName_example; // String | 

try {
    final response = api.getBitcoinCashAccount(authorization, accountName);
    print(response);
} catch on DioException (e) {
    print('Exception when calling BitcoincashApi->getBitcoinCashAccount: $e\n');
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

[\[Back to top\]](bitcoincashapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## **listBitcoinCashAccounts**

> AccountAPIResponse listBitcoinCashAccounts(authorization)

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

final api = Moonsdk().getBitcoincashApi();
final String authorization = authorization_example; // String | 

try {
    final response = api.listBitcoinCashAccounts(authorization);
    print(response);
} catch on DioException (e) {
    print('Exception when calling BitcoincashApi->listBitcoinCashAccounts: $e\n');
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

[\[Back to top\]](bitcoincashapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## **signBitcoinCashTransaction**

> BitcoinCashAPIResponse signBitcoinCashTransaction(authorization, accountName, bitcoinCashTransactionInput)

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

final api = Moonsdk().getBitcoincashApi();
final String authorization = authorization_example; // String | 
final String accountName = accountName_example; // String | 
final BitcoinCashTransactionInput bitcoinCashTransactionInput = ; // BitcoinCashTransactionInput | 

try {
    final response = api.signBitcoinCashTransaction(authorization, accountName, bitcoinCashTransactionInput);
    print(response);
} catch on DioException (e) {
    print('Exception when calling BitcoincashApi->signBitcoinCashTransaction: $e\n');
}
```

#### Parameters

| Name                            | Type                                                              | Description | Notes |
| ------------------------------- | ----------------------------------------------------------------- | ----------- | ----- |
| **authorization**               | **String**                                                        |             |       |
| **accountName**                 | **String**                                                        |             |       |
| **bitcoinCashTransactionInput** | [**BitcoinCashTransactionInput**](bitcoincashtransactioninput.md) |             |       |

#### Return type

[**BitcoinCashAPIResponse**](bitcoincashapiresponse.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](bitcoincashapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)
