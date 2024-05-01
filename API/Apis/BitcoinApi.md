# BitcoinApi

All URIs are relative to *https://beta.usemoon.ai*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createBitcoinAccount**](BitcoinApi.md#createBitcoinAccount) | **POST** /bitcoin |  |
| [**getBitcoinAccount**](BitcoinApi.md#getBitcoinAccount) | **GET** /bitcoin/{accountName} |  |
| [**listBitcoinAccounts**](BitcoinApi.md#listBitcoinAccounts) | **GET** /bitcoin |  |
| [**signBitcoinTransaction**](BitcoinApi.md#signBitcoinTransaction) | **POST** /bitcoin/{accountName}/sign-tx |  |


<a name="createBitcoinAccount"></a>
# **createBitcoinAccount**
> AccountAPIResponse createBitcoinAccount(Authorization, BitcoinInput)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **BitcoinInput** | [**BitcoinInput**](../Models/BitcoinInput.md)|  | |

### Return type

[**AccountAPIResponse**](../Models/AccountAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="getBitcoinAccount"></a>
# **getBitcoinAccount**
> AccountAPIResponse getBitcoinAccount(Authorization, accountName)



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

<a name="listBitcoinAccounts"></a>
# **listBitcoinAccounts**
> AccountAPIResponse listBitcoinAccounts(Authorization)



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

<a name="signBitcoinTransaction"></a>
# **signBitcoinTransaction**
> BitcoinAPIResponse signBitcoinTransaction(Authorization, accountName, BitcoinTransactionInput)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **accountName** | **String**|  | [default to null] |
| **BitcoinTransactionInput** | [**BitcoinTransactionInput**](../Models/BitcoinTransactionInput.md)|  | |

### Return type

[**BitcoinAPIResponse**](../Models/BitcoinAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

