# ConveyorFinanceApi

## moonsdk.api.ConveyorFinanceApi

### Load the API package

```dart
import 'package:moonsdk/api.dart';
```

All URIs are relative to _https://beta.usemoon.ai_

| Method                                 | HTTP request                          | Description |
| -------------------------------------- | ------------------------------------- | ----------- |
| [**swap**](conveyorfinanceapi.md#swap) | **POST** /conveyorfinance/{name}/swap |             |

## **swap**

> ConveyorFinanceControllerResponse swap(authorization, name, tokenSwapParams)

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

final api = Moonsdk().getConveyorFinanceApi();
final String authorization = authorization_example; // String | 
final String name = name_example; // String | 
final TokenSwapParams tokenSwapParams = ; // TokenSwapParams | 

try {
    final response = api.swap(authorization, name, tokenSwapParams);
    print(response);
} catch on DioException (e) {
    print('Exception when calling ConveyorFinanceApi->swap: $e\n');
}
```

#### Parameters

| Name                | Type                                      | Description | Notes |
| ------------------- | ----------------------------------------- | ----------- | ----- |
| **authorization**   | **String**                                |             |       |
| **name**            | **String**                                |             |       |
| **tokenSwapParams** | [**TokenSwapParams**](tokenswapparams.md) |             |       |

#### Return type

[**ConveyorFinanceControllerResponse**](conveyorfinancecontrollerresponse.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](conveyorfinanceapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)
