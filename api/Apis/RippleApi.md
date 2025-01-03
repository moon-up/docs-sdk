# RippleApi

All URIs are relative to *https://beta.usemoon.ai*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createRippleAccount**](RippleApi.md#createRippleAccount) | **POST** /ripple |  |
| [**deleteRippleAccount**](RippleApi.md#deleteRippleAccount) | **POST** /ripple/{accountName}/delete |  |
| [**exportRippleAccount**](RippleApi.md#exportRippleAccount) | **POST** /ripple/{accountName}/export |  |
| [**getRippleAccount**](RippleApi.md#getRippleAccount) | **GET** /ripple/{accountName} |  |
| [**listRippleAccounts**](RippleApi.md#listRippleAccounts) | **GET** /ripple |  |
| [**signRippleTransaction**](RippleApi.md#signRippleTransaction) | **POST** /ripple/{accountName}/sign-tx |  |


<a name="createRippleAccount"></a>
# **createRippleAccount**
> AccountAPIResponse createRippleAccount(Authorization, RippleInput)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **RippleInput** | [**RippleInput**](../Models/RippleInput.md)|  | |

### Return type

[**AccountAPIResponse**](../Models/AccountAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="deleteRippleAccount"></a>
# **deleteRippleAccount**
> AccountAPIResponse deleteRippleAccount(Authorization, accountName)



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

<a name="exportRippleAccount"></a>
# **exportRippleAccount**
> AccountAPIResponse exportRippleAccount(Authorization, accountName)



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

<a name="getRippleAccount"></a>
# **getRippleAccount**
> AccountAPIResponse getRippleAccount(Authorization, accountName)



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

<a name="listRippleAccounts"></a>
# **listRippleAccounts**
> AccountAPIResponse listRippleAccounts(Authorization)



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

<a name="signRippleTransaction"></a>
# **signRippleTransaction**
> RippleAPIResponse signRippleTransaction(Authorization, accountName, RippleTransactionInput)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **accountName** | **String**|  | [default to null] |
| **RippleTransactionInput** | [**RippleTransactionInput**](../Models/RippleTransactionInput.md)|  | |

### Return type

[**RippleAPIResponse**](../Models/RippleAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

