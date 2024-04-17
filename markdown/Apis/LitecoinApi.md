# LitecoinApi

All URIs are relative to *https://beta.usemoon.ai*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createLitecoinAccount**](LitecoinApi.md#createLitecoinAccount) | **POST** /litecoin |  |
| [**getLitecoinAccount**](LitecoinApi.md#getLitecoinAccount) | **GET** /litecoin/{accountName} |  |
| [**listLitecoinAccounts**](LitecoinApi.md#listLitecoinAccounts) | **GET** /litecoin |  |
| [**signLitecoinTransaction**](LitecoinApi.md#signLitecoinTransaction) | **POST** /litecoin/{accountName}/sign-tx |  |


<a name="createLitecoinAccount"></a>
# **createLitecoinAccount**
> AccountAPIResponse createLitecoinAccount(Authorization, LitecoinInput)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **LitecoinInput** | [**LitecoinInput**](../Models/LitecoinInput.md)|  | |

### Return type

[**AccountAPIResponse**](../Models/AccountAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="getLitecoinAccount"></a>
# **getLitecoinAccount**
> AccountAPIResponse getLitecoinAccount(Authorization, accountName)



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

<a name="listLitecoinAccounts"></a>
# **listLitecoinAccounts**
> AccountAPIResponse listLitecoinAccounts(Authorization)



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

<a name="signLitecoinTransaction"></a>
# **signLitecoinTransaction**
> LitecoinAPIResponse signLitecoinTransaction(Authorization, accountName, LitecoinTransactionInput)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **accountName** | **String**|  | [default to null] |
| **LitecoinTransactionInput** | [**LitecoinTransactionInput**](../Models/LitecoinTransactionInput.md)|  | |

### Return type

[**LitecoinAPIResponse**](../Models/LitecoinAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

