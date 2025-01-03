# AAVEV3UIPoolDataProviderApi

All URIs are relative to *https://beta.usemoon.ai*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**aaveV3UiPoolDataProviderEthCurrencyUnit**](AAVEV3UIPoolDataProviderApi.md#aaveV3UiPoolDataProviderEthCurrencyUnit) | **GET** /aave/v3/pool-data/eth-currency-unit |  |
| [**aaveV3UiPoolDataProviderMarketReferenceCurrencyPriceInUsdProxyAggregator**](AAVEV3UIPoolDataProviderApi.md#aaveV3UiPoolDataProviderMarketReferenceCurrencyPriceInUsdProxyAggregator) | **GET** /aave/v3/pool-data/market-reference-currency-price-in-usd-proxy-aggregator |  |
| [**aaveV3UiPoolDataProviderNetworkBaseTokenPriceInUsdProxyAggregator**](AAVEV3UIPoolDataProviderApi.md#aaveV3UiPoolDataProviderNetworkBaseTokenPriceInUsdProxyAggregator) | **GET** /aave/v3/pool-data/network-base-token-price-in-usd-proxy-aggregator |  |
| [**aaveV3UiPoolDataProviderReservesList**](AAVEV3UIPoolDataProviderApi.md#aaveV3UiPoolDataProviderReservesList) | **GET** /aave/v3/pool-data/reserves-list |  |
| [**aaveV3UiPoolDataProviderUserReservesData**](AAVEV3UIPoolDataProviderApi.md#aaveV3UiPoolDataProviderUserReservesData) | **GET** /aave/v3/pool-data/user-reserves-data |  |
| [**getReservesData**](AAVEV3UIPoolDataProviderApi.md#getReservesData) | **GET** /aave/v3/pool-data/reserves-data |  |


<a name="aaveV3UiPoolDataProviderEthCurrencyUnit"></a>
# **aaveV3UiPoolDataProviderEthCurrencyUnit**
> AAVEv3UiPoolDataProviderAPIResponse_string_ aaveV3UiPoolDataProviderEthCurrencyUnit(Authorization, contract\_address, chain\_id)



    Retrieves the ETH currency unit from the AAVE V3 UI Pool Data Provider.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**| - The authorization token for the request. | [default to null] |
| **contract\_address** | **String**| - The contract address to query. | [default to null] |
| **chain\_id** | **String**| - The chain ID to query. | [default to null] |

### Return type

[**AAVEv3UiPoolDataProviderAPIResponse_string_**](../Models/AAVEv3UiPoolDataProviderAPIResponse_string_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="aaveV3UiPoolDataProviderMarketReferenceCurrencyPriceInUsdProxyAggregator"></a>
# **aaveV3UiPoolDataProviderMarketReferenceCurrencyPriceInUsdProxyAggregator**
> AAVEv3UiPoolDataProviderAPIResponse_string_ aaveV3UiPoolDataProviderMarketReferenceCurrencyPriceInUsdProxyAggregator(Authorization, contract\_address, chain\_id)



    Retrieves the market reference currency price in USD using the proxy aggregator.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**| - The authorization token. | [default to null] |
| **contract\_address** | **String**| - The contract address to query. | [default to null] |
| **chain\_id** | **String**| - The chain ID to query. | [default to null] |

### Return type

[**AAVEv3UiPoolDataProviderAPIResponse_string_**](../Models/AAVEv3UiPoolDataProviderAPIResponse_string_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="aaveV3UiPoolDataProviderNetworkBaseTokenPriceInUsdProxyAggregator"></a>
# **aaveV3UiPoolDataProviderNetworkBaseTokenPriceInUsdProxyAggregator**
> AAVEv3UiPoolDataProviderAPIResponse_string_ aaveV3UiPoolDataProviderNetworkBaseTokenPriceInUsdProxyAggregator(Authorization, contract\_address, chain\_id)



     Retrieves the network base token price in USD using the proxy aggregator.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**| - The authorization token. | [default to null] |
| **contract\_address** | **String**| - The contract address to query. | [default to null] |
| **chain\_id** | **String**| - The chain ID to query. | [default to null] |

### Return type

[**AAVEv3UiPoolDataProviderAPIResponse_string_**](../Models/AAVEv3UiPoolDataProviderAPIResponse_string_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="aaveV3UiPoolDataProviderReservesList"></a>
# **aaveV3UiPoolDataProviderReservesList**
> AAVEv3UiPoolDataProviderAPIResponse_string-Array_ aaveV3UiPoolDataProviderReservesList(Authorization, contract\_address, chain\_id, provider)



    Retrieves the list of reserves from the AAVE V3 UI Pool Data Provider.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**| - The authorization token. | [default to null] |
| **contract\_address** | **String**| - The contract address to query. | [default to null] |
| **chain\_id** | **String**| - The chain ID to query. | [default to null] |
| **provider** | **String**| - The provider to use for querying the reserves list. | [default to null] |

### Return type

[**AAVEv3UiPoolDataProviderAPIResponse_string-Array_**](../Models/AAVEv3UiPoolDataProviderAPIResponse_string-Array_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="aaveV3UiPoolDataProviderUserReservesData"></a>
# **aaveV3UiPoolDataProviderUserReservesData**
> AAVEv3UiPoolDataProviderAPIResponse_UserReserveData-Array_ aaveV3UiPoolDataProviderUserReservesData(Authorization, contract\_address, chain\_id, provider, user)



    Retrieves the user&#39;s reserve data from the AAVE v3 UI Pool Data Provider.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**| - The authorization token. | [default to null] |
| **contract\_address** | **String**| - The contract address of the AAVE v3 UI Pool Data Provider. | [default to null] |
| **chain\_id** | **String**| - The chain ID where the contract is deployed. | [default to null] |
| **provider** | **String**| - The provider address. | [default to null] |
| **user** | **String**| - The user address whose reserve data is to be fetched. | [default to null] |

### Return type

[**AAVEv3UiPoolDataProviderAPIResponse_UserReserveData-Array_**](../Models/AAVEv3UiPoolDataProviderAPIResponse_UserReserveData-Array_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getReservesData"></a>
# **getReservesData**
> AAVEv3UiPoolDataProviderAPIResponse_any_ getReservesData(Authorization, contract\_address, chain\_id, provider)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **contract\_address** | **String**|  | [default to null] |
| **chain\_id** | **String**|  | [default to null] |
| **provider** | **String**|  | [default to null] |

### Return type

[**AAVEv3UiPoolDataProviderAPIResponse_any_**](../Models/AAVEv3UiPoolDataProviderAPIResponse_any_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

