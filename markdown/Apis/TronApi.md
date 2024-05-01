# TronApi

All URIs are relative to *https://beta.usemoon.ai*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createTronAccount**](TronApi.md#createTronAccount) | **POST** /tron |  |
| [**getTronAccount**](TronApi.md#getTronAccount) | **GET** /tron/{accountName} |  |
| [**listTronAccounts**](TronApi.md#listTronAccounts) | **GET** /tron |  |
| [**signTronTransaction**](TronApi.md#signTronTransaction) | **POST** /tron/{accountName}/sign-tx |  |


<a name="createTronAccount"></a>
# **createTronAccount**
> AccountAPIResponse createTronAccount(Authorization, TronInput)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **TronInput** | [**TronInput**](../Models/TronInput.md)|  | |

### Return type

[**AccountAPIResponse**](../Models/AccountAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="getTronAccount"></a>
# **getTronAccount**
> AccountAPIResponse getTronAccount(Authorization, accountName)



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

<a name="listTronAccounts"></a>
# **listTronAccounts**
> AccountAPIResponse listTronAccounts(Authorization)



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

<a name="signTronTransaction"></a>
# **signTronTransaction**
> TronAPIResponse signTronTransaction(Authorization, accountName, TronTransactionInput)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **accountName** | **String**|  | [default to null] |
| **TronTransactionInput** | [**TronTransactionInput**](../Models/TronTransactionInput.md)|  | |

### Return type

[**TronAPIResponse**](../Models/TronAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

