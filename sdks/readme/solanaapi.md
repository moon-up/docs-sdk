# SolanaApi

## moonsdk.api.SolanaApi

### Load the API package

```dart
import 'package:moonsdk/api.dart';
```

All URIs are relative to _https://beta.usemoon.ai_

| Method                                                          | HTTP request                           | Description |
| --------------------------------------------------------------- | -------------------------------------- | ----------- |
| [**createSolanaAccount**](solanaapi.md#createsolanaaccount)     | **POST** /solana                       |             |
| [**getSolanaAccount**](solanaapi.md#getsolanaaccount)           | **GET** /solana/{accountName}          |             |
| [**listSolanaAccounts**](solanaapi.md#listsolanaaccounts)       | **GET** /solana                        |             |
| [**signSolanaTransaction**](solanaapi.md#signsolanatransaction) | **POST** /solana/{accountName}/sign-tx |             |

## **createSolanaAccount**

> AccountAPIResponse createSolanaAccount(authorization, solanaInput)

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

final api = Moonsdk().getSolanaApi();
final String authorization = authorization_example; // String | 
final SolanaInput solanaInput = ; // SolanaInput | 

try {
    final response = api.createSolanaAccount(authorization, solanaInput);
    print(response);
} catch on DioException (e) {
    print('Exception when calling SolanaApi->createSolanaAccount: $e\n');
}
```

#### Parameters

| Name              | Type                              | Description | Notes |
| ----------------- | --------------------------------- | ----------- | ----- |
| **authorization** | **String**                        |             |       |
| **solanaInput**   | [**SolanaInput**](solanainput.md) |             |       |

#### Return type

[**AccountAPIResponse**](accountapiresponse.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](solanaapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## **getSolanaAccount**

> AccountAPIResponse getSolanaAccount(authorization, accountName)

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

final api = Moonsdk().getSolanaApi();
final String authorization = authorization_example; // String | 
final String accountName = accountName_example; // String | 

try {
    final response = api.getSolanaAccount(authorization, accountName);
    print(response);
} catch on DioException (e) {
    print('Exception when calling SolanaApi->getSolanaAccount: $e\n');
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

[\[Back to top\]](solanaapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## **listSolanaAccounts**

> AccountAPIResponse listSolanaAccounts(authorization)

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

final api = Moonsdk().getSolanaApi();
final String authorization = authorization_example; // String | 

try {
    final response = api.listSolanaAccounts(authorization);
    print(response);
} catch on DioException (e) {
    print('Exception when calling SolanaApi->listSolanaAccounts: $e\n');
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

[\[Back to top\]](solanaapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## **signSolanaTransaction**

> SolanaAPIResponse signSolanaTransaction(authorization, accountName, solanaTransactionInput)

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

final api = Moonsdk().getSolanaApi();
final String authorization = authorization_example; // String | 
final String accountName = accountName_example; // String | 
final SolanaTransactionInput solanaTransactionInput = ; // SolanaTransactionInput | 

try {
    final response = api.signSolanaTransaction(authorization, accountName, solanaTransactionInput);
    print(response);
} catch on DioException (e) {
    print('Exception when calling SolanaApi->signSolanaTransaction: $e\n');
}
```

#### Parameters

| Name                       | Type                                                    | Description | Notes |
| -------------------------- | ------------------------------------------------------- | ----------- | ----- |
| **authorization**          | **String**                                              |             |       |
| **accountName**            | **String**                                              |             |       |
| **solanaTransactionInput** | [**SolanaTransactionInput**](solanatransactioninput.md) |             |       |

#### Return type

[**SolanaAPIResponse**](solanaapiresponse.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](solanaapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)
