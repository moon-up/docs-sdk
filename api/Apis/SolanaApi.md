# SolanaApi

All URIs are relative to *https://beta.usemoon.ai*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createSolanaAccount**](SolanaApi.md#createSolanaAccount) | **POST** /solana |  |
| [**deleteSolanaAccount**](SolanaApi.md#deleteSolanaAccount) | **POST** /solana/{accountName}/delete |  |
| [**exportSolanaAccount**](SolanaApi.md#exportSolanaAccount) | **POST** /solana/{accountName}/export |  |
| [**getSolanaAccount**](SolanaApi.md#getSolanaAccount) | **GET** /solana/{accountName} |  |
| [**listSolanaAccounts**](SolanaApi.md#listSolanaAccounts) | **GET** /solana |  |
| [**multiSignSolanaTransaction**](SolanaApi.md#multiSignSolanaTransaction) | **POST** /solana/{accountName}/multi-sign-tx |  |
| [**signSolanaTransaction**](SolanaApi.md#signSolanaTransaction) | **POST** /solana/{accountName}/sign-tx |  |
| [**transferSolanaTransaction**](SolanaApi.md#transferSolanaTransaction) | **POST** /solana/{accountName}/transfer |  |
| [**transferTokensSignSolanaTransaction**](SolanaApi.md#transferTokensSignSolanaTransaction) | **POST** /solana/{accountName}/transfer-tokens |  |


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

<a name="deleteSolanaAccount"></a>
# **deleteSolanaAccount**
> AccountAPIResponse deleteSolanaAccount(Authorization, accountName)



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

<a name="exportSolanaAccount"></a>
# **exportSolanaAccount**
> AccountAPIResponse exportSolanaAccount(Authorization, accountName)



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

<a name="multiSignSolanaTransaction"></a>
# **multiSignSolanaTransaction**
> SolanaAPIResponse multiSignSolanaTransaction(Authorization, accountName, SolanaSignTransactionInput)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **accountName** | **String**|  | [default to null] |
| **SolanaSignTransactionInput** | [**SolanaSignTransactionInput**](../Models/SolanaSignTransactionInput.md)|  | |

### Return type

[**SolanaAPIResponse**](../Models/SolanaAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="signSolanaTransaction"></a>
# **signSolanaTransaction**
> SolanaAPIResponse signSolanaTransaction(Authorization, accountName, SolanaSignTransactionInput)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **accountName** | **String**|  | [default to null] |
| **SolanaSignTransactionInput** | [**SolanaSignTransactionInput**](../Models/SolanaSignTransactionInput.md)|  | |

### Return type

[**SolanaAPIResponse**](../Models/SolanaAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="transferSolanaTransaction"></a>
# **transferSolanaTransaction**
> SolanaAPIResponse transferSolanaTransaction(Authorization, accountName, SolanaTransactionInput)



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

<a name="transferTokensSignSolanaTransaction"></a>
# **transferTokensSignSolanaTransaction**
> SolanaAPIResponse transferTokensSignSolanaTransaction(Authorization, accountName, SolanaTransactionInput)



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

