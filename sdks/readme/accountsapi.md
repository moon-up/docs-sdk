# AccountsApi

## moonsdk.api.AccountsApi

### Load the API package

```dart
import 'package:moonsdk/api.dart';
```

All URIs are relative to _https://beta.usemoon.ai_

| Method                                                | HTTP request                                      | Description |
| ----------------------------------------------------- | ------------------------------------------------- | ----------- |
| [**broadcastTx**](accountsapi.md#broadcasttx)         | **POST** /accounts/{accountName}/broadcast-tx     |             |
| [**createAccount**](accountsapi.md#createaccount)     | **POST** /accounts                                |             |
| [**deleteAccount**](accountsapi.md#deleteaccount)     | **DELETE** /accounts/{accountName}                |             |
| [**deployContract**](accountsapi.md#deploycontract)   | **POST** /accounts/{accountName}/deploy           |             |
| [**getAccount**](accountsapi.md#getaccount)           | **GET** /accounts/{accountName}                   |             |
| [**getBalance**](accountsapi.md#getbalance)           | **GET** /accounts/{accountName}/balance           |             |
| [**getNonce**](accountsapi.md#getnonce)               | **GET** /accounts/{accountName}/nonce             |             |
| [**listAccounts**](accountsapi.md#listaccounts)       | **GET** /accounts                                 |             |
| [**signMessage**](accountsapi.md#signmessage)         | **POST** /accounts/{accountName}/sign-message     |             |
| [**signTransaction**](accountsapi.md#signtransaction) | **POST** /accounts/{accountName}/sign-transaction |             |
| [**signTypedData**](accountsapi.md#signtypeddata)     | **POST** /accounts/{accountName}/sign-typed-data  |             |
| [**transferEth**](accountsapi.md#transfereth)         | **POST** /accounts/{accountName}/transfer-eth     |             |

## **broadcastTx**

> BroadCastRawTransactionAPIResponse broadcastTx(authorization, accountName, broadcastInput)

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

final api = Moonsdk().getAccountsApi();
final String authorization = authorization_example; // String | 
final String accountName = accountName_example; // String | 
final BroadcastInput broadcastInput = ; // BroadcastInput | 

try {
    final response = api.broadcastTx(authorization, accountName, broadcastInput);
    print(response);
} catch on DioException (e) {
    print('Exception when calling AccountsApi->broadcastTx: $e\n');
}
```

#### Parameters

| Name               | Type                                    | Description | Notes |
| ------------------ | --------------------------------------- | ----------- | ----- |
| **authorization**  | **String**                              |             |       |
| **accountName**    | **String**                              |             |       |
| **broadcastInput** | [**BroadcastInput**](broadcastinput.md) |             |       |

#### Return type

[**BroadCastRawTransactionAPIResponse**](broadcastrawtransactionapiresponse.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](accountsapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## **createAccount**

> AccountAPIResponse createAccount(authorization, createAccountInput)

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

final api = Moonsdk().getAccountsApi();
final String authorization = authorization_example; // String | 
final CreateAccountInput createAccountInput = ; // CreateAccountInput | 

try {
    final response = api.createAccount(authorization, createAccountInput);
    print(response);
} catch on DioException (e) {
    print('Exception when calling AccountsApi->createAccount: $e\n');
}
```

#### Parameters

| Name                   | Type                                            | Description | Notes |
| ---------------------- | ----------------------------------------------- | ----------- | ----- |
| **authorization**      | **String**                                      |             |       |
| **createAccountInput** | [**CreateAccountInput**](createaccountinput.md) |             |       |

#### Return type

[**AccountAPIResponse**](accountapiresponse.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](accountsapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## **deleteAccount**

> AccountAPIResponse deleteAccount(authorization, accountName)

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

final api = Moonsdk().getAccountsApi();
final String authorization = authorization_example; // String | 
final String accountName = accountName_example; // String | 

try {
    final response = api.deleteAccount(authorization, accountName);
    print(response);
} catch on DioException (e) {
    print('Exception when calling AccountsApi->deleteAccount: $e\n');
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

[\[Back to top\]](accountsapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## **deployContract**

> TransactionAPIResponse deployContract(authorization, accountName, deployInput)

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

final api = Moonsdk().getAccountsApi();
final String authorization = authorization_example; // String | 
final String accountName = accountName_example; // String | 
final DeployInput deployInput = ; // DeployInput | 

try {
    final response = api.deployContract(authorization, accountName, deployInput);
    print(response);
} catch on DioException (e) {
    print('Exception when calling AccountsApi->deployContract: $e\n');
}
```

#### Parameters

| Name              | Type                              | Description | Notes |
| ----------------- | --------------------------------- | ----------- | ----- |
| **authorization** | **String**                        |             |       |
| **accountName**   | **String**                        |             |       |
| **deployInput**   | [**DeployInput**](deployinput.md) |             |       |

#### Return type

[**TransactionAPIResponse**](transactionapiresponse.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](accountsapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## **getAccount**

> AccountAPIResponse getAccount(authorization, accountName)

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

final api = Moonsdk().getAccountsApi();
final String authorization = authorization_example; // String | 
final String accountName = accountName_example; // String | 

try {
    final response = api.getAccount(authorization, accountName);
    print(response);
} catch on DioException (e) {
    print('Exception when calling AccountsApi->getAccount: $e\n');
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

[\[Back to top\]](accountsapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## **getBalance**

> BalanceAPIResponse getBalance(accountName, authorization, chainId)

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

final api = Moonsdk().getAccountsApi();
final String accountName = accountName_example; // String | 
final String authorization = authorization_example; // String | 
final String chainId = chainId_example; // String | 

try {
    final response = api.getBalance(accountName, authorization, chainId);
    print(response);
} catch on DioException (e) {
    print('Exception when calling AccountsApi->getBalance: $e\n');
}
```

#### Parameters

| Name              | Type       | Description | Notes |
| ----------------- | ---------- | ----------- | ----- |
| **accountName**   | **String** |             |       |
| **authorization** | **String** |             |       |
| **chainId**       | **String** |             |       |

#### Return type

[**BalanceAPIResponse**](balanceapiresponse.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: Not defined
* **Accept**: application/json

[\[Back to top\]](accountsapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## **getNonce**

> NonceAPIResponse getNonce(accountName, authorization)

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

final api = Moonsdk().getAccountsApi();
final String accountName = accountName_example; // String | 
final String authorization = authorization_example; // String | 

try {
    final response = api.getNonce(accountName, authorization);
    print(response);
} catch on DioException (e) {
    print('Exception when calling AccountsApi->getNonce: $e\n');
}
```

#### Parameters

| Name              | Type       | Description | Notes |
| ----------------- | ---------- | ----------- | ----- |
| **accountName**   | **String** |             |       |
| **authorization** | **String** |             |       |

#### Return type

[**NonceAPIResponse**](nonceapiresponse.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: Not defined
* **Accept**: application/json

[\[Back to top\]](accountsapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## **listAccounts**

> AccountAPIResponse listAccounts(authorization)

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

final api = Moonsdk().getAccountsApi();
final String authorization = authorization_example; // String | 

try {
    final response = api.listAccounts(authorization);
    print(response);
} catch on DioException (e) {
    print('Exception when calling AccountsApi->listAccounts: $e\n');
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

[\[Back to top\]](accountsapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## **signMessage**

> SignMessageAPIResponse signMessage(accountName, authorization, signMessage)

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

final api = Moonsdk().getAccountsApi();
final String accountName = accountName_example; // String | 
final String authorization = authorization_example; // String | 
final SignMessage signMessage = ; // SignMessage | 

try {
    final response = api.signMessage(accountName, authorization, signMessage);
    print(response);
} catch on DioException (e) {
    print('Exception when calling AccountsApi->signMessage: $e\n');
}
```

#### Parameters

| Name              | Type                              | Description | Notes |
| ----------------- | --------------------------------- | ----------- | ----- |
| **accountName**   | **String**                        |             |       |
| **authorization** | **String**                        |             |       |
| **signMessage**   | [**SignMessage**](signmessage.md) |             |       |

#### Return type

[**SignMessageAPIResponse**](signmessageapiresponse.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](accountsapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## **signTransaction**

> TransactionAPIResponse signTransaction(accountName, authorization, inputBody)

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

final api = Moonsdk().getAccountsApi();
final String accountName = accountName_example; // String | 
final String authorization = authorization_example; // String | 
final InputBody inputBody = ; // InputBody | 

try {
    final response = api.signTransaction(accountName, authorization, inputBody);
    print(response);
} catch on DioException (e) {
    print('Exception when calling AccountsApi->signTransaction: $e\n');
}
```

#### Parameters

| Name              | Type                          | Description | Notes |
| ----------------- | ----------------------------- | ----------- | ----- |
| **accountName**   | **String**                    |             |       |
| **authorization** | **String**                    |             |       |
| **inputBody**     | [**InputBody**](inputbody.md) |             |       |

#### Return type

[**TransactionAPIResponse**](transactionapiresponse.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](accountsapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## **signTypedData**

> SignMessageAPIResponse signTypedData(accountName, authorization, signTypedData)

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

final api = Moonsdk().getAccountsApi();
final String accountName = accountName_example; // String | 
final String authorization = authorization_example; // String | 
final SignTypedData signTypedData = ; // SignTypedData | 

try {
    final response = api.signTypedData(accountName, authorization, signTypedData);
    print(response);
} catch on DioException (e) {
    print('Exception when calling AccountsApi->signTypedData: $e\n');
}
```

#### Parameters

| Name              | Type                                  | Description | Notes |
| ----------------- | ------------------------------------- | ----------- | ----- |
| **accountName**   | **String**                            |             |       |
| **authorization** | **String**                            |             |       |
| **signTypedData** | [**SignTypedData**](signtypeddata.md) |             |       |

#### Return type

[**SignMessageAPIResponse**](signmessageapiresponse.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](accountsapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## **transferEth**

> TransactionAPIResponse transferEth(accountName, authorization, inputBody)

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

final api = Moonsdk().getAccountsApi();
final String accountName = accountName_example; // String | 
final String authorization = authorization_example; // String | 
final InputBody inputBody = ; // InputBody | 

try {
    final response = api.transferEth(accountName, authorization, inputBody);
    print(response);
} catch on DioException (e) {
    print('Exception when calling AccountsApi->transferEth: $e\n');
}
```

#### Parameters

| Name              | Type                          | Description | Notes |
| ----------------- | ----------------------------- | ----------- | ----- |
| **accountName**   | **String**                    |             |       |
| **authorization** | **String**                    |             |       |
| **inputBody**     | [**InputBody**](inputbody.md) |             |       |

#### Return type

[**TransactionAPIResponse**](transactionapiresponse.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

[\[Back to top\]](accountsapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)
