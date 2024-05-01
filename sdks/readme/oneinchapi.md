# OneinchApi

## moonsdk.api.OneinchApi

### Load the API package

```dart
import 'package:moonsdk/api.dart';
```

All URIs are relative to _https://beta.usemoon.ai_

| Method                                               | HTTP request                         | Description |
| ---------------------------------------------------- | ------------------------------------ | ----------- |
| [**approveCallData**](oneinchapi.md#approvecalldata) | **POST** /oneinch/approve-call-data  |             |
| [**approveSpender**](oneinchapi.md#approvespender)   | **POST** /oneinch/approve-spender    |             |
| [**protocols**](oneinchapi.md#protocols)             | **POST** /oneinch/protocols          |             |
| [**quote**](oneinchapi.md#quote)                     | **POST** /oneinch/quote              |             |
| [**swap**](oneinchapi.md#swap)                       | **POST** /oneinch/{accountName}/swap |             |
| [**tokens**](oneinchapi.md#tokens)                   | **POST** /oneinch/tokens             |             |

## **approveCallData**

> JsonObject approveCallData(body)

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

final api = Moonsdk().getOneinchApi();
final JsonObject body = ; // JsonObject | 

try {
    final response = api.approveCallData(body);
    print(response);
} catch on DioException (e) {
    print('Exception when calling OneinchApi->approveCallData: $e\n');
}
```

#### Parameters

| Name     | Type           | Description | Notes |
| -------- | -------------- | ----------- | ----- |
| **body** | **JsonObject** |             |       |

#### Return type

[**JsonObject**](../../dart/doc/JsonObject.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](oneinchapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## **approveSpender**

> JsonObject approveSpender(body)

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

final api = Moonsdk().getOneinchApi();
final JsonObject body = ; // JsonObject | 

try {
    final response = api.approveSpender(body);
    print(response);
} catch on DioException (e) {
    print('Exception when calling OneinchApi->approveSpender: $e\n');
}
```

#### Parameters

| Name     | Type           | Description | Notes |
| -------- | -------------- | ----------- | ----- |
| **body** | **JsonObject** |             |       |

#### Return type

[**JsonObject**](../../dart/doc/JsonObject.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](oneinchapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## **protocols**

> JsonObject protocols(body)

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

final api = Moonsdk().getOneinchApi();
final JsonObject body = ; // JsonObject | 

try {
    final response = api.protocols(body);
    print(response);
} catch on DioException (e) {
    print('Exception when calling OneinchApi->protocols: $e\n');
}
```

#### Parameters

| Name     | Type           | Description | Notes |
| -------- | -------------- | ----------- | ----- |
| **body** | **JsonObject** |             |       |

#### Return type

[**JsonObject**](../../dart/doc/JsonObject.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](oneinchapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## **quote**

> JsonObject quote(body)

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

final api = Moonsdk().getOneinchApi();
final JsonObject body = ; // JsonObject | 

try {
    final response = api.quote(body);
    print(response);
} catch on DioException (e) {
    print('Exception when calling OneinchApi->quote: $e\n');
}
```

#### Parameters

| Name     | Type           | Description | Notes |
| -------- | -------------- | ----------- | ----- |
| **body** | **JsonObject** |             |       |

#### Return type

[**JsonObject**](../../dart/doc/JsonObject.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](oneinchapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## **swap**

> JsonObject swap(accountName, authorization, getSwapDto)

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

final api = Moonsdk().getOneinchApi();
final String accountName = accountName_example; // String | 
final String authorization = authorization_example; // String | 
final GetSwapDto getSwapDto = ; // GetSwapDto | 

try {
    final response = api.swap(accountName, authorization, getSwapDto);
    print(response);
} catch on DioException (e) {
    print('Exception when calling OneinchApi->swap: $e\n');
}
```

#### Parameters

| Name              | Type                            | Description | Notes |
| ----------------- | ------------------------------- | ----------- | ----- |
| **accountName**   | **String**                      |             |       |
| **authorization** | **String**                      |             |       |
| **getSwapDto**    | [**GetSwapDto**](getswapdto.md) |             |       |

#### Return type

[**JsonObject**](../../dart/doc/JsonObject.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](oneinchapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## **tokens**

> JsonObject tokens(body)

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

final api = Moonsdk().getOneinchApi();
final JsonObject body = ; // JsonObject | 

try {
    final response = api.tokens(body);
    print(response);
} catch on DioException (e) {
    print('Exception when calling OneinchApi->tokens: $e\n');
}
```

#### Parameters

| Name     | Type           | Description | Notes |
| -------- | -------------- | ----------- | ----- |
| **body** | **JsonObject** |             |       |

#### Return type

[**JsonObject**](../../dart/doc/JsonObject.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](oneinchapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)