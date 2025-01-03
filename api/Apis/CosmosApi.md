# CosmosApi

All URIs are relative to *https://beta.usemoon.ai*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**cosmosCosmosCreateAccount**](CosmosApi.md#cosmosCosmosCreateAccount) | **POST** /cosmos |  |
| [**cosmosCosmosDeleteAccount**](CosmosApi.md#cosmosCosmosDeleteAccount) | **DELETE** /cosmos/{accountName} |  |
| [**cosmosCosmosExportAccount**](CosmosApi.md#cosmosCosmosExportAccount) | **POST** /cosmos/{accountName}/export |  |
| [**cosmosCosmosGetAccount**](CosmosApi.md#cosmosCosmosGetAccount) | **GET** /cosmos/{accountName} |  |
| [**cosmosCosmosListAccounts**](CosmosApi.md#cosmosCosmosListAccounts) | **GET** /cosmos |  |
| [**cosmosCosmosSignIBCTransferTransaction**](CosmosApi.md#cosmosCosmosSignIBCTransferTransaction) | **POST** /cosmos/{accountName}/sign-ibc-transfer |  |
| [**cosmosCosmosSignMessage**](CosmosApi.md#cosmosCosmosSignMessage) | **POST** /cosmos/{accountName}/sign-message |  |
| [**cosmosCosmosSignTransferTransaction**](CosmosApi.md#cosmosCosmosSignTransferTransaction) | **POST** /cosmos/{accountName}/sign-transfer |  |


<a name="cosmosCosmosCreateAccount"></a>
# **cosmosCosmosCreateAccount**
> CosmosAccountAPIResponse cosmosCosmosCreateAccount(Authorization, Cosmos\_CosmosCreateAccount\_request)



    Creates a new Cosmos account.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**| - The authorization token from the request header. | [default to null] |
| **Cosmos\_CosmosCreateAccount\_request** | [**Cosmos_CosmosCreateAccount_request**](../Models/Cosmos_CosmosCreateAccount_request.md)| - The request body containing optional network information. | |

### Return type

[**CosmosAccountAPIResponse**](../Models/CosmosAccountAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="cosmosCosmosDeleteAccount"></a>
# **cosmosCosmosDeleteAccount**
> BaseCosmosAPIResponse cosmosCosmosDeleteAccount(Authorization, accountName)



    Deletes an account in the Cosmos SDK.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**| - The authorization token provided in the request header. | [default to null] |
| **accountName** | **String**| - The name of the account to be deleted. | [default to null] |

### Return type

[**BaseCosmosAPIResponse**](../Models/BaseCosmosAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="cosmosCosmosExportAccount"></a>
# **cosmosCosmosExportAccount**
> BaseCosmosAPIResponse cosmosCosmosExportAccount(Authorization, accountName)



    Exports a Cosmos account.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**| - The authorization token provided in the request header. | [default to null] |
| **accountName** | **String**| - The name of the account to be exported. | [default to null] |

### Return type

[**BaseCosmosAPIResponse**](../Models/BaseCosmosAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="cosmosCosmosGetAccount"></a>
# **cosmosCosmosGetAccount**
> CosmosAccountAPIResponse cosmosCosmosGetAccount(Authorization, accountName)



    Retrieves account information from the Cosmos SDK.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**| - The authorization token provided in the request header. | [default to null] |
| **accountName** | **String**| - The name of the account to retrieve. | [default to null] |

### Return type

[**CosmosAccountAPIResponse**](../Models/CosmosAccountAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="cosmosCosmosListAccounts"></a>
# **cosmosCosmosListAccounts**
> CosmosAccountListAPIResponse cosmosCosmosListAccounts(Authorization)



    Lists Cosmos accounts associated with the provided authorization token.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**| - The authorization token from the request header. | [default to null] |

### Return type

[**CosmosAccountListAPIResponse**](../Models/CosmosAccountListAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="cosmosCosmosSignIBCTransferTransaction"></a>
# **cosmosCosmosSignIBCTransferTransaction**
> CosmosTransactionAPIResponse cosmosCosmosSignIBCTransferTransaction(Authorization, accountName, CosmosIBCTransferInput)



    Signs an IBC transfer transaction for a given account.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**| - The authorization token from the request header. | [default to null] |
| **accountName** | **String**| - The name of the account for which the transaction is being signed. | [default to null] |
| **CosmosIBCTransferInput** | [**CosmosIBCTransferInput**](../Models/CosmosIBCTransferInput.md)| - The input data for the Cosmos IBC transfer transaction. | |

### Return type

[**CosmosTransactionAPIResponse**](../Models/CosmosTransactionAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="cosmosCosmosSignMessage"></a>
# **cosmosCosmosSignMessage**
> CosmosSignedMessageAPIResponse cosmosCosmosSignMessage(Authorization, accountName, CosmosSignMessageInput)



    Signs a message using the Cosmos SDK.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**| - The authorization token from the request header. | [default to null] |
| **accountName** | **String**| - The name of the account to sign the message for. | [default to null] |
| **CosmosSignMessageInput** | [**CosmosSignMessageInput**](../Models/CosmosSignMessageInput.md)| - The input data required to sign the message. | |

### Return type

[**CosmosSignedMessageAPIResponse**](../Models/CosmosSignedMessageAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="cosmosCosmosSignTransferTransaction"></a>
# **cosmosCosmosSignTransferTransaction**
> CosmosTransactionAPIResponse cosmosCosmosSignTransferTransaction(Authorization, accountName, CosmosTransferInput)



    Signs a transfer transaction using the provided authorization token and account name.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**| - The authorization token provided in the request header. | [default to null] |
| **accountName** | **String**| - The name of the account to sign the transaction for. | [default to null] |
| **CosmosTransferInput** | [**CosmosTransferInput**](../Models/CosmosTransferInput.md)| - The transfer input details required for the transaction. | |

### Return type

[**CosmosTransactionAPIResponse**](../Models/CosmosTransactionAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

