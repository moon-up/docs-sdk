# AccountsApi

All URIs are relative to *https://beta.usemoon.ai*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**broadcastTx**](AccountsApi.md#broadcastTx) | **POST** /accounts/{accountName}/broadcast-tx |  |
| [**createAccount**](AccountsApi.md#createAccount) | **POST** /accounts |  |
| [**deleteAccount**](AccountsApi.md#deleteAccount) | **DELETE** /accounts/{accountName} |  |
| [**deployContract**](AccountsApi.md#deployContract) | **POST** /accounts/{accountName}/deploy |  |
| [**getAccount**](AccountsApi.md#getAccount) | **GET** /accounts/{accountName} |  |
| [**getBalance**](AccountsApi.md#getBalance) | **GET** /accounts/{accountName}/balance |  |
| [**getNonce**](AccountsApi.md#getNonce) | **GET** /accounts/{accountName}/nonce |  |
| [**listAccounts**](AccountsApi.md#listAccounts) | **GET** /accounts |  |
| [**signMessage**](AccountsApi.md#signMessage) | **POST** /accounts/{accountName}/sign-message |  |
| [**signTransaction**](AccountsApi.md#signTransaction) | **POST** /accounts/{accountName}/sign-transaction |  |
| [**signTypedData**](AccountsApi.md#signTypedData) | **POST** /accounts/{accountName}/sign-typed-data |  |
| [**transferEth**](AccountsApi.md#transferEth) | **POST** /accounts/{accountName}/transfer-eth |  |


<a name="broadcastTx"></a>
# **broadcastTx**
> BroadCastRawTransactionAPIResponse broadcastTx(Authorization, accountName, BroadcastInput)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **accountName** | **String**|  | [default to null] |
| **BroadcastInput** | [**BroadcastInput**](../Models/BroadcastInput.md)|  | |

### Return type

[**BroadCastRawTransactionAPIResponse**](../Models/BroadCastRawTransactionAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="createAccount"></a>
# **createAccount**
> AccountAPIResponse createAccount(Authorization, CreateAccountInput)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **CreateAccountInput** | [**CreateAccountInput**](../Models/CreateAccountInput.md)|  | |

### Return type

[**AccountAPIResponse**](../Models/AccountAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="deleteAccount"></a>
# **deleteAccount**
> AccountAPIResponse deleteAccount(Authorization, accountName)



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

<a name="deployContract"></a>
# **deployContract**
> TransactionAPIResponse deployContract(Authorization, accountName, DeployInput)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **accountName** | **String**|  | [default to null] |
| **DeployInput** | [**DeployInput**](../Models/DeployInput.md)|  | |

### Return type

[**TransactionAPIResponse**](../Models/TransactionAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="getAccount"></a>
# **getAccount**
> AccountAPIResponse getAccount(Authorization, accountName)



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

<a name="getBalance"></a>
# **getBalance**
> BalanceAPIResponse getBalance(accountName, Authorization, chainId)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **accountName** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |

### Return type

[**BalanceAPIResponse**](../Models/BalanceAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getNonce"></a>
# **getNonce**
> NonceAPIResponse getNonce(accountName, Authorization)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **accountName** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |

### Return type

[**NonceAPIResponse**](../Models/NonceAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="listAccounts"></a>
# **listAccounts**
> AccountAPIResponse listAccounts(Authorization)



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

<a name="signMessage"></a>
# **signMessage**
> SignMessageAPIResponse signMessage(accountName, Authorization, SignMessage)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **accountName** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **SignMessage** | [**SignMessage**](../Models/SignMessage.md)|  | |

### Return type

[**SignMessageAPIResponse**](../Models/SignMessageAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="signTransaction"></a>
# **signTransaction**
> TransactionAPIResponse signTransaction(accountName, Authorization, InputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **accountName** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **InputBody** | [**InputBody**](../Models/InputBody.md)|  | |

### Return type

[**TransactionAPIResponse**](../Models/TransactionAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="signTypedData"></a>
# **signTypedData**
> SignMessageAPIResponse signTypedData(accountName, Authorization, SignTypedData)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **accountName** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **SignTypedData** | [**SignTypedData**](../Models/SignTypedData.md)|  | |

### Return type

[**SignMessageAPIResponse**](../Models/SignMessageAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="transferEth"></a>
# **transferEth**
> TransactionAPIResponse transferEth(accountName, Authorization, InputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **accountName** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **InputBody** | [**InputBody**](../Models/InputBody.md)|  | |

### Return type

[**TransactionAPIResponse**](../Models/TransactionAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

