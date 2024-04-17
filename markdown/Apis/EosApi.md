# EosApi

All URIs are relative to *https://beta.usemoon.ai*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createEosAccount**](EosApi.md#createEosAccount) | **POST** /eos |  |
| [**getEosAccount**](EosApi.md#getEosAccount) | **GET** /eos/{accountName} |  |
| [**listEosAccounts**](EosApi.md#listEosAccounts) | **GET** /eos |  |
| [**signEosTransaction**](EosApi.md#signEosTransaction) | **POST** /eos/{accountName}/sign-tx |  |


<a name="createEosAccount"></a>
# **createEosAccount**
> AccountAPIResponse createEosAccount(Authorization, EosInput)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **EosInput** | [**EosInput**](../Models/EosInput.md)|  | |

### Return type

[**AccountAPIResponse**](../Models/AccountAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="getEosAccount"></a>
# **getEosAccount**
> AccountAPIResponse getEosAccount(Authorization, accountName)



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

<a name="listEosAccounts"></a>
# **listEosAccounts**
> AccountAPIResponse listEosAccounts(Authorization)



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

<a name="signEosTransaction"></a>
# **signEosTransaction**
> EosAPIResponse signEosTransaction(Authorization, accountName, EosTransactionInput)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **accountName** | **String**|  | [default to null] |
| **EosTransactionInput** | [**EosTransactionInput**](../Models/EosTransactionInput.md)|  | |

### Return type

[**EosAPIResponse**](../Models/EosAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

