# AAVEv3PoolApi

All URIs are relative to *https://beta.usemoon.ai*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**aavev3PoolBorrow**](AAVEv3PoolApi.md#aavev3PoolBorrow) | **POST** /aave/v3/pool/{address}/borrow |  |
| [**aavev3PoolGetReserveData**](AAVEv3PoolApi.md#aavev3PoolGetReserveData) | **GET** /aave/v3/pool/{account}/getReserveData |  |
| [**aavev3PoolGetUserAccountData**](AAVEv3PoolApi.md#aavev3PoolGetUserAccountData) | **GET** /aave/v3/pool/{account}/getUserAccountData |  |
| [**aavev3PoolLiquidationCall**](AAVEv3PoolApi.md#aavev3PoolLiquidationCall) | **POST** /aave/v3/pool/{address}/liquidationCall |  |
| [**aavev3PoolRepay**](AAVEv3PoolApi.md#aavev3PoolRepay) | **POST** /aave/v3/pool/{address}/repay |  |
| [**aavev3PoolSetUserUseReserveAsCollateral**](AAVEv3PoolApi.md#aavev3PoolSetUserUseReserveAsCollateral) | **POST** /aave/v3/pool/{address}/setUserUseReserveAsCollateral |  |
| [**aavev3PoolSupply**](AAVEv3PoolApi.md#aavev3PoolSupply) | **POST** /aave/v3/pool/{address}/supply |  |
| [**aavev3PoolWithdraw**](AAVEv3PoolApi.md#aavev3PoolWithdraw) | **POST** /aave/v3/pool/{address}/withdraw |  |


<a name="aavev3PoolBorrow"></a>
# **aavev3PoolBorrow**
> AavePoolAPIResponse_AavePoolExecuteFunctionResult_ aavev3PoolBorrow(address, Authorization, AavePoolInputBody)



    Borrows assets from the Aave pool.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**| - The address of the borrower. | [default to null] |
| **Authorization** | **String**| - The authorization token. | [default to null] |
| **AavePoolInputBody** | [**AavePoolInputBody**](../Models/AavePoolInputBody.md)| - The input body containing details for the borrow operation. | |

### Return type

[**AavePoolAPIResponse_AavePoolExecuteFunctionResult_**](../Models/AavePoolAPIResponse_AavePoolExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="aavev3PoolGetReserveData"></a>
# **aavev3PoolGetReserveData**
> AavePoolAPIResponse_any_ aavev3PoolGetReserveData(account, Authorization, chainId, address, asset)



    Retrieves reserve data for a specific asset from the Aave pool.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **account** | **String**| - The account identifier. | [default to null] |
| **Authorization** | **String**| - The authorization token. | [default to null] |
| **chainId** | **String**| - The blockchain chain ID. | [default to null] |
| **address** | **String**| - The address of the Aave pool. | [default to null] |
| **asset** | **String**| - The asset for which to retrieve reserve data. | [default to null] |

### Return type

[**AavePoolAPIResponse_any_**](../Models/AavePoolAPIResponse_any_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="aavev3PoolGetUserAccountData"></a>
# **aavev3PoolGetUserAccountData**
> AavePoolAPIResponse_any_ aavev3PoolGetUserAccountData(account, Authorization, chainId, address, user)



    Retrieves user account data from the Aave pool.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **account** | **String**| - The account identifier from the path. | [default to null] |
| **Authorization** | **String**| - The authorization token from the header. | [default to null] |
| **chainId** | **String**| - The chain ID from the query parameters. | [default to null] |
| **address** | **String**| - The address from the query parameters. | [default to null] |
| **user** | **String**| - The user identifier from the query parameters. | [default to null] |

### Return type

[**AavePoolAPIResponse_any_**](../Models/AavePoolAPIResponse_any_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="aavev3PoolLiquidationCall"></a>
# **aavev3PoolLiquidationCall**
> AavePoolAPIResponse_AavePoolExecuteFunctionResult_ aavev3PoolLiquidationCall(address, Authorization, AavePoolInputBody)



    Handles the liquidation call to the Aave pool.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**| - The address to be liquidated. | [default to null] |
| **Authorization** | **String**| - The authorization token. | [default to null] |
| **AavePoolInputBody** | [**AavePoolInputBody**](../Models/AavePoolInputBody.md)| - The body containing the Aave pool input data. | |

### Return type

[**AavePoolAPIResponse_AavePoolExecuteFunctionResult_**](../Models/AavePoolAPIResponse_AavePoolExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="aavev3PoolRepay"></a>
# **aavev3PoolRepay**
> AavePoolAPIResponse_AavePoolExecuteFunctionResult_ aavev3PoolRepay(address, Authorization, AavePoolInputBody)



    Repays a loan on the Aave protocol.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**| - The address of the borrower. | [default to null] |
| **Authorization** | **String**| - The authorization token. | [default to null] |
| **AavePoolInputBody** | [**AavePoolInputBody**](../Models/AavePoolInputBody.md)| - The body of the request containing repayment details. | |

### Return type

[**AavePoolAPIResponse_AavePoolExecuteFunctionResult_**](../Models/AavePoolAPIResponse_AavePoolExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="aavev3PoolSetUserUseReserveAsCollateral"></a>
# **aavev3PoolSetUserUseReserveAsCollateral**
> AavePoolAPIResponse_AavePoolExecuteFunctionResult_ aavev3PoolSetUserUseReserveAsCollateral(address, Authorization, AavePoolInputBody)



    Sets the user&#39;s reserve as collateral in the Aave pool.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**| - The address of the user. | [default to null] |
| **Authorization** | **String**| - The authorization token. | [default to null] |
| **AavePoolInputBody** | [**AavePoolInputBody**](../Models/AavePoolInputBody.md)| - The body containing the Aave pool input data. | |

### Return type

[**AavePoolAPIResponse_AavePoolExecuteFunctionResult_**](../Models/AavePoolAPIResponse_AavePoolExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="aavev3PoolSupply"></a>
# **aavev3PoolSupply**
> AavePoolAPIResponse_AavePoolExecuteFunctionResult_ aavev3PoolSupply(address, Authorization, AavePoolInputBody)



    Supplies assets to the Aave pool.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**| - The address of the user supplying the assets. | [default to null] |
| **Authorization** | **String**| - The authorization token. | [default to null] |
| **AavePoolInputBody** | [**AavePoolInputBody**](../Models/AavePoolInputBody.md)| - The input body containing details for the supply operation. | |

### Return type

[**AavePoolAPIResponse_AavePoolExecuteFunctionResult_**](../Models/AavePoolAPIResponse_AavePoolExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="aavev3PoolWithdraw"></a>
# **aavev3PoolWithdraw**
> AavePoolAPIResponse_AavePoolExecuteFunctionResult_ aavev3PoolWithdraw(address, Authorization, AavePoolInputBody)



    Withdraws assets from the Aave pool.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**| - The address from which to withdraw assets. | [default to null] |
| **Authorization** | **String**| - The authorization token. | [default to null] |
| **AavePoolInputBody** | [**AavePoolInputBody**](../Models/AavePoolInputBody.md)| - The body containing the withdrawal details. | |

### Return type

[**AavePoolAPIResponse_AavePoolExecuteFunctionResult_**](../Models/AavePoolAPIResponse_AavePoolExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

