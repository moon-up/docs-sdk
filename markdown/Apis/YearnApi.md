# YearnApi

All URIs are relative to *https://beta.usemoon.ai*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**addLiquidity**](YearnApi.md#addLiquidity) | **POST** /yearn/{name}/add-liquidity |  |
| [**addLiquidityWeth**](YearnApi.md#addLiquidityWeth) | **POST** /yearn/{name}/add-liquidity-weth |  |
| [**removeLiquidity**](YearnApi.md#removeLiquidity) | **POST** /yearn/{name}/remove-liquidity |  |
| [**removeLiquidityWeth**](YearnApi.md#removeLiquidityWeth) | **POST** /yearn/{name}/remove-liquidity-weth |  |


<a name="addLiquidity"></a>
# **addLiquidity**
> TransactionAPIResponse addLiquidity(Authorization, name, InputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **name** | **String**|  | [default to null] |
| **InputBody** | [**InputBody**](../Models/InputBody.md)|  | |

### Return type

[**TransactionAPIResponse**](../Models/TransactionAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="addLiquidityWeth"></a>
# **addLiquidityWeth**
> TransactionAPIResponse addLiquidityWeth(Authorization, name, InputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **name** | **String**|  | [default to null] |
| **InputBody** | [**InputBody**](../Models/InputBody.md)|  | |

### Return type

[**TransactionAPIResponse**](../Models/TransactionAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="removeLiquidity"></a>
# **removeLiquidity**
> TransactionAPIResponse removeLiquidity(Authorization, name, InputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **name** | **String**|  | [default to null] |
| **InputBody** | [**InputBody**](../Models/InputBody.md)|  | |

### Return type

[**TransactionAPIResponse**](../Models/TransactionAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="removeLiquidityWeth"></a>
# **removeLiquidityWeth**
> TransactionAPIResponse removeLiquidityWeth(Authorization, name, InputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **name** | **String**|  | [default to null] |
| **InputBody** | [**InputBody**](../Models/InputBody.md)|  | |

### Return type

[**TransactionAPIResponse**](../Models/TransactionAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

