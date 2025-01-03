# PoolAddressProviderApi

All URIs are relative to *https://beta.usemoon.ai*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**aavev3PoolAddressProviderGetACLAdmin**](PoolAddressProviderApi.md#aavev3PoolAddressProviderGetACLAdmin) | **GET** /aave/v3/poolAddressProvider/{account}/getACLAdmin |  |
| [**aavev3PoolAddressProviderGetACLManager**](PoolAddressProviderApi.md#aavev3PoolAddressProviderGetACLManager) | **GET** /aave/v3/poolAddressProvider/{account}/getACLManager |  |
| [**aavev3PoolAddressProviderGetAddress**](PoolAddressProviderApi.md#aavev3PoolAddressProviderGetAddress) | **GET** /aave/v3/poolAddressProvider/{account}/getAddress |  |
| [**aavev3PoolAddressProviderGetMarketId**](PoolAddressProviderApi.md#aavev3PoolAddressProviderGetMarketId) | **GET** /aave/v3/poolAddressProvider/{account}/getMarketId |  |
| [**aavev3PoolAddressProviderGetPool**](PoolAddressProviderApi.md#aavev3PoolAddressProviderGetPool) | **GET** /aave/v3/poolAddressProvider/{account}/getPool |  |
| [**aavev3PoolAddressProviderGetPoolConfigurator**](PoolAddressProviderApi.md#aavev3PoolAddressProviderGetPoolConfigurator) | **GET** /aave/v3/poolAddressProvider/{account}/getPoolConfigurator |  |
| [**aavev3PoolAddressProviderGetPriceOracle**](PoolAddressProviderApi.md#aavev3PoolAddressProviderGetPriceOracle) | **GET** /aave/v3/poolAddressProvider/{account}/getPriceOracle |  |
| [**aavev3PoolAddressProviderSetACLAdmin**](PoolAddressProviderApi.md#aavev3PoolAddressProviderSetACLAdmin) | **POST** /aave/v3/poolAddressProvider/{address}/setACLAdmin |  |
| [**aavev3PoolAddressProviderSetACLManager**](PoolAddressProviderApi.md#aavev3PoolAddressProviderSetACLManager) | **POST** /aave/v3/poolAddressProvider/{address}/setACLManager |  |
| [**aavev3PoolAddressProviderSetAddress**](PoolAddressProviderApi.md#aavev3PoolAddressProviderSetAddress) | **POST** /aave/v3/poolAddressProvider/{address}/setAddress |  |
| [**aavev3PoolAddressProviderSetMarketId**](PoolAddressProviderApi.md#aavev3PoolAddressProviderSetMarketId) | **POST** /aave/v3/poolAddressProvider/{address}/setMarketId |  |
| [**aavev3PoolAddressProviderSetPoolConfiguratorImpl**](PoolAddressProviderApi.md#aavev3PoolAddressProviderSetPoolConfiguratorImpl) | **POST** /aave/v3/poolAddressProvider/{address}/setPoolConfiguratorImpl |  |
| [**aavev3PoolAddressProviderSetPoolImpl**](PoolAddressProviderApi.md#aavev3PoolAddressProviderSetPoolImpl) | **POST** /aave/v3/poolAddressProvider/{address}/setPoolImpl |  |


<a name="aavev3PoolAddressProviderGetACLAdmin"></a>
# **aavev3PoolAddressProviderGetACLAdmin**
> PoolAddressProviderAPIResponse_string_ aavev3PoolAddressProviderGetACLAdmin(account, Authorization, chainId, address)



    Retrieves the ACL (Access Control List) admin address for a given account.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **account** | **String**| - The account address to query. | [default to null] |
| **Authorization** | **String**| - The authorization token for the request. | [default to null] |
| **chainId** | **String**| - The chain ID of the blockchain network. | [default to null] |
| **address** | **String**| - The address of the pool address provider. | [default to null] |

### Return type

[**PoolAddressProviderAPIResponse_string_**](../Models/PoolAddressProviderAPIResponse_string_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="aavev3PoolAddressProviderGetACLManager"></a>
# **aavev3PoolAddressProviderGetACLManager**
> PoolAddressProviderAPIResponse_string_ aavev3PoolAddressProviderGetACLManager(account, Authorization, chainId, address)



    Retrieves the ACL Manager address from the Pool Address Provider.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **account** | **String**| - The account path parameter. | [default to null] |
| **Authorization** | **String**| - The authorization token from the request header. | [default to null] |
| **chainId** | **String**| - The chain ID query parameter. | [default to null] |
| **address** | **String**| - The address query parameter. | [default to null] |

### Return type

[**PoolAddressProviderAPIResponse_string_**](../Models/PoolAddressProviderAPIResponse_string_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="aavev3PoolAddressProviderGetAddress"></a>
# **aavev3PoolAddressProviderGetAddress**
> PoolAddressProviderAPIResponse_string_ aavev3PoolAddressProviderGetAddress(account, Authorization, chainId, address, id)



    Retrieves an address from the Pool Address Provider.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **account** | **String**| - The account path parameter. | [default to null] |
| **Authorization** | **String**| - The authorization token from the request header. | [default to null] |
| **chainId** | **String**| - The chain ID from the query parameters. | [default to null] |
| **address** | **String**| - The address from the query parameters. | [default to null] |
| **id** | **String**| - The ID from the query parameters. | [default to null] |

### Return type

[**PoolAddressProviderAPIResponse_string_**](../Models/PoolAddressProviderAPIResponse_string_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="aavev3PoolAddressProviderGetMarketId"></a>
# **aavev3PoolAddressProviderGetMarketId**
> PoolAddressProviderAPIResponse_string_ aavev3PoolAddressProviderGetMarketId(account, Authorization, chainId, address)



    Retrieves the market ID from the Pool Address Provider.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **account** | **String**| - The account path parameter. | [default to null] |
| **Authorization** | **String**| - The authorization token from the request header. | [default to null] |
| **chainId** | **String**| - The chain ID from the query parameters. | [default to null] |
| **address** | **String**| - The address from the query parameters. | [default to null] |

### Return type

[**PoolAddressProviderAPIResponse_string_**](../Models/PoolAddressProviderAPIResponse_string_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="aavev3PoolAddressProviderGetPool"></a>
# **aavev3PoolAddressProviderGetPool**
> PoolAddressProviderAPIResponse_string_ aavev3PoolAddressProviderGetPool(account, Authorization, chainId, address)



    Retrieves the pool address from the Aave protocol.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **account** | **String**| - The account identifier. | [default to null] |
| **Authorization** | **String**| - The authorization token. | [default to null] |
| **chainId** | **String**| - The blockchain network identifier. | [default to null] |
| **address** | **String**| - The address to query. | [default to null] |

### Return type

[**PoolAddressProviderAPIResponse_string_**](../Models/PoolAddressProviderAPIResponse_string_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="aavev3PoolAddressProviderGetPoolConfigurator"></a>
# **aavev3PoolAddressProviderGetPoolConfigurator**
> PoolAddressProviderAPIResponse_string_ aavev3PoolAddressProviderGetPoolConfigurator(account, Authorization, chainId, address)



    Retrieves the pool configurator for a given account.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **account** | **String**| - The account identifier. | [default to null] |
| **Authorization** | **String**| - The authorization token. | [default to null] |
| **chainId** | **String**| - The chain identifier. | [default to null] |
| **address** | **String**| - The address of the pool. | [default to null] |

### Return type

[**PoolAddressProviderAPIResponse_string_**](../Models/PoolAddressProviderAPIResponse_string_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="aavev3PoolAddressProviderGetPriceOracle"></a>
# **aavev3PoolAddressProviderGetPriceOracle**
> PoolAddressProviderAPIResponse_string_ aavev3PoolAddressProviderGetPriceOracle(account, Authorization, chainId, address)



    Retrieves the price oracle address from the Aave pool address provider.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **account** | **String**| - The account identifier. | [default to null] |
| **Authorization** | **String**| - The authorization token. | [default to null] |
| **chainId** | **String**| - The blockchain chain identifier. | [default to null] |
| **address** | **String**| - The address of the pool address provider. | [default to null] |

### Return type

[**PoolAddressProviderAPIResponse_string_**](../Models/PoolAddressProviderAPIResponse_string_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="aavev3PoolAddressProviderSetACLAdmin"></a>
# **aavev3PoolAddressProviderSetACLAdmin**
> PoolAddressProviderAPIResponse_PoolAddressProviderExecuteFunctionResult_ aavev3PoolAddressProviderSetACLAdmin(address, Authorization, PoolAddressProviderInputBody)



    Sets the ACL (Access Control List) admin for the specified address.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**| - The address for which the ACL admin is being set. | [default to null] |
| **Authorization** | **String**| - The authorization token for the request. | [default to null] |
| **PoolAddressProviderInputBody** | [**PoolAddressProviderInputBody**](../Models/PoolAddressProviderInputBody.md)| - The body of the request containing additional parameters. | |

### Return type

[**PoolAddressProviderAPIResponse_PoolAddressProviderExecuteFunctionResult_**](../Models/PoolAddressProviderAPIResponse_PoolAddressProviderExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="aavev3PoolAddressProviderSetACLManager"></a>
# **aavev3PoolAddressProviderSetACLManager**
> PoolAddressProviderAPIResponse_PoolAddressProviderExecuteFunctionResult_ aavev3PoolAddressProviderSetACLManager(address, Authorization, PoolAddressProviderInputBody)



    Sets the ACL Manager for the specified pool address provider.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**| - The address of the pool address provider. | [default to null] |
| **Authorization** | **String**| - The authorization token. | [default to null] |
| **PoolAddressProviderInputBody** | [**PoolAddressProviderInputBody**](../Models/PoolAddressProviderInputBody.md)| - The input body containing the chain ID and other necessary information. | |

### Return type

[**PoolAddressProviderAPIResponse_PoolAddressProviderExecuteFunctionResult_**](../Models/PoolAddressProviderAPIResponse_PoolAddressProviderExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="aavev3PoolAddressProviderSetAddress"></a>
# **aavev3PoolAddressProviderSetAddress**
> PoolAddressProviderAPIResponse_PoolAddressProviderExecuteFunctionResult_ aavev3PoolAddressProviderSetAddress(address, Authorization, PoolAddressProviderInputBody)



    Sets the address for the Pool Address Provider.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**| - The address to be set. | [default to null] |
| **Authorization** | **String**| - The authorization token. | [default to null] |
| **PoolAddressProviderInputBody** | [**PoolAddressProviderInputBody**](../Models/PoolAddressProviderInputBody.md)| - The body containing the chain ID and other necessary information. | |

### Return type

[**PoolAddressProviderAPIResponse_PoolAddressProviderExecuteFunctionResult_**](../Models/PoolAddressProviderAPIResponse_PoolAddressProviderExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="aavev3PoolAddressProviderSetMarketId"></a>
# **aavev3PoolAddressProviderSetMarketId**
> PoolAddressProviderAPIResponse_PoolAddressProviderExecuteFunctionResult_ aavev3PoolAddressProviderSetMarketId(address, Authorization, PoolAddressProviderInputBody)



    Sets the market ID for the given pool address provider.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**| - The address of the pool address provider. | [default to null] |
| **Authorization** | **String**| - The authorization token. | [default to null] |
| **PoolAddressProviderInputBody** | [**PoolAddressProviderInputBody**](../Models/PoolAddressProviderInputBody.md)| - The input body containing the chain ID and other necessary information. | |

### Return type

[**PoolAddressProviderAPIResponse_PoolAddressProviderExecuteFunctionResult_**](../Models/PoolAddressProviderAPIResponse_PoolAddressProviderExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="aavev3PoolAddressProviderSetPoolConfiguratorImpl"></a>
# **aavev3PoolAddressProviderSetPoolConfiguratorImpl**
> PoolAddressProviderAPIResponse_PoolAddressProviderExecuteFunctionResult_ aavev3PoolAddressProviderSetPoolConfiguratorImpl(address, Authorization, PoolAddressProviderInputBody)



    Sets the Pool Configurator implementation for the given address.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**| - The address of the pool. | [default to null] |
| **Authorization** | **String**| - The authorization token. | [default to null] |
| **PoolAddressProviderInputBody** | [**PoolAddressProviderInputBody**](../Models/PoolAddressProviderInputBody.md)| - The body containing the pool address provider input data. | |

### Return type

[**PoolAddressProviderAPIResponse_PoolAddressProviderExecuteFunctionResult_**](../Models/PoolAddressProviderAPIResponse_PoolAddressProviderExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="aavev3PoolAddressProviderSetPoolImpl"></a>
# **aavev3PoolAddressProviderSetPoolImpl**
> PoolAddressProviderAPIResponse_PoolAddressProviderExecuteFunctionResult_ aavev3PoolAddressProviderSetPoolImpl(address, Authorization, PoolAddressProviderInputBody)



    Sets the pool implementation address for the given address.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**| - The address of the pool. | [default to null] |
| **Authorization** | **String**| - The authorization token. | [default to null] |
| **PoolAddressProviderInputBody** | [**PoolAddressProviderInputBody**](../Models/PoolAddressProviderInputBody.md)| - The body containing the pool address provider input data. | |

### Return type

[**PoolAddressProviderAPIResponse_PoolAddressProviderExecuteFunctionResult_**](../Models/PoolAddressProviderAPIResponse_PoolAddressProviderExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

