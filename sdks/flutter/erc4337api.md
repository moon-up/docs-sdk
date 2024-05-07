# Erc4337Api

## openapi.api.Erc4337Api

### Load the API package

```dart
import 'package:openapi/api.dart';
```

All URIs are relative to _https://vault-api.usemoon.ai_

| Method                                                           | HTTP request                                             | Description |
| ---------------------------------------------------------------- | -------------------------------------------------------- | ----------- |
| [**getAddress**](erc4337api.md#getaddress)                       | **POST** /erc4337/{accountName}/address                  |             |
| [**signBroadcastUserOpTx**](erc4337api.md#signbroadcastuseroptx) | **POST** /erc4337/{accountName}/sign-broadcast-userop-tx |             |

## **getAddress**

> AccountControllerResponse getAddress(authorization, accountName, inputBody)

#### Example

```dart
import 'package:openapi/api.dart';
// TODO Configure API key authorization: ApiKeyAuth
//defaultApiClient.getAuthentication<ApiKeyAuth>('ApiKeyAuth').apiKey = 'YOUR_API_KEY';
// uncomment below to setup prefix (e.g. Bearer) for API key, if needed
//defaultApiClient.getAuthentication<ApiKeyAuth>('ApiKeyAuth').apiKeyPrefix = 'Bearer';
// TODO Configure API key authorization: BearerAuth
//defaultApiClient.getAuthentication<ApiKeyAuth>('BearerAuth').apiKey = 'YOUR_API_KEY';
// uncomment below to setup prefix (e.g. Bearer) for API key, if needed
//defaultApiClient.getAuthentication<ApiKeyAuth>('BearerAuth').apiKeyPrefix = 'Bearer';

final api = Openapi().getErc4337Api();
final String authorization = authorization_example; // String | 
final String accountName = accountName_example; // String | 
final InputBody inputBody = ; // InputBody | 

try {
    final response = api.getAddress(authorization, accountName, inputBody);
    print(response);
} catch on DioException (e) {
    print('Exception when calling Erc4337Api->getAddress: $e\n');
}
```

#### Parameters

| Name              | Type                          | Description | Notes |
| ----------------- | ----------------------------- | ----------- | ----- |
| **authorization** | **String**                    |             |       |
| **accountName**   | **String**                    |             |       |
| **inputBody**     | [**InputBody**](inputbody.md) |             |       |

#### Return type

[**AccountControllerResponse**](accountcontrollerresponse.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](erc4337api.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## **signBroadcastUserOpTx**

> AccountControllerResponse signBroadcastUserOpTx(authorization, accountName, inputBody)

#### Example

```dart
import 'package:openapi/api.dart';
// TODO Configure API key authorization: ApiKeyAuth
//defaultApiClient.getAuthentication<ApiKeyAuth>('ApiKeyAuth').apiKey = 'YOUR_API_KEY';
// uncomment below to setup prefix (e.g. Bearer) for API key, if needed
//defaultApiClient.getAuthentication<ApiKeyAuth>('ApiKeyAuth').apiKeyPrefix = 'Bearer';
// TODO Configure API key authorization: BearerAuth
//defaultApiClient.getAuthentication<ApiKeyAuth>('BearerAuth').apiKey = 'YOUR_API_KEY';
// uncomment below to setup prefix (e.g. Bearer) for API key, if needed
//defaultApiClient.getAuthentication<ApiKeyAuth>('BearerAuth').apiKeyPrefix = 'Bearer';

final api = Openapi().getErc4337Api();
final String authorization = authorization_example; // String | 
final String accountName = accountName_example; // String | 
final InputBody inputBody = ; // InputBody | 

try {
    final response = api.signBroadcastUserOpTx(authorization, accountName, inputBody);
    print(response);
} catch on DioException (e) {
    print('Exception when calling Erc4337Api->signBroadcastUserOpTx: $e\n');
}
```

#### Parameters

| Name              | Type                          | Description | Notes |
| ----------------- | ----------------------------- | ----------- | ----- |
| **authorization** | **String**                    |             |       |
| **accountName**   | **String**                    |             |       |
| **inputBody**     | [**InputBody**](inputbody.md) |             |       |

#### Return type

[**AccountControllerResponse**](accountcontrollerresponse.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](erc4337api.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)
