# SolanaApi

All URIs are relative to *https://beta.usemoon.ai*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createSolanaAccount**](SolanaApi.md#createSolanaAccount) | **POST** /solana |  |
| [**getSolanaAccount**](SolanaApi.md#getSolanaAccount) | **GET** /solana/{accountName} |  |
| [**listSolanaAccounts**](SolanaApi.md#listSolanaAccounts) | **GET** /solana |  |
| [**signSolanaTransaction**](SolanaApi.md#signSolanaTransaction) | **POST** /solana/{accountName}/sign-tx |  |


<a name="createSolanaAccount"></a>
# **createSolanaAccount**
> AccountAPIResponse createSolanaAccount(Authorization, SolanaInput)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **SolanaInput** | [**SolanaInput**](../Models/SolanaInput.md)|  | |

### Return type

[**AccountAPIResponse**](../Models/AccountAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="getSolanaAccount"></a>
# **getSolanaAccount**
> AccountAPIResponse getSolanaAccount(Authorization, accountName)



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

<a name="listSolanaAccounts"></a>
# **listSolanaAccounts**
> AccountAPIResponse listSolanaAccounts(Authorization)



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

<a name="signSolanaTransaction"></a>
# **signSolanaTransaction**
> SolanaAPIResponse signSolanaTransaction(Authorization, accountName, SolanaTransactionInput)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **accountName** | **String**|  | [default to null] |
| **SolanaTransactionInput** | [**SolanaTransactionInput**](../Models/SolanaTransactionInput.md)|  | |

### Return type

[**SolanaAPIResponse**](../Models/SolanaAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

