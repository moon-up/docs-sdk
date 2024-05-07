# Erc721Api

## moonsdk.api.Erc721Api

### Load the API package

```dart
import 'package:moonsdk/api.dart';
```

All URIs are relative to _https://beta.usemoon.ai_

| Method                                                  | HTTP request                                 | Description |
| ------------------------------------------------------- | -------------------------------------------- | ----------- |
| [**approve**](erc721api.md#approve)                     | **POST** /erc721/{name}/approve              |             |
| [**balanceOf**](erc721api.md#balanceof)                 | **POST** /erc721/{name}/balance-of           |             |
| [**getApproved**](erc721api.md#getapproved)             | **POST** /erc721/{name}/get-approved         |             |
| [**isApprovedForAll**](erc721api.md#isapprovedforall)   | **POST** /erc721/{name}/is-approved-for-all  |             |
| [**name**](erc721api.md#name)                           | **POST** /erc721/{name}/name                 |             |
| [**ownerOf**](erc721api.md#ownerof)                     | **POST** /erc721/{name}/owner-of             |             |
| [**safeTransferFrom**](erc721api.md#safetransferfrom)   | **POST** /erc721/{name}/safe-transfer-from   |             |
| [**setApprovalForAll**](erc721api.md#setapprovalforall) | **POST** /erc721/{name}/set-approval-for-all |             |
| [**symbol**](erc721api.md#symbol)                       | **POST** /erc721/{name}/symbol               |             |
| [**tokenUri**](erc721api.md#tokenuri)                   | **POST** /erc721/{name}/token-uri            |             |
| [**transfer**](erc721api.md#transfer)                   | **POST** /erc721/{name}/transfer             |             |
| [**transferFrom**](erc721api.md#transferfrom)           | **POST** /erc721/{name}/transfer-from        |             |

## **approve**

> TransactionAPIResponse approve(authorization, name, erc721Request)

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

final api = Moonsdk().getErc721Api();
final String authorization = authorization_example; // String | 
final String name = name_example; // String | 
final Erc721Request erc721Request = ; // Erc721Request | 

try {
    final response = api.approve(authorization, name, erc721Request);
    print(response);
} catch on DioException (e) {
    print('Exception when calling Erc721Api->approve: $e\n');
}
```

#### Parameters

| Name              | Type                                  | Description | Notes |
| ----------------- | ------------------------------------- | ----------- | ----- |
| **authorization** | **String**                            |             |       |
| **name**          | **String**                            |             |       |
| **erc721Request** | [**Erc721Request**](erc721request.md) |             |       |

#### Return type

[**TransactionAPIResponse**](transactionapiresponse.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](erc721api.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## **balanceOf**

> TransactionAPIResponse balanceOf(authorization, name, erc721Request)

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

final api = Moonsdk().getErc721Api();
final String authorization = authorization_example; // String | 
final String name = name_example; // String | 
final Erc721Request erc721Request = ; // Erc721Request | 

try {
    final response = api.balanceOf(authorization, name, erc721Request);
    print(response);
} catch on DioException (e) {
    print('Exception when calling Erc721Api->balanceOf: $e\n');
}
```

#### Parameters

| Name              | Type                                  | Description | Notes |
| ----------------- | ------------------------------------- | ----------- | ----- |
| **authorization** | **String**                            |             |       |
| **name**          | **String**                            |             |       |
| **erc721Request** | [**Erc721Request**](erc721request.md) |             |       |

#### Return type

[**TransactionAPIResponse**](transactionapiresponse.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](erc721api.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## **getApproved**

> TransactionAPIResponse getApproved(authorization, name, erc721Request)

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

final api = Moonsdk().getErc721Api();
final String authorization = authorization_example; // String | 
final String name = name_example; // String | 
final Erc721Request erc721Request = ; // Erc721Request | 

try {
    final response = api.getApproved(authorization, name, erc721Request);
    print(response);
} catch on DioException (e) {
    print('Exception when calling Erc721Api->getApproved: $e\n');
}
```

#### Parameters

| Name              | Type                                  | Description | Notes |
| ----------------- | ------------------------------------- | ----------- | ----- |
| **authorization** | **String**                            |             |       |
| **name**          | **String**                            |             |       |
| **erc721Request** | [**Erc721Request**](erc721request.md) |             |       |

#### Return type

[**TransactionAPIResponse**](transactionapiresponse.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](erc721api.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## **isApprovedForAll**

> TransactionAPIResponse isApprovedForAll(authorization, name, erc721Request)

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

final api = Moonsdk().getErc721Api();
final String authorization = authorization_example; // String | 
final String name = name_example; // String | 
final Erc721Request erc721Request = ; // Erc721Request | 

try {
    final response = api.isApprovedForAll(authorization, name, erc721Request);
    print(response);
} catch on DioException (e) {
    print('Exception when calling Erc721Api->isApprovedForAll: $e\n');
}
```

#### Parameters

| Name              | Type                                  | Description | Notes |
| ----------------- | ------------------------------------- | ----------- | ----- |
| **authorization** | **String**                            |             |       |
| **name**          | **String**                            |             |       |
| **erc721Request** | [**Erc721Request**](erc721request.md) |             |       |

#### Return type

[**TransactionAPIResponse**](transactionapiresponse.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](erc721api.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## **name**

> TransactionAPIResponse name(authorization, name, erc721Request)

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

final api = Moonsdk().getErc721Api();
final String authorization = authorization_example; // String | 
final String name = name_example; // String | 
final Erc721Request erc721Request = ; // Erc721Request | 

try {
    final response = api.name(authorization, name, erc721Request);
    print(response);
} catch on DioException (e) {
    print('Exception when calling Erc721Api->name: $e\n');
}
```

#### Parameters

| Name              | Type                                  | Description | Notes |
| ----------------- | ------------------------------------- | ----------- | ----- |
| **authorization** | **String**                            |             |       |
| **name**          | **String**                            |             |       |
| **erc721Request** | [**Erc721Request**](erc721request.md) |             |       |

#### Return type

[**TransactionAPIResponse**](transactionapiresponse.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](erc721api.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## **ownerOf**

> TransactionAPIResponse ownerOf(authorization, name, erc721Request)

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

final api = Moonsdk().getErc721Api();
final String authorization = authorization_example; // String | 
final String name = name_example; // String | 
final Erc721Request erc721Request = ; // Erc721Request | 

try {
    final response = api.ownerOf(authorization, name, erc721Request);
    print(response);
} catch on DioException (e) {
    print('Exception when calling Erc721Api->ownerOf: $e\n');
}
```

#### Parameters

| Name              | Type                                  | Description | Notes |
| ----------------- | ------------------------------------- | ----------- | ----- |
| **authorization** | **String**                            |             |       |
| **name**          | **String**                            |             |       |
| **erc721Request** | [**Erc721Request**](erc721request.md) |             |       |

#### Return type

[**TransactionAPIResponse**](transactionapiresponse.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](erc721api.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## **safeTransferFrom**

> TransactionAPIResponse safeTransferFrom(authorization, name, erc721Request)

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

final api = Moonsdk().getErc721Api();
final String authorization = authorization_example; // String | 
final String name = name_example; // String | 
final Erc721Request erc721Request = ; // Erc721Request | 

try {
    final response = api.safeTransferFrom(authorization, name, erc721Request);
    print(response);
} catch on DioException (e) {
    print('Exception when calling Erc721Api->safeTransferFrom: $e\n');
}
```

#### Parameters

| Name              | Type                                  | Description | Notes |
| ----------------- | ------------------------------------- | ----------- | ----- |
| **authorization** | **String**                            |             |       |
| **name**          | **String**                            |             |       |
| **erc721Request** | [**Erc721Request**](erc721request.md) |             |       |

#### Return type

[**TransactionAPIResponse**](transactionapiresponse.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](erc721api.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## **setApprovalForAll**

> TransactionAPIResponse setApprovalForAll(authorization, name, erc721Request)

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

final api = Moonsdk().getErc721Api();
final String authorization = authorization_example; // String | 
final String name = name_example; // String | 
final Erc721Request erc721Request = ; // Erc721Request | 

try {
    final response = api.setApprovalForAll(authorization, name, erc721Request);
    print(response);
} catch on DioException (e) {
    print('Exception when calling Erc721Api->setApprovalForAll: $e\n');
}
```

#### Parameters

| Name              | Type                                  | Description | Notes |
| ----------------- | ------------------------------------- | ----------- | ----- |
| **authorization** | **String**                            |             |       |
| **name**          | **String**                            |             |       |
| **erc721Request** | [**Erc721Request**](erc721request.md) |             |       |

#### Return type

[**TransactionAPIResponse**](transactionapiresponse.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](erc721api.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## **symbol**

> TransactionAPIResponse symbol(authorization, name, erc721Request)

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

final api = Moonsdk().getErc721Api();
final String authorization = authorization_example; // String | 
final String name = name_example; // String | 
final Erc721Request erc721Request = ; // Erc721Request | 

try {
    final response = api.symbol(authorization, name, erc721Request);
    print(response);
} catch on DioException (e) {
    print('Exception when calling Erc721Api->symbol: $e\n');
}
```

#### Parameters

| Name              | Type                                  | Description | Notes |
| ----------------- | ------------------------------------- | ----------- | ----- |
| **authorization** | **String**                            |             |       |
| **name**          | **String**                            |             |       |
| **erc721Request** | [**Erc721Request**](erc721request.md) |             |       |

#### Return type

[**TransactionAPIResponse**](transactionapiresponse.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](erc721api.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## **tokenUri**

> TransactionAPIResponse tokenUri(authorization, name, erc721Request)

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

final api = Moonsdk().getErc721Api();
final String authorization = authorization_example; // String | 
final String name = name_example; // String | 
final Erc721Request erc721Request = ; // Erc721Request | 

try {
    final response = api.tokenUri(authorization, name, erc721Request);
    print(response);
} catch on DioException (e) {
    print('Exception when calling Erc721Api->tokenUri: $e\n');
}
```

#### Parameters

| Name              | Type                                  | Description | Notes |
| ----------------- | ------------------------------------- | ----------- | ----- |
| **authorization** | **String**                            |             |       |
| **name**          | **String**                            |             |       |
| **erc721Request** | [**Erc721Request**](erc721request.md) |             |       |

#### Return type

[**TransactionAPIResponse**](transactionapiresponse.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](erc721api.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## **transfer**

> TransactionAPIResponse transfer(authorization, name, erc721Request)

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

final api = Moonsdk().getErc721Api();
final String authorization = authorization_example; // String | 
final String name = name_example; // String | 
final Erc721Request erc721Request = ; // Erc721Request | 

try {
    final response = api.transfer(authorization, name, erc721Request);
    print(response);
} catch on DioException (e) {
    print('Exception when calling Erc721Api->transfer: $e\n');
}
```

#### Parameters

| Name              | Type                                  | Description | Notes |
| ----------------- | ------------------------------------- | ----------- | ----- |
| **authorization** | **String**                            |             |       |
| **name**          | **String**                            |             |       |
| **erc721Request** | [**Erc721Request**](erc721request.md) |             |       |

#### Return type

[**TransactionAPIResponse**](transactionapiresponse.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](erc721api.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## **transferFrom**

> TransactionAPIResponse transferFrom(authorization, name, erc721Request)

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

final api = Moonsdk().getErc721Api();
final String authorization = authorization_example; // String | 
final String name = name_example; // String | 
final Erc721Request erc721Request = ; // Erc721Request | 

try {
    final response = api.transferFrom(authorization, name, erc721Request);
    print(response);
} catch on DioException (e) {
    print('Exception when calling Erc721Api->transferFrom: $e\n');
}
```

#### Parameters

| Name              | Type                                  | Description | Notes |
| ----------------- | ------------------------------------- | ----------- | ----- |
| **authorization** | **String**                            |             |       |
| **name**          | **String**                            |             |       |
| **erc721Request** | [**Erc721Request**](erc721request.md) |             |       |

#### Return type

[**TransactionAPIResponse**](transactionapiresponse.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](erc721api.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)
