# DataApi

All URIs are relative to *https://beta.usemoon.ai*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**chartsGetChartAnalysis**](DataApi.md#chartsGetChartAnalysis) | **GET** /data/analysis/{symbol}/{timeframe} |  |
| [**dataExecuteCustomSupabaseQuery**](DataApi.md#dataExecuteCustomSupabaseQuery) | **POST** /data/query |  |
| [**dataGetPortfolioFetchStatus**](DataApi.md#dataGetPortfolioFetchStatus) | **GET** /data/portfolio/status/{jobId} |  |
| [**dataGetTokensMetadata**](DataApi.md#dataGetTokensMetadata) | **GET** /data/token-metadata |  |
| [**dataGetUserDebankComplexProtocolList**](DataApi.md#dataGetUserDebankComplexProtocolList) | **GET** /data/{address}/debank/complex-protocols |  |
| [**dataGetUserDebankTokenList**](DataApi.md#dataGetUserDebankTokenList) | **GET** /data/{address}/debank/tokens |  |
| [**dataGetUserDebankTotalBalance**](DataApi.md#dataGetUserDebankTotalBalance) | **GET** /data/{address}/debank/total-balance |  |
| [**dataGetUserWalletPortfolio**](DataApi.md#dataGetUserWalletPortfolio) | **GET** /data/{address}/portfolio |  |
| [**dataGetWalletNFTs**](DataApi.md#dataGetWalletNFTs) | **GET** /data/{address}/nfts |  |
| [**dataGetWalletTokenBalances**](DataApi.md#dataGetWalletTokenBalances) | **GET** /data/{address}/balance |  |
| [**dataGetWalletTransactionHistory**](DataApi.md#dataGetWalletTransactionHistory) | **GET** /data/{address}/history |  |
| [**getAllDebankUserTokens**](DataApi.md#getAllDebankUserTokens) | **GET** /data/{address}/debank/all-tokens |  |


<a name="chartsGetChartAnalysis"></a>
# **chartsGetChartAnalysis**
> ChartAnalysisAPIResponse chartsGetChartAnalysis(symbol, Authorization, timeframe)



    Retrieves the chart analysis for a given trading symbol and timeframe.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **symbol** | **String**| - The trading view symbol for which the chart analysis is requested. | [default to null] |
| **Authorization** | **String**| - The authorization token for the request. | [default to null] |
| **timeframe** | **String**| - The timeframe for the chart analysis. Defaults to \&quot;1D\&quot;. Can be \&quot;1D\&quot;, \&quot;4H\&quot;, or \&quot;1H\&quot;. | [default to 1D] [enum: 1D, 4H, 1H, 15m] |

### Return type

[**ChartAnalysisAPIResponse**](../Models/ChartAnalysisAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="dataExecuteCustomSupabaseQuery"></a>
# **dataExecuteCustomSupabaseQuery**
> oas_any_type_not_mapped dataExecuteCustomSupabaseQuery(Authorization, body)



    Executes a query using the LLMSupabaseQueryGenerator and returns the result.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**| - The authorization token for the request. | [default to null] |
| **body** | **String**| - The query string to be executed. | |

### Return type

[**oas_any_type_not_mapped**](../Models/AnyType.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="dataGetPortfolioFetchStatus"></a>
# **dataGetPortfolioFetchStatus**
> PortfolioAPIResponse dataGetPortfolioFetchStatus(jobId, Authorization)



    Retrieves the status of a portfolio job.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **jobId** | **String**| - The ID of the job to retrieve the status for. | [default to null] |
| **Authorization** | **String**| - The authorization token. | [default to null] |

### Return type

[**PortfolioAPIResponse**](../Models/PortfolioAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="dataGetTokensMetadata"></a>
# **dataGetTokensMetadata**
> TokenMetadataAPIResponse dataGetTokensMetadata(Authorization, chain, addresses)



    Retrieves token metadata from the Moralis service.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**| - The authorization token from the request header. | [default to null] |
| **chain** | **String**| - The blockchain network identifier. | [default to null] |
| **addresses** | [**List**](../Models/String.md)| - An array of token addresses to fetch metadata for. | [default to null] |

### Return type

[**TokenMetadataAPIResponse**](../Models/TokenMetadataAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="dataGetUserDebankComplexProtocolList"></a>
# **dataGetUserDebankComplexProtocolList**
> DebankPortfolioAPIResponse dataGetUserDebankComplexProtocolList(address, Authorization, refresh)



    Retrieves the user&#39;s complex protocol list from Debank, with Supabase caching.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**| - The wallet address of the user. | [default to null] |
| **Authorization** | **String**| - The authorization token. | [default to null] |
| **refresh** | **Boolean**|  | [optional] [default to null] |

### Return type

[**DebankPortfolioAPIResponse**](../Models/DebankPortfolioAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="dataGetUserDebankTokenList"></a>
# **dataGetUserDebankTokenList**
> WalletBalanceAPIResponse dataGetUserDebankTokenList(address, Authorization, chainId, refresh)



    Retrieves the user&#39;s token list from Debank, with Supabase caching.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**| - The wallet address of the user. | [default to null] |
| **Authorization** | **String**| - The authorization token. | [default to null] |
| **chainId** | **String**| - The chain ID to fetch tokens for. | [default to null] |
| **refresh** | **Boolean**|  | [optional] [default to null] |

### Return type

[**WalletBalanceAPIResponse**](../Models/WalletBalanceAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="dataGetUserDebankTotalBalance"></a>
# **dataGetUserDebankTotalBalance**
> DebankPortfolioAPIResponse dataGetUserDebankTotalBalance(address, Authorization, refresh)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **refresh** | **Boolean**|  | [optional] [default to null] |

### Return type

[**DebankPortfolioAPIResponse**](../Models/DebankPortfolioAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="dataGetUserWalletPortfolio"></a>
# **dataGetUserWalletPortfolio**
> PortfolioAPIResponse dataGetUserWalletPortfolio(address, Authorization, page, pageSize)



    Retrieves the user&#39;s portfolio based on the provided wallet address.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**| - The wallet address of the user. | [default to null] |
| **Authorization** | **String**| - The authorization token. | [default to null] |
| **page** | **Double**| - The page number for pagination (default is 1). | [optional] [default to 1] |
| **pageSize** | **Double**| - The number of items per page for pagination (default is 100). | [optional] [default to 100] |

### Return type

[**PortfolioAPIResponse**](../Models/PortfolioAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="dataGetWalletNFTs"></a>
# **dataGetWalletNFTs**
> NFTsAPIResponse dataGetWalletNFTs(address, Authorization, chain)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **chain** | **String**|  | [default to null] |

### Return type

[**NFTsAPIResponse**](../Models/NFTsAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="dataGetWalletTokenBalances"></a>
# **dataGetWalletTokenBalances**
> WalletBalanceAPIResponse dataGetWalletTokenBalances(address, Authorization, chain, excludeNative)



    Retrieves the wallet balance for a given address.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**| - The wallet address to retrieve the balance for. | [default to null] |
| **Authorization** | **String**| - The authorization token. | [default to null] |
| **chain** | **String**| - The blockchain network to query. | [default to null] |
| **excludeNative** | **Boolean**| - Optional flag to exclude native currency from the balance. | [optional] [default to null] |

### Return type

[**WalletBalanceAPIResponse**](../Models/WalletBalanceAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="dataGetWalletTransactionHistory"></a>
# **dataGetWalletTransactionHistory**
> WalletHistoryAPIResponse dataGetWalletTransactionHistory(address, Authorization, chain)



    Retrieves the wallet history for a given address and blockchain chain.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**| - The wallet address to retrieve history for. | [default to null] |
| **Authorization** | **String**| - The authorization token for the request. | [default to null] |
| **chain** | **String**| - The blockchain chain to retrieve history from. | [default to null] |

### Return type

[**WalletHistoryAPIResponse**](../Models/WalletHistoryAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getAllDebankUserTokens"></a>
# **getAllDebankUserTokens**
> GetAllDebankUserTokens_200_response getAllDebankUserTokens(address, Authorization, isAll, refresh)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **isAll** | **Boolean**|  | [default to null] |
| **refresh** | **Boolean**|  | [optional] [default to null] |

### Return type

[**GetAllDebankUserTokens_200_response**](../Models/GetAllDebankUserTokens_200_response.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

