# PaymentApi

## openapi.api.PaymentApi

### Load the API package

```dart
import 'package:openapi/api.dart';
```

All URIs are relative to _https://vault-api.usemoon.ai_

| Method                                                                       | HTTP request                         | Description |
| ---------------------------------------------------------------------------- | ------------------------------------ | ----------- |
| [**createPaymentIntentConfig**](paymentapi.md#createpaymentintentconfig)     | **POST** /payment/config             |             |
| [**deletePaymentIntentConfig**](paymentapi.md#deletepaymentintentconfig)     | **DELETE** /payment/config/{id}      |             |
| [**getAllPaymentIntentConfigs**](paymentapi.md#getallpaymentintentconfigs)   | **GET** /payment/config              |             |
| [**getOnePaymentIntentConfigs**](paymentapi.md#getonepaymentintentconfigs)   | **GET** /payment/config/{id}         |             |
| [**moralisWebhook**](paymentapi.md#moraliswebhook)                           | **POST** /payment/webhook/{id}       |             |
| [**paymentCreatePaymentIntent**](paymentapi.md#paymentcreatepaymentintent)   | **POST** /payment                    |             |
| [**paymentDeletePaymentIntent**](paymentapi.md#paymentdeletepaymentintent)   | **DELETE** /payment/{id}             |             |
| [**paymentGetAllPaymentIntents**](paymentapi.md#paymentgetallpaymentintents) | **GET** /payment                     |             |
| [**paymentGetAvailableChains**](paymentapi.md#paymentgetavailablechains)     | **GET** /payment/chains              |             |
| [**paymentGetPaymentIntent**](paymentapi.md#paymentgetpaymentintent)         | **GET** /payment/{id}                |             |
| [**paymentUpdatePaymentIntent**](paymentapi.md#paymentupdatepaymentintent)   | **PUT** /payment/{id}                |             |
| [**tatumWebhook**](paymentapi.md#tatumwebhook)                               | **POST** /payment/webhook/tatum/{id} |             |
| [**updatePaymentIntentConfig**](paymentapi.md#updatepaymentintentconfig)     | **PUT** /payment/config/{id}         |             |

## **createPaymentIntentConfig**

> JsonObject createPaymentIntentConfig(authorization, body)

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

final api = Openapi().getPaymentApi();
final String authorization = authorization_example; // String | 
final JsonObject body = ; // JsonObject | 

try {
    final response = api.createPaymentIntentConfig(authorization, body);
    print(response);
} catch on DioException (e) {
    print('Exception when calling PaymentApi->createPaymentIntentConfig: $e\n');
}
```

#### Parameters

| Name              | Type           | Description | Notes |
| ----------------- | -------------- | ----------- | ----- |
| **authorization** | **String**     |             |       |
| **body**          | **JsonObject** |             |       |

#### Return type

[**JsonObject**](../../dart/doc/JsonObject.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](paymentapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## **deletePaymentIntentConfig**

> PaymentIntentResponse deletePaymentIntentConfig(authorization, id)

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

final api = Openapi().getPaymentApi();
final String authorization = authorization_example; // String | 
final String id = id_example; // String | 

try {
    final response = api.deletePaymentIntentConfig(authorization, id);
    print(response);
} catch on DioException (e) {
    print('Exception when calling PaymentApi->deletePaymentIntentConfig: $e\n');
}
```

#### Parameters

| Name              | Type       | Description | Notes |
| ----------------- | ---------- | ----------- | ----- |
| **authorization** | **String** |             |       |
| **id**            | **String** |             |       |

#### Return type

[**PaymentIntentResponse**](paymentintentresponse.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: Not defined
* **Accept**: application/json

[\[Back to top\]](paymentapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## **getAllPaymentIntentConfigs**

> BuiltList getAllPaymentIntentConfigs(authorization)

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

final api = Openapi().getPaymentApi();
final String authorization = authorization_example; // String | 

try {
    final response = api.getAllPaymentIntentConfigs(authorization);
    print(response);
} catch on DioException (e) {
    print('Exception when calling PaymentApi->getAllPaymentIntentConfigs: $e\n');
}
```

#### Parameters

| Name              | Type       | Description | Notes |
| ----------------- | ---------- | ----------- | ----- |
| **authorization** | **String** |             |       |

#### Return type

[**BuiltList\<PaymentIntentResponse>**](paymentintentresponse.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: Not defined
* **Accept**: application/json

[\[Back to top\]](paymentapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## **getOnePaymentIntentConfigs**

> PaymentIntentResponse getOnePaymentIntentConfigs(authorization, id)

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

final api = Openapi().getPaymentApi();
final String authorization = authorization_example; // String | 
final String id = id_example; // String | 

try {
    final response = api.getOnePaymentIntentConfigs(authorization, id);
    print(response);
} catch on DioException (e) {
    print('Exception when calling PaymentApi->getOnePaymentIntentConfigs: $e\n');
}
```

#### Parameters

| Name              | Type       | Description | Notes |
| ----------------- | ---------- | ----------- | ----- |
| **authorization** | **String** |             |       |
| **id**            | **String** |             |       |

#### Return type

[**PaymentIntentResponse**](paymentintentresponse.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: Not defined
* **Accept**: application/json

[\[Back to top\]](paymentapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## **moralisWebhook**

> JsonObject moralisWebhook(id, iWebhook)

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

final api = Openapi().getPaymentApi();
final String id = id_example; // String | 
final IWebhook iWebhook = ; // IWebhook | 

try {
    final response = api.moralisWebhook(id, iWebhook);
    print(response);
} catch on DioException (e) {
    print('Exception when calling PaymentApi->moralisWebhook: $e\n');
}
```

#### Parameters

| Name         | Type                        | Description | Notes |
| ------------ | --------------------------- | ----------- | ----- |
| **id**       | **String**                  |             |       |
| **iWebhook** | [**IWebhook**](iwebhook.md) |             |       |

#### Return type

[**JsonObject**](../../dart/doc/JsonObject.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](paymentapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## **paymentCreatePaymentIntent**

> PaymentIntentResponse paymentCreatePaymentIntent(authorization, createPaymentIntentInput)

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

final api = Openapi().getPaymentApi();
final String authorization = authorization_example; // String | 
final CreatePaymentIntentInput createPaymentIntentInput = ; // CreatePaymentIntentInput | 

try {
    final response = api.paymentCreatePaymentIntent(authorization, createPaymentIntentInput);
    print(response);
} catch on DioException (e) {
    print('Exception when calling PaymentApi->paymentCreatePaymentIntent: $e\n');
}
```

#### Parameters

| Name                         | Type                                                        | Description | Notes |
| ---------------------------- | ----------------------------------------------------------- | ----------- | ----- |
| **authorization**            | **String**                                                  |             |       |
| **createPaymentIntentInput** | [**CreatePaymentIntentInput**](createpaymentintentinput.md) |             |       |

#### Return type

[**PaymentIntentResponse**](paymentintentresponse.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](paymentapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## **paymentDeletePaymentIntent**

> PaymentIntentResponse paymentDeletePaymentIntent(authorization, id)

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

final api = Openapi().getPaymentApi();
final String authorization = authorization_example; // String | 
final String id = id_example; // String | 

try {
    final response = api.paymentDeletePaymentIntent(authorization, id);
    print(response);
} catch on DioException (e) {
    print('Exception when calling PaymentApi->paymentDeletePaymentIntent: $e\n');
}
```

#### Parameters

| Name              | Type       | Description | Notes |
| ----------------- | ---------- | ----------- | ----- |
| **authorization** | **String** |             |       |
| **id**            | **String** |             |       |

#### Return type

[**PaymentIntentResponse**](paymentintentresponse.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: Not defined
* **Accept**: application/json

[\[Back to top\]](paymentapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## **paymentGetAllPaymentIntents**

> BuiltList paymentGetAllPaymentIntents(authorization)

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

final api = Openapi().getPaymentApi();
final String authorization = authorization_example; // String | 

try {
    final response = api.paymentGetAllPaymentIntents(authorization);
    print(response);
} catch on DioException (e) {
    print('Exception when calling PaymentApi->paymentGetAllPaymentIntents: $e\n');
}
```

#### Parameters

| Name              | Type       | Description | Notes |
| ----------------- | ---------- | ----------- | ----- |
| **authorization** | **String** |             |       |

#### Return type

[**BuiltList\<PaymentIntentResponse>**](paymentintentresponse.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: Not defined
* **Accept**: application/json

[\[Back to top\]](paymentapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## **paymentGetAvailableChains**

> BuiltList paymentGetAvailableChains()

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

final api = Openapi().getPaymentApi();

try {
    final response = api.paymentGetAvailableChains();
    print(response);
} catch on DioException (e) {
    print('Exception when calling PaymentApi->paymentGetAvailableChains: $e\n');
}
```

#### Parameters

This endpoint does not need any parameter.

#### Return type

**BuiltList\<String>**

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: Not defined
* **Accept**: application/json

[\[Back to top\]](paymentapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## **paymentGetPaymentIntent**

> PaymentIntentResponse paymentGetPaymentIntent(authorization, id)

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

final api = Openapi().getPaymentApi();
final String authorization = authorization_example; // String | 
final String id = id_example; // String | 

try {
    final response = api.paymentGetPaymentIntent(authorization, id);
    print(response);
} catch on DioException (e) {
    print('Exception when calling PaymentApi->paymentGetPaymentIntent: $e\n');
}
```

#### Parameters

| Name              | Type       | Description | Notes |
| ----------------- | ---------- | ----------- | ----- |
| **authorization** | **String** |             |       |
| **id**            | **String** |             |       |

#### Return type

[**PaymentIntentResponse**](paymentintentresponse.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: Not defined
* **Accept**: application/json

[\[Back to top\]](paymentapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## **paymentUpdatePaymentIntent**

> PaymentIntentResponse paymentUpdatePaymentIntent(authorization, id, createPaymentIntentInput)

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

final api = Openapi().getPaymentApi();
final String authorization = authorization_example; // String | 
final String id = id_example; // String | 
final CreatePaymentIntentInput createPaymentIntentInput = ; // CreatePaymentIntentInput | 

try {
    final response = api.paymentUpdatePaymentIntent(authorization, id, createPaymentIntentInput);
    print(response);
} catch on DioException (e) {
    print('Exception when calling PaymentApi->paymentUpdatePaymentIntent: $e\n');
}
```

#### Parameters

| Name                         | Type                                                        | Description | Notes |
| ---------------------------- | ----------------------------------------------------------- | ----------- | ----- |
| **authorization**            | **String**                                                  |             |       |
| **id**                       | **String**                                                  |             |       |
| **createPaymentIntentInput** | [**CreatePaymentIntentInput**](createpaymentintentinput.md) |             |       |

#### Return type

[**PaymentIntentResponse**](paymentintentresponse.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](paymentapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## **tatumWebhook**

> JsonObject tatumWebhook(id, tatumTransactionEvent)

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

final api = Openapi().getPaymentApi();
final String id = id_example; // String | 
final TatumTransactionEvent tatumTransactionEvent = ; // TatumTransactionEvent | 

try {
    final response = api.tatumWebhook(id, tatumTransactionEvent);
    print(response);
} catch on DioException (e) {
    print('Exception when calling PaymentApi->tatumWebhook: $e\n');
}
```

#### Parameters

| Name                      | Type                                                  | Description | Notes |
| ------------------------- | ----------------------------------------------------- | ----------- | ----- |
| **id**                    | **String**                                            |             |       |
| **tatumTransactionEvent** | [**TatumTransactionEvent**](tatumtransactionevent.md) |             |       |

#### Return type

[**JsonObject**](../../dart/doc/JsonObject.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](paymentapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## **updatePaymentIntentConfig**

> PaymentIntentResponse updatePaymentIntentConfig(authorization, id, body)

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

final api = Openapi().getPaymentApi();
final String authorization = authorization_example; // String | 
final String id = id_example; // String | 
final JsonObject body = ; // JsonObject | 

try {
    final response = api.updatePaymentIntentConfig(authorization, id, body);
    print(response);
} catch on DioException (e) {
    print('Exception when calling PaymentApi->updatePaymentIntentConfig: $e\n');
}
```

#### Parameters

| Name              | Type           | Description | Notes |
| ----------------- | -------------- | ----------- | ----- |
| **authorization** | **String**     |             |       |
| **id**            | **String**     |             |       |
| **body**          | **JsonObject** |             |       |

#### Return type

[**PaymentIntentResponse**](paymentintentresponse.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](paymentapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)
