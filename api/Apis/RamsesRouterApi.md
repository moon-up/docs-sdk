# RamsesRouterApi

All URIs are relative to *https://beta.usemoon.ai*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**addLiquidity**](RamsesRouterApi.md#addLiquidity) | **POST** /ramses/router/{address}/addLiquidity |  |
| [**addLiquidityETH**](RamsesRouterApi.md#addLiquidityETH) | **POST** /ramses/router/{address}/addLiquidityETH |  |
| [**getAmountOut**](RamsesRouterApi.md#getAmountOut) | **GET** /ramses/router/getAmountOut |  |
| [**getAmountsOut**](RamsesRouterApi.md#getAmountsOut) | **GET** /ramses/router/getAmountsOut |  |
| [**getFactory**](RamsesRouterApi.md#getFactory) | **GET** /ramses/router/factory |  |
| [**getReserves**](RamsesRouterApi.md#getReserves) | **GET** /ramses/router/getReserves |  |
| [**getWeth**](RamsesRouterApi.md#getWeth) | **GET** /ramses/router/weth |  |
| [**isPair**](RamsesRouterApi.md#isPair) | **GET** /ramses/router/isPair |  |
| [**pairFor**](RamsesRouterApi.md#pairFor) | **GET** /ramses/router/pairFor |  |
| [**quoteAddLiquidity**](RamsesRouterApi.md#quoteAddLiquidity) | **GET** /ramses/router/quoteAddLiquidity |  |
| [**quoteRemoveLiquidity**](RamsesRouterApi.md#quoteRemoveLiquidity) | **GET** /ramses/router/quoteRemoveLiquidity |  |
| [**removeLiquidity**](RamsesRouterApi.md#removeLiquidity) | **POST** /ramses/router/{address}/removeLiquidity |  |
| [**removeLiquidityETH**](RamsesRouterApi.md#removeLiquidityETH) | **POST** /ramses/router/{address}/removeLiquidityETH |  |
| [**sortTokens**](RamsesRouterApi.md#sortTokens) | **GET** /ramses/router/sortTokens |  |
| [**swapExactETHForTokens**](RamsesRouterApi.md#swapExactETHForTokens) | **POST** /ramses/router/{address}/swapExactETHForTokens |  |
| [**swapExactTokensForETH**](RamsesRouterApi.md#swapExactTokensForETH) | **POST** /ramses/router/{address}/swapExactTokensForETH |  |
| [**swapExactTokensForTokens**](RamsesRouterApi.md#swapExactTokensForTokens) | **POST** /ramses/router/{address}/swapExactTokensForTokens |  |
| [**uNSAFESwapExactTokensForTokens**](RamsesRouterApi.md#uNSAFESwapExactTokensForTokens) | **POST** /ramses/router/{address}/UNSAFE_swapExactTokensForTokens |  |


<a name="addLiquidity"></a>
# **addLiquidity**
> RamsesRouterAPIResponse_RamsesRouterExecuteFunctionResult_ addLiquidity(address, Authorization, RamsesRouterInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **RamsesRouterInputBody** | [**RamsesRouterInputBody**](../Models/RamsesRouterInputBody.md)|  | |

### Return type

[**RamsesRouterAPIResponse_RamsesRouterExecuteFunctionResult_**](../Models/RamsesRouterAPIResponse_RamsesRouterExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="addLiquidityETH"></a>
# **addLiquidityETH**
> RamsesRouterAPIResponse_RamsesRouterExecuteFunctionResult_ addLiquidityETH(address, Authorization, RamsesRouterInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **RamsesRouterInputBody** | [**RamsesRouterInputBody**](../Models/RamsesRouterInputBody.md)|  | |

### Return type

[**RamsesRouterAPIResponse_RamsesRouterExecuteFunctionResult_**](../Models/RamsesRouterAPIResponse_RamsesRouterExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="getAmountOut"></a>
# **getAmountOut**
> RamsesRouterAPIResponse__amountOut-string--stable-boolean__ getAmountOut(Authorization, chainId, address, amountIn, tokenIn, tokenOut)



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

[**RamsesRouterAPIResponse__amountOut-string--stable-boolean__**](../Models/RamsesRouterAPIResponse__amountOut-string--stable-boolean__.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getAmountsOut"></a>
# **getAmountsOut**
> RamsesRouterAPIResponse_string-Array_ getAmountsOut(Authorization, chainId, address, amountIn, routes)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |
| **amountIn** | **String**|  | [default to null] |
| **routes** | **String**|  | [default to null] |

### Return type

[**RamsesRouterAPIResponse_string-Array_**](../Models/RamsesRouterAPIResponse_string-Array_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getFactory"></a>
# **getFactory**
> RamsesRouterAPIResponse_string_ getFactory(Authorization, chainId, address)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |

### Return type

[**RamsesRouterAPIResponse_string_**](../Models/RamsesRouterAPIResponse_string_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getReserves"></a>
# **getReserves**
> RamsesRouterAPIResponse__reserve0:string--reserve1:string__ getReserves(Authorization, chainId, address, tokenA, tokenB, stable)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |
| **tokenA** | **String**|  | [default to null] |
| **tokenB** | **String**|  | [default to null] |
| **stable** | **Boolean**|  | [default to null] |

### Return type

[**RamsesRouterAPIResponse__reserve0:string--reserve1:string__**](../Models/RamsesRouterAPIResponse__reserve0:string--reserve1:string__.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getWeth"></a>
# **getWeth**
> RamsesRouterAPIResponse_string_ getWeth(Authorization, chainId, address)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |

### Return type

[**RamsesRouterAPIResponse_string_**](../Models/RamsesRouterAPIResponse_string_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="isPair"></a>
# **isPair**
> RamsesRouterAPIResponse_boolean_ isPair(Authorization, chainId, address, pair)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |
| **pair** | **String**|  | [default to null] |

### Return type

[**RamsesRouterAPIResponse_boolean_**](../Models/RamsesRouterAPIResponse_boolean_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="pairFor"></a>
# **pairFor**
> RamsesRouterAPIResponse_string_ pairFor(Authorization, chainId, address, tokenA, tokenB, stable)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |
| **tokenA** | **String**|  | [default to null] |
| **tokenB** | **String**|  | [default to null] |
| **stable** | **Boolean**|  | [default to null] |

### Return type

[**RamsesRouterAPIResponse_string_**](../Models/RamsesRouterAPIResponse_string_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="quoteAddLiquidity"></a>
# **quoteAddLiquidity**
> RamsesRouterAPIResponse__amountA-string--amountB-string--liquidity-string--__ quoteAddLiquidity(Authorization, chainId, address, tokenA, tokenB, stable, amountADesired, amountBDesired)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |
| **tokenA** | **String**|  | [default to null] |
| **tokenB** | **String**|  | [default to null] |
| **stable** | **Boolean**|  | [default to null] |
| **amountADesired** | **String**|  | [default to null] |
| **amountBDesired** | **String**|  | [default to null] |

### Return type

[**RamsesRouterAPIResponse__amountA-string--amountB-string--liquidity-string--__**](../Models/RamsesRouterAPIResponse__amountA-string--amountB-string--liquidity-string--__.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="quoteRemoveLiquidity"></a>
# **quoteRemoveLiquidity**
> RamsesRouterAPIResponse__amountA-string--amountB-string__ quoteRemoveLiquidity(Authorization, chainId, address, tokenA, tokenB, stable, liquidity)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |
| **tokenA** | **String**|  | [default to null] |
| **tokenB** | **String**|  | [default to null] |
| **stable** | **Boolean**|  | [default to null] |
| **liquidity** | **String**|  | [default to null] |

### Return type

[**RamsesRouterAPIResponse__amountA-string--amountB-string__**](../Models/RamsesRouterAPIResponse__amountA-string--amountB-string__.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="removeLiquidity"></a>
# **removeLiquidity**
> RamsesRouterAPIResponse_RamsesRouterExecuteFunctionResult_ removeLiquidity(address, Authorization, RamsesRouterInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **RamsesRouterInputBody** | [**RamsesRouterInputBody**](../Models/RamsesRouterInputBody.md)|  | |

### Return type

[**RamsesRouterAPIResponse_RamsesRouterExecuteFunctionResult_**](../Models/RamsesRouterAPIResponse_RamsesRouterExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="removeLiquidityETH"></a>
# **removeLiquidityETH**
> RamsesRouterAPIResponse_RamsesRouterExecuteFunctionResult_ removeLiquidityETH(address, Authorization, RamsesRouterInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **RamsesRouterInputBody** | [**RamsesRouterInputBody**](../Models/RamsesRouterInputBody.md)|  | |

### Return type

[**RamsesRouterAPIResponse_RamsesRouterExecuteFunctionResult_**](../Models/RamsesRouterAPIResponse_RamsesRouterExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="sortTokens"></a>
# **sortTokens**
> RamsesRouterAPIResponse_SortedTokens_ sortTokens(Authorization, chainId, address, tokenA, tokenB)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |
| **tokenA** | **String**|  | [default to null] |
| **tokenB** | **String**|  | [default to null] |

### Return type

[**RamsesRouterAPIResponse_SortedTokens_**](../Models/RamsesRouterAPIResponse_SortedTokens_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="swapExactETHForTokens"></a>
# **swapExactETHForTokens**
> RamsesRouterAPIResponse_RamsesRouterExecuteFunctionResult_ swapExactETHForTokens(address, Authorization, RamsesRouterInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **RamsesRouterInputBody** | [**RamsesRouterInputBody**](../Models/RamsesRouterInputBody.md)|  | |

### Return type

[**RamsesRouterAPIResponse_RamsesRouterExecuteFunctionResult_**](../Models/RamsesRouterAPIResponse_RamsesRouterExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="swapExactTokensForETH"></a>
# **swapExactTokensForETH**
> RamsesRouterAPIResponse_RamsesRouterExecuteFunctionResult_ swapExactTokensForETH(address, Authorization, RamsesRouterInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **RamsesRouterInputBody** | [**RamsesRouterInputBody**](../Models/RamsesRouterInputBody.md)|  | |

### Return type

[**RamsesRouterAPIResponse_RamsesRouterExecuteFunctionResult_**](../Models/RamsesRouterAPIResponse_RamsesRouterExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="swapExactTokensForTokens"></a>
# **swapExactTokensForTokens**
> RamsesRouterAPIResponse_RamsesRouterExecuteFunctionResult_ swapExactTokensForTokens(address, Authorization, RamsesRouterInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **RamsesRouterInputBody** | [**RamsesRouterInputBody**](../Models/RamsesRouterInputBody.md)|  | |

### Return type

[**RamsesRouterAPIResponse_RamsesRouterExecuteFunctionResult_**](../Models/RamsesRouterAPIResponse_RamsesRouterExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="uNSAFESwapExactTokensForTokens"></a>
# **uNSAFESwapExactTokensForTokens**
> RamsesRouterAPIResponse_RamsesRouterExecuteFunctionResult_ uNSAFESwapExactTokensForTokens(address, Authorization, RamsesRouterInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **RamsesRouterInputBody** | [**RamsesRouterInputBody**](../Models/RamsesRouterInputBody.md)|  | |

### Return type

[**RamsesRouterAPIResponse_RamsesRouterExecuteFunctionResult_**](../Models/RamsesRouterAPIResponse_RamsesRouterExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

