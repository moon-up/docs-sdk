# LynexRouterApi

All URIs are relative to *https://beta.usemoon.ai*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**addLiquidity**](LynexRouterApi.md#addLiquidity) | **POST** /lynex/router/{address}/addLiquidity |  |
| [**addLiquidityETH**](LynexRouterApi.md#addLiquidityETH) | **POST** /lynex/router/{address}/addLiquidityETH |  |
| [**getAmountOut**](LynexRouterApi.md#getAmountOut) | **GET** /lynex/router/getAmountOut |  |
| [**getAmountsOut**](LynexRouterApi.md#getAmountsOut) | **GET** /lynex/router/getAmountsOut |  |
| [**getFactory**](LynexRouterApi.md#getFactory) | **GET** /lynex/router/factory |  |
| [**getWETH**](LynexRouterApi.md#getWETH) | **GET** /lynex/router/wETH |  |
| [**swapExactETHForTokens**](LynexRouterApi.md#swapExactETHForTokens) | **POST** /lynex/router/{address}/swapExactETHForTokens |  |
| [**swapExactTokensForETH**](LynexRouterApi.md#swapExactTokensForETH) | **POST** /lynex/router/{address}/swapExactTokensForETH |  |
| [**swapExactTokensForTokens**](LynexRouterApi.md#swapExactTokensForTokens) | **POST** /lynex/router/{address}/swapExactTokensForTokens |  |


<a name="addLiquidity"></a>
# **addLiquidity**
> LynexRouterAPIResponse_LynexRouterExecuteFunctionResult_ addLiquidity(address, Authorization, LynexRouterInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **LynexRouterInputBody** | [**LynexRouterInputBody**](../Models/LynexRouterInputBody.md)|  | |

### Return type

[**LynexRouterAPIResponse_LynexRouterExecuteFunctionResult_**](../Models/LynexRouterAPIResponse_LynexRouterExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="addLiquidityETH"></a>
# **addLiquidityETH**
> LynexRouterAPIResponse_LynexRouterExecuteFunctionResult_ addLiquidityETH(address, Authorization, LynexRouterInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **LynexRouterInputBody** | [**LynexRouterInputBody**](../Models/LynexRouterInputBody.md)|  | |

### Return type

[**LynexRouterAPIResponse_LynexRouterExecuteFunctionResult_**](../Models/LynexRouterAPIResponse_LynexRouterExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="getAmountOut"></a>
# **getAmountOut**
> LynexRouterAPIResponse__amountOut-string--stable-boolean__ getAmountOut(Authorization, chainId, address, amountIn, tokenIn, tokenOut)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |
| **amountIn** | **String**|  | [default to null] |
| **tokenIn** | **String**|  | [default to null] |
| **tokenOut** | **String**|  | [default to null] |

### Return type

[**LynexRouterAPIResponse__amountOut-string--stable-boolean__**](../Models/LynexRouterAPIResponse__amountOut-string--stable-boolean__.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getAmountsOut"></a>
# **getAmountsOut**
> LynexRouterAPIResponse_string-Array_ getAmountsOut(Authorization, chainId, address, amountIn, routes)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |
| **amountIn** | **String**|  | [default to null] |
| **routes** | **String**|  | [default to null] |

### Return type

[**LynexRouterAPIResponse_string-Array_**](../Models/LynexRouterAPIResponse_string-Array_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getFactory"></a>
# **getFactory**
> LynexRouterAPIResponse_string_ getFactory(Authorization, chainId, address)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |

### Return type

[**LynexRouterAPIResponse_string_**](../Models/LynexRouterAPIResponse_string_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getWETH"></a>
# **getWETH**
> LynexRouterAPIResponse_string_ getWETH(Authorization, chainId, address)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |

### Return type

[**LynexRouterAPIResponse_string_**](../Models/LynexRouterAPIResponse_string_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="swapExactETHForTokens"></a>
# **swapExactETHForTokens**
> LynexRouterAPIResponse_LynexRouterExecuteFunctionResult_ swapExactETHForTokens(address, Authorization, LynexRouterInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **LynexRouterInputBody** | [**LynexRouterInputBody**](../Models/LynexRouterInputBody.md)|  | |

### Return type

[**LynexRouterAPIResponse_LynexRouterExecuteFunctionResult_**](../Models/LynexRouterAPIResponse_LynexRouterExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="swapExactTokensForETH"></a>
# **swapExactTokensForETH**
> LynexRouterAPIResponse_LynexRouterExecuteFunctionResult_ swapExactTokensForETH(address, Authorization, LynexRouterInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **LynexRouterInputBody** | [**LynexRouterInputBody**](../Models/LynexRouterInputBody.md)|  | |

### Return type

[**LynexRouterAPIResponse_LynexRouterExecuteFunctionResult_**](../Models/LynexRouterAPIResponse_LynexRouterExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="swapExactTokensForTokens"></a>
# **swapExactTokensForTokens**
> LynexRouterAPIResponse_LynexRouterExecuteFunctionResult_ swapExactTokensForTokens(address, Authorization, LynexRouterInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **LynexRouterInputBody** | [**LynexRouterInputBody**](../Models/LynexRouterInputBody.md)|  | |

### Return type

[**LynexRouterAPIResponse_LynexRouterExecuteFunctionResult_**](../Models/LynexRouterAPIResponse_LynexRouterExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

