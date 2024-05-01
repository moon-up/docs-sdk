# CosmosApi

All URIs are relative to *https://beta.usemoon.ai*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createCosmosAccount**](CosmosApi.md#createCosmosAccount) | **POST** /cosmos |  |
| [**getCosmosAccount**](CosmosApi.md#getCosmosAccount) | **GET** /cosmos/{accountName} |  |
| [**listCosmosAccounts**](CosmosApi.md#listCosmosAccounts) | **GET** /cosmos |  |
| [**signCosmosTransaction**](CosmosApi.md#signCosmosTransaction) | **POST** /cosmos/{accountName}/sign-tx |  |


<a name="createCosmosAccount"></a>
# **createCosmosAccount**
> AccountAPIResponse createCosmosAccount(Authorization, CosmosInput)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **CosmosInput** | [**CosmosInput**](../Models/CosmosInput.md)|  | |

### Return type

[**AccountAPIResponse**](../Models/AccountAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="getCosmosAccount"></a>
# **getCosmosAccount**
> AccountAPIResponse getCosmosAccount(Authorization, accountName)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **accountName** | **String**|  | [default to null] |

### Return type

[**AccountAPIResponse**](../Models/AccountAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="listCosmosAccounts"></a>
# **listCosmosAccounts**
> AccountAPIResponse listCosmosAccounts(Authorization)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |

### Return type

[**AccountAPIResponse**](../Models/AccountAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="signCosmosTransaction"></a>
# **signCosmosTransaction**
> CosmosAPIResponse signCosmosTransaction(Authorization, accountName, CosmosTransactionInput)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **accountName** | **String**|  | [default to null] |
| **CosmosTransactionInput** | [**CosmosTransactionInput**](../Models/CosmosTransactionInput.md)|  | |

### Return type

[**CosmosAPIResponse**](../Models/CosmosAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

