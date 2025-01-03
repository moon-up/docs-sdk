# OdosApi

All URIs are relative to *https://beta.usemoon.ai*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**getZapQuote**](OdosApi.md#getZapQuote) | **POST** /odos/{accountName}/get-zap-quote |  |
| [**oDOSAssembleTransaction**](OdosApi.md#oDOSAssembleTransaction) | **POST** /odos/assemble-transaction |  |
| [**oDOSGetContractInfo**](OdosApi.md#oDOSGetContractInfo) | **GET** /odos/contract-info |  |
| [**oDOSGetCurrentBlock**](OdosApi.md#oDOSGetCurrentBlock) | **GET** /odos/current-block |  |
| [**oDOSGetExecutorAddress**](OdosApi.md#oDOSGetExecutorAddress) | **GET** /odos/executor-address |  |
| [**oDOSGetLiquiditySources**](OdosApi.md#oDOSGetLiquiditySources) | **GET** /odos/liquidity-sources |  |
| [**oDOSGetQuote**](OdosApi.md#oDOSGetQuote) | **POST** /odos/{accountName}/get-quote |  |
| [**oDOSGetRouterAddress**](OdosApi.md#oDOSGetRouterAddress) | **GET** /odos/router-address |  |
| [**oDOSGetSupportedChains**](OdosApi.md#oDOSGetSupportedChains) | **GET** /odos/supported-chains |  |
| [**oDOSGetSupportedTokens**](OdosApi.md#oDOSGetSupportedTokens) | **GET** /odos/supported-tokens |  |
| [**oDOSSwapTokens**](OdosApi.md#oDOSSwapTokens) | **POST** /odos/{accountName}/swap |  |
| [**zap**](OdosApi.md#zap) | **POST** /odos/{accountName}/zap |  |


<a name="getZapQuote"></a>
# **getZapQuote**
> OdosAPIResponse_OdosExecuteFunctionResult_ getZapQuote(accountName, Authorization, OdosSwapInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **accountName** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **OdosSwapInputBody** | [**OdosSwapInputBody**](../Models/OdosSwapInputBody.md)|  | |

### Return type

[**OdosAPIResponse_OdosExecuteFunctionResult_**](../Models/OdosAPIResponse_OdosExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="oDOSAssembleTransaction"></a>
# **oDOSAssembleTransaction**
> OdosAPIResponse_OdosExecuteFunctionResult_ oDOSAssembleTransaction(Authorization, AssembleRequest)



    Assembles a transaction using the provided authorization token and request body.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**| - The authorization token from the request header. | [default to null] |
| **AssembleRequest** | [**AssembleRequest**](../Models/AssembleRequest.md)| - The request body containing the transaction details. | |

### Return type

[**OdosAPIResponse_OdosExecuteFunctionResult_**](../Models/OdosAPIResponse_OdosExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="oDOSGetContractInfo"></a>
# **oDOSGetContractInfo**
> OdosAPIResponse_OdosExecuteFunctionResult_ oDOSGetContractInfo(Authorization, version, chainId)



    Retrieves contract information from the Odos API.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**| - The authorization token from the request header. | [default to null] |
| **version** | **String**| - The version of the API to use, expected to be &#39;v2&#39;. | [default to null] [enum: v2] |
| **chainId** | **Double**| - The chain ID for which the contract information is requested. | [default to null] |

### Return type

[**OdosAPIResponse_OdosExecuteFunctionResult_**](../Models/OdosAPIResponse_OdosExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="oDOSGetCurrentBlock"></a>
# **oDOSGetCurrentBlock**
> OdosAPIResponse_OdosExecuteFunctionResult_ oDOSGetCurrentBlock(Authorization, chainId)



    Retrieves the current block information for a given blockchain.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**| - The authorization token from the request header. | [default to null] |
| **chainId** | **Double**| - The ID of the blockchain to query. | [default to null] |

### Return type

[**OdosAPIResponse_OdosExecuteFunctionResult_**](../Models/OdosAPIResponse_OdosExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="oDOSGetExecutorAddress"></a>
# **oDOSGetExecutorAddress**
> OdosAPIResponse_OdosExecuteFunctionResult_ oDOSGetExecutorAddress(Authorization, version, chainId)



    Retrieves the executor address from the Odos API.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**| - The authorization token from the request header. | [default to null] |
| **version** | **String**| - The API version, expected to be &#39;v2&#39;. | [default to null] [enum: v2] |
| **chainId** | **Double**| - The chain ID for which the executor address is requested. | [default to null] |

### Return type

[**OdosAPIResponse_OdosExecuteFunctionResult_**](../Models/OdosAPIResponse_OdosExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="oDOSGetLiquiditySources"></a>
# **oDOSGetLiquiditySources**
> OdosAPIResponse_OdosExecuteFunctionResult_ oDOSGetLiquiditySources(Authorization, chainId)



    Retrieves liquidity sources for a given chain ID.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**| - The authorization token from the request header. | [default to null] |
| **chainId** | **Double**| - The ID of the blockchain to query for liquidity sources. | [default to null] |

### Return type

[**OdosAPIResponse_OdosExecuteFunctionResult_**](../Models/OdosAPIResponse_OdosExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="oDOSGetQuote"></a>
# **oDOSGetQuote**
> OdosAPIResponse_OdosExecuteFunctionResult_ oDOSGetQuote(accountName, Authorization, OdosSwapInputBody)



    Retrieves a quote for a given account and input body.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **accountName** | **String**| - The name of the account for which the quote is being retrieved. | [default to null] |
| **Authorization** | **String**| - The authorization token for the request. | [default to null] |
| **OdosSwapInputBody** | [**OdosSwapInputBody**](../Models/OdosSwapInputBody.md)| - The input body containing the details for the quote request. | |

### Return type

[**OdosAPIResponse_OdosExecuteFunctionResult_**](../Models/OdosAPIResponse_OdosExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="oDOSGetRouterAddress"></a>
# **oDOSGetRouterAddress**
> OdosAPIResponse_OdosExecuteFunctionResult_ oDOSGetRouterAddress(Authorization, version, chainId)



    Retrieves the router address for the specified version and chain ID.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**| - The authorization token from the request header. | [default to null] |
| **version** | **String**| - The version of the API to use, default is &#39;v2&#39;. | [default to null] [enum: v2] |
| **chainId** | **Double**| - The ID of the blockchain network. | [default to null] |

### Return type

[**OdosAPIResponse_OdosExecuteFunctionResult_**](../Models/OdosAPIResponse_OdosExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="oDOSGetSupportedChains"></a>
# **oDOSGetSupportedChains**
> OdosAPIResponse_OdosExecuteFunctionResult_ oDOSGetSupportedChains(Authorization)



    Retrieves the supported blockchain networks from the Odos API.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**| - The authorization token provided in the request header. | [default to null] |

### Return type

[**OdosAPIResponse_OdosExecuteFunctionResult_**](../Models/OdosAPIResponse_OdosExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="oDOSGetSupportedTokens"></a>
# **oDOSGetSupportedTokens**
> OdosAPIResponse_OdosExecuteFunctionResult_ oDOSGetSupportedTokens(Authorization, chainId)



    Retrieves the supported tokens for a given blockchain network.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**| - The authorization token from the request header. | [default to null] |
| **chainId** | **Double**| - The ID of the blockchain network to query. | [default to null] |

### Return type

[**OdosAPIResponse_OdosExecuteFunctionResult_**](../Models/OdosAPIResponse_OdosExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="oDOSSwapTokens"></a>
# **oDOSSwapTokens**
> OdosAPIResponse_OdosExecuteFunctionResult_ oDOSSwapTokens(accountName, Authorization, OdosSwapInputBody)



    Handles the swap operation for the given account.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **accountName** | **String**| - The name of the account to perform the swap for. | [default to null] |
| **Authorization** | **String**| - The authorization token for the request. | [default to null] |
| **OdosSwapInputBody** | [**OdosSwapInputBody**](../Models/OdosSwapInputBody.md)| - The input body containing the swap details. | |

### Return type

[**OdosAPIResponse_OdosExecuteFunctionResult_**](../Models/OdosAPIResponse_OdosExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="zap"></a>
# **zap**
> OdosAPIResponse_OdosExecuteFunctionResult_ zap(accountName, Authorization, OdosSwapInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **accountName** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **OdosSwapInputBody** | [**OdosSwapInputBody**](../Models/OdosSwapInputBody.md)|  | |

### Return type

[**OdosAPIResponse_OdosExecuteFunctionResult_**](../Models/OdosAPIResponse_OdosExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

