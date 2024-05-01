# AaveApi

## moonsdk.api.AaveApi

### Load the API package

```dart
import 'package:moonsdk/api.dart';
```

All URIs are relative to _https://beta.usemoon.ai_

| Method                                            | HTTP request                            | Description |
| ------------------------------------------------- | --------------------------------------- | ----------- |
| [**borrow**](aaveapi.md#borrow)                   | **POST** /aave/{name}/borrow            |             |
| [**lend**](aaveapi.md#lend)                       | **POST** /aave/{name}/lend              |             |
| [**repay**](aaveapi.md#repay)                     | **POST** /aave/{name}/repay             |             |
| [**userReserveData**](aaveapi.md#userreservedata) | **POST** /aave/{name}/user-reserve-data |             |

## **borrow**

> TransactionAPIResponse borrow(authorization, name, aaveInput)

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

final api = Moonsdk().getAaveApi();
final String authorization = authorization_example; // String | 
final String name = name_example; // String | 
final AaveInput aaveInput = ; // AaveInput | 

try {
    final response = api.borrow(authorization, name, aaveInput);
    print(response);
} catch on DioException (e) {
    print('Exception when calling AaveApi->borrow: $e\n');
}
```

#### Parameters

| Name              | Type                          | Description | Notes |
| ----------------- | ----------------------------- | ----------- | ----- |
| **authorization** | **String**                    |             |       |
| **name**          | **String**                    |             |       |
| **aaveInput**     | [**AaveInput**](aaveinput.md) |             |       |

#### Return type

[**TransactionAPIResponse**](transactionapiresponse.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](aaveapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## **lend**

> TransactionAPIResponse lend(authorization, name, aaveInput)

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

final api = Moonsdk().getAaveApi();
final String authorization = authorization_example; // String | 
final String name = name_example; // String | 
final AaveInput aaveInput = ; // AaveInput | 

try {
    final response = api.lend(authorization, name, aaveInput);
    print(response);
} catch on DioException (e) {
    print('Exception when calling AaveApi->lend: $e\n');
}
```

#### Parameters

| Name              | Type                          | Description | Notes |
| ----------------- | ----------------------------- | ----------- | ----- |
| **authorization** | **String**                    |             |       |
| **name**          | **String**                    |             |       |
| **aaveInput**     | [**AaveInput**](aaveinput.md) |             |       |

#### Return type

[**TransactionAPIResponse**](transactionapiresponse.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](aaveapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## **repay**

> TransactionAPIResponse repay(authorization, name, aaveInput)

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

final api = Moonsdk().getAaveApi();
final String authorization = authorization_example; // String | 
final String name = name_example; // String | 
final AaveInput aaveInput = ; // AaveInput | 

try {
    final response = api.repay(authorization, name, aaveInput);
    print(response);
} catch on DioException (e) {
    print('Exception when calling AaveApi->repay: $e\n');
}
```

#### Parameters

| Name              | Type                          | Description | Notes |
| ----------------- | ----------------------------- | ----------- | ----- |
| **authorization** | **String**                    |             |       |
| **name**          | **String**                    |             |       |
| **aaveInput**     | [**AaveInput**](aaveinput.md) |             |       |

#### Return type

[**TransactionAPIResponse**](transactionapiresponse.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](aaveapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## **userReserveData**

> AaveReservesAPIResponse userReserveData(authorization, name, aaveInput)

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

final api = Moonsdk().getAaveApi();
final String authorization = authorization_example; // String | 
final String name = name_example; // String | 
final AaveInput aaveInput = ; // AaveInput | 

try {
    final response = api.userReserveData(authorization, name, aaveInput);
    print(response);
} catch on DioException (e) {
    print('Exception when calling AaveApi->userReserveData: $e\n');
}
```

#### Parameters

| Name              | Type                          | Description | Notes |
| ----------------- | ----------------------------- | ----------- | ----- |
| **authorization** | **String**                    |             |       |
| **name**          | **String**                    |             |       |
| **aaveInput**     | [**AaveInput**](aaveinput.md) |             |       |

#### Return type

[**AaveReservesAPIResponse**](aavereservesapiresponse.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](aaveapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)
