# PoolAddressProviderRegistryApi

All URIs are relative to *https://beta.usemoon.ai*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**aavev3PoolAddressProviderRegistryGetATokenTotalSupply**](PoolAddressProviderRegistryApi.md#aavev3PoolAddressProviderRegistryGetATokenTotalSupply) | **GET** /aave/v3/poolAddressProviderRegistry/{account}/getATokenTotalSupply |  |
| [**aavev3PoolAddressProviderRegistryGetAddressesProvider**](PoolAddressProviderRegistryApi.md#aavev3PoolAddressProviderRegistryGetAddressesProvider) | **GET** /aave/v3/poolAddressProviderRegistry/{account}/getAddressesProvider |  |
| [**aavev3PoolAddressProviderRegistryGetAllATokens**](PoolAddressProviderRegistryApi.md#aavev3PoolAddressProviderRegistryGetAllATokens) | **GET** /aave/v3/poolAddressProviderRegistry/{account}/getAllATokens |  |
| [**aavev3PoolAddressProviderRegistryGetDebtCeiling**](PoolAddressProviderRegistryApi.md#aavev3PoolAddressProviderRegistryGetDebtCeiling) | **GET** /aave/v3/poolAddressProviderRegistry/{account}/getDebtCeiling |  |
| [**getAllReservesTokens**](PoolAddressProviderRegistryApi.md#getAllReservesTokens) | **GET** /aave/v3/poolAddressProviderRegistry/{account}/getAllReservesTokens |  |


<a name="aavev3PoolAddressProviderRegistryGetATokenTotalSupply"></a>
# **aavev3PoolAddressProviderRegistryGetATokenTotalSupply**
> PoolAddressProviderRegistryAPIResponse_string_ aavev3PoolAddressProviderRegistryGetATokenTotalSupply(account, Authorization, chainId, address, asset)



    Retrieves the total supply of a specific AToken.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **account** | **String**| - The account address. | [default to null] |
| **Authorization** | **String**| - The authorization token. | [default to null] |
| **chainId** | **String**| - The chain ID. | [default to null] |
| **address** | **String**| - The address of the pool address provider registry. | [default to null] |
| **asset** | **String**| - The asset for which to get the total supply. | [default to null] |

### Return type

[**PoolAddressProviderRegistryAPIResponse_string_**](../Models/PoolAddressProviderRegistryAPIResponse_string_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="aavev3PoolAddressProviderRegistryGetAddressesProvider"></a>
# **aavev3PoolAddressProviderRegistryGetAddressesProvider**
> PoolAddressProviderRegistryAPIResponse_string_ aavev3PoolAddressProviderRegistryGetAddressesProvider(account, Authorization, chainId, address)



    Retrieves the addresses provider from the Aave V3 Pool Address Provider Registry.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **account** | **String**| - The account identifier. | [default to null] |
| **Authorization** | **String**| - The authorization token. | [default to null] |
| **chainId** | **String**| - The blockchain chain identifier. | [default to null] |
| **address** | **String**| - The address of the registry. | [default to null] |

### Return type

[**PoolAddressProviderRegistryAPIResponse_string_**](../Models/PoolAddressProviderRegistryAPIResponse_string_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="aavev3PoolAddressProviderRegistryGetAllATokens"></a>
# **aavev3PoolAddressProviderRegistryGetAllATokens**
> PoolAddressProviderRegistryAPIResponse_any-Array_ aavev3PoolAddressProviderRegistryGetAllATokens(account, Authorization, chainId, address)



    Retrieves all ATokens associated with the specified account.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **account** | **String**| - The account identifier. | [default to null] |
| **Authorization** | **String**| - The authorization token. | [default to null] |
| **chainId** | **String**| - The blockchain chain identifier. | [default to null] |
| **address** | **String**| - The address to query. | [default to null] |

### Return type

[**PoolAddressProviderRegistryAPIResponse_any-Array_**](../Models/PoolAddressProviderRegistryAPIResponse_any-Array_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="aavev3PoolAddressProviderRegistryGetDebtCeiling"></a>
# **aavev3PoolAddressProviderRegistryGetDebtCeiling**
> PoolAddressProviderRegistryAPIResponse_string_ aavev3PoolAddressProviderRegistryGetDebtCeiling(account, Authorization, chainId, address, asset)



    Retrieves the debt ceiling for a specified asset from the Aave V3 Pool Address Provider Registry.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **account** | **String**| - The account identifier. | [default to null] |
| **Authorization** | **String**| - The authorization token. | [default to null] |
| **chainId** | **String**| - The blockchain chain identifier. | [default to null] |
| **address** | **String**| - The address of the Pool Address Provider Registry. | [default to null] |
| **asset** | **String**| - The asset for which to retrieve the debt ceiling. | [default to null] |

### Return type

[**PoolAddressProviderRegistryAPIResponse_string_**](../Models/PoolAddressProviderRegistryAPIResponse_string_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getAllReservesTokens"></a>
# **getAllReservesTokens**
> PoolAddressProviderRegistryAPIResponse_any-Array_ getAllReservesTokens(account, Authorization, chainId, address)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **account** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |

### Return type

[**PoolAddressProviderRegistryAPIResponse_any-Array_**](../Models/PoolAddressProviderRegistryAPIResponse_any-Array_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

