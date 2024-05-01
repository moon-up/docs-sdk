# BitcoincashApi

All URIs are relative to *https://beta.usemoon.ai*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createBitcoinCashAccount**](BitcoincashApi.md#createBitcoinCashAccount) | **POST** /bitcoincash |  |
| [**getBitcoinCashAccount**](BitcoincashApi.md#getBitcoinCashAccount) | **GET** /bitcoincash/{accountName} |  |
| [**listBitcoinCashAccounts**](BitcoincashApi.md#listBitcoinCashAccounts) | **GET** /bitcoincash |  |
| [**signBitcoinCashTransaction**](BitcoincashApi.md#signBitcoinCashTransaction) | **POST** /bitcoincash/{accountName}/sign-tx |  |


<a name="createBitcoinCashAccount"></a>
# **createBitcoinCashAccount**
> AccountAPIResponse createBitcoinCashAccount(Authorization, BitcoinCashInput)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **BitcoinCashInput** | [**BitcoinCashInput**](../Models/BitcoinCashInput.md)|  | |

### Return type

[**AccountAPIResponse**](../Models/AccountAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="getBitcoinCashAccount"></a>
# **getBitcoinCashAccount**
> AccountAPIResponse getBitcoinCashAccount(Authorization, accountName)



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

<a name="listBitcoinCashAccounts"></a>
# **listBitcoinCashAccounts**
> AccountAPIResponse listBitcoinCashAccounts(Authorization)



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

<a name="signBitcoinCashTransaction"></a>
# **signBitcoinCashTransaction**
> BitcoinCashAPIResponse signBitcoinCashTransaction(Authorization, accountName, BitcoinCashTransactionInput)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **accountName** | **String**|  | [default to null] |
| **BitcoinCashTransactionInput** | [**BitcoinCashTransactionInput**](../Models/BitcoinCashTransactionInput.md)|  | |

### Return type

[**BitcoinCashAPIResponse**](../Models/BitcoinCashAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

