# UniswapV2RouterApi

All URIs are relative to *https://beta.usemoon.ai*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**addLiquidity**](UniswapV2RouterApi.md#addLiquidity) | **POST** /uniswap/v2/router/{account}/addLiquidity |  |
| [**addLiquidityETH**](UniswapV2RouterApi.md#addLiquidityETH) | **POST** /uniswap/v2/router/{account}/addLiquidityETH |  |
| [**getAmountIn**](UniswapV2RouterApi.md#getAmountIn) | **POST** /uniswap/v2/router/{account}/getAmountIn |  |
| [**getAmountOut**](UniswapV2RouterApi.md#getAmountOut) | **POST** /uniswap/v2/router/{account}/getAmountOut |  |
| [**getAmountsIn**](UniswapV2RouterApi.md#getAmountsIn) | **POST** /uniswap/v2/router/{account}/getAmountsIn |  |
| [**getAmountsOut**](UniswapV2RouterApi.md#getAmountsOut) | **POST** /uniswap/v2/router/{account}/getAmountsOut |  |
| [**getWETH**](UniswapV2RouterApi.md#getWETH) | **GET** /uniswap/v2/router/{account}/WETH |  |
| [**quote**](UniswapV2RouterApi.md#quote) | **POST** /uniswap/v2/router/{account}/quote |  |
| [**removeLiquidity**](UniswapV2RouterApi.md#removeLiquidity) | **POST** /uniswap/v2/router/{account}/removeLiquidity |  |
| [**removeLiquidityETH**](UniswapV2RouterApi.md#removeLiquidityETH) | **POST** /uniswap/v2/router/{account}/removeLiquidityETH |  |
| [**removeLiquidityETHSupportingFeeOnTransferTokens**](UniswapV2RouterApi.md#removeLiquidityETHSupportingFeeOnTransferTokens) | **POST** /uniswap/v2/router/{account}/removeLiquidityETHSupportingFeeOnTransferTokens |  |
| [**removeLiquidityETHWithPermit**](UniswapV2RouterApi.md#removeLiquidityETHWithPermit) | **POST** /uniswap/v2/router/{account}/removeLiquidityETHWithPermit |  |
| [**removeLiquidityETHWithPermitSupportingFeeOnTransferTokens**](UniswapV2RouterApi.md#removeLiquidityETHWithPermitSupportingFeeOnTransferTokens) | **POST** /uniswap/v2/router/{account}/removeLiquidityETHWithPermitSupportingFeeOnTransferTokens |  |
| [**removeLiquidityWithPermit**](UniswapV2RouterApi.md#removeLiquidityWithPermit) | **POST** /uniswap/v2/router/{account}/removeLiquidityWithPermit |  |
| [**swapETHForExactTokens**](UniswapV2RouterApi.md#swapETHForExactTokens) | **POST** /uniswap/v2/router/{account}/swapETHForExactTokens |  |
| [**swapExactETHForTokens**](UniswapV2RouterApi.md#swapExactETHForTokens) | **POST** /uniswap/v2/router/{account}/swapExactETHForTokens |  |
| [**swapExactETHForTokensSupportingFeeOnTransferTokens**](UniswapV2RouterApi.md#swapExactETHForTokensSupportingFeeOnTransferTokens) | **POST** /uniswap/v2/router/{account}/swapExactETHForTokensSupportingFeeOnTransferTokens |  |
| [**swapExactTokensForETH**](UniswapV2RouterApi.md#swapExactTokensForETH) | **POST** /uniswap/v2/router/{account}/swapExactTokensForETH |  |
| [**swapExactTokensForETHSupportingFeeOnTransferTokens**](UniswapV2RouterApi.md#swapExactTokensForETHSupportingFeeOnTransferTokens) | **POST** /uniswap/v2/router/{account}/swapExactTokensForETHSupportingFeeOnTransferTokens |  |
| [**swapExactTokensForTokens**](UniswapV2RouterApi.md#swapExactTokensForTokens) | **POST** /uniswap/v2/router/{account}/swapExactTokensForTokens |  |
| [**swapExactTokensForTokensSupportingFeeOnTransferTokens**](UniswapV2RouterApi.md#swapExactTokensForTokensSupportingFeeOnTransferTokens) | **POST** /uniswap/v2/router/{account}/swapExactTokensForTokensSupportingFeeOnTransferTokens |  |
| [**swapTokensForExactETH**](UniswapV2RouterApi.md#swapTokensForExactETH) | **POST** /uniswap/v2/router/{account}/swapTokensForExactETH |  |
| [**swapTokensForExactTokens**](UniswapV2RouterApi.md#swapTokensForExactTokens) | **POST** /uniswap/v2/router/{account}/swapTokensForExactTokens |  |


<a name="addLiquidity"></a>
# **addLiquidity**
> UniswapV2APIResponse_UniswapV2ExecuteFunctionResult_ addLiquidity(account, Authorization, UniswapV2InputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **account** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **UniswapV2InputBody** | [**UniswapV2InputBody**](../Models/UniswapV2InputBody.md)|  | |

### Return type

[**UniswapV2APIResponse_UniswapV2ExecuteFunctionResult_**](../Models/UniswapV2APIResponse_UniswapV2ExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="addLiquidityETH"></a>
# **addLiquidityETH**
> UniswapV2APIResponse_UniswapV2ExecuteFunctionResult_ addLiquidityETH(account, Authorization, UniswapV2InputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **account** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **UniswapV2InputBody** | [**UniswapV2InputBody**](../Models/UniswapV2InputBody.md)|  | |

### Return type

[**UniswapV2APIResponse_UniswapV2ExecuteFunctionResult_**](../Models/UniswapV2APIResponse_UniswapV2ExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="getAmountIn"></a>
# **getAmountIn**
> UniswapV2APIResponse_UniswapV2ExecuteFunctionResult_ getAmountIn(account, Authorization, UniswapV2InputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **account** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **UniswapV2InputBody** | [**UniswapV2InputBody**](../Models/UniswapV2InputBody.md)|  | |

### Return type

[**UniswapV2APIResponse_UniswapV2ExecuteFunctionResult_**](../Models/UniswapV2APIResponse_UniswapV2ExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="getAmountOut"></a>
# **getAmountOut**
> UniswapV2APIResponse_UniswapV2ExecuteFunctionResult_ getAmountOut(account, Authorization, UniswapV2InputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **account** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **UniswapV2InputBody** | [**UniswapV2InputBody**](../Models/UniswapV2InputBody.md)|  | |

### Return type

[**UniswapV2APIResponse_UniswapV2ExecuteFunctionResult_**](../Models/UniswapV2APIResponse_UniswapV2ExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="getAmountsIn"></a>
# **getAmountsIn**
> UniswapV2APIResponse_UniswapV2ExecuteFunctionResult_ getAmountsIn(account, Authorization, UniswapV2InputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **account** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **UniswapV2InputBody** | [**UniswapV2InputBody**](../Models/UniswapV2InputBody.md)|  | |

### Return type

[**UniswapV2APIResponse_UniswapV2ExecuteFunctionResult_**](../Models/UniswapV2APIResponse_UniswapV2ExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="getAmountsOut"></a>
# **getAmountsOut**
> UniswapV2APIResponse_UniswapV2ExecuteFunctionResult_ getAmountsOut(account, Authorization, UniswapV2InputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **account** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **UniswapV2InputBody** | [**UniswapV2InputBody**](../Models/UniswapV2InputBody.md)|  | |

### Return type

[**UniswapV2APIResponse_UniswapV2ExecuteFunctionResult_**](../Models/UniswapV2APIResponse_UniswapV2ExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="getWETH"></a>
# **getWETH**
> UniswapV2APIResponse_UniswapV2ExecuteFunctionResult_ getWETH(account, Authorization, chainId, address)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **account** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |

### Return type

[**UniswapV2APIResponse_UniswapV2ExecuteFunctionResult_**](../Models/UniswapV2APIResponse_UniswapV2ExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="quote"></a>
# **quote**
> UniswapV2APIResponse_UniswapV2ExecuteFunctionResult_ quote(account, Authorization, UniswapV2InputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **account** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **UniswapV2InputBody** | [**UniswapV2InputBody**](../Models/UniswapV2InputBody.md)|  | |

### Return type

[**UniswapV2APIResponse_UniswapV2ExecuteFunctionResult_**](../Models/UniswapV2APIResponse_UniswapV2ExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="removeLiquidity"></a>
# **removeLiquidity**
> UniswapV2APIResponse_UniswapV2ExecuteFunctionResult_ removeLiquidity(account, Authorization, UniswapV2InputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **account** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **UniswapV2InputBody** | [**UniswapV2InputBody**](../Models/UniswapV2InputBody.md)|  | |

### Return type

[**UniswapV2APIResponse_UniswapV2ExecuteFunctionResult_**](../Models/UniswapV2APIResponse_UniswapV2ExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="removeLiquidityETH"></a>
# **removeLiquidityETH**
> UniswapV2APIResponse_UniswapV2ExecuteFunctionResult_ removeLiquidityETH(account, Authorization, UniswapV2InputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **account** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **UniswapV2InputBody** | [**UniswapV2InputBody**](../Models/UniswapV2InputBody.md)|  | |

### Return type

[**UniswapV2APIResponse_UniswapV2ExecuteFunctionResult_**](../Models/UniswapV2APIResponse_UniswapV2ExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="removeLiquidityETHSupportingFeeOnTransferTokens"></a>
# **removeLiquidityETHSupportingFeeOnTransferTokens**
> UniswapV2APIResponse_UniswapV2ExecuteFunctionResult_ removeLiquidityETHSupportingFeeOnTransferTokens(account, Authorization, UniswapV2InputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **account** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **UniswapV2InputBody** | [**UniswapV2InputBody**](../Models/UniswapV2InputBody.md)|  | |

### Return type

[**UniswapV2APIResponse_UniswapV2ExecuteFunctionResult_**](../Models/UniswapV2APIResponse_UniswapV2ExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="removeLiquidityETHWithPermit"></a>
# **removeLiquidityETHWithPermit**
> UniswapV2APIResponse_UniswapV2ExecuteFunctionResult_ removeLiquidityETHWithPermit(account, Authorization, UniswapV2InputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **account** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **UniswapV2InputBody** | [**UniswapV2InputBody**](../Models/UniswapV2InputBody.md)|  | |

### Return type

[**UniswapV2APIResponse_UniswapV2ExecuteFunctionResult_**](../Models/UniswapV2APIResponse_UniswapV2ExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="removeLiquidityETHWithPermitSupportingFeeOnTransferTokens"></a>
# **removeLiquidityETHWithPermitSupportingFeeOnTransferTokens**
> UniswapV2APIResponse_UniswapV2ExecuteFunctionResult_ removeLiquidityETHWithPermitSupportingFeeOnTransferTokens(account, Authorization, UniswapV2InputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **account** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **UniswapV2InputBody** | [**UniswapV2InputBody**](../Models/UniswapV2InputBody.md)|  | |

### Return type

[**UniswapV2APIResponse_UniswapV2ExecuteFunctionResult_**](../Models/UniswapV2APIResponse_UniswapV2ExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="removeLiquidityWithPermit"></a>
# **removeLiquidityWithPermit**
> UniswapV2APIResponse_UniswapV2ExecuteFunctionResult_ removeLiquidityWithPermit(account, Authorization, UniswapV2InputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **account** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **UniswapV2InputBody** | [**UniswapV2InputBody**](../Models/UniswapV2InputBody.md)|  | |

### Return type

[**UniswapV2APIResponse_UniswapV2ExecuteFunctionResult_**](../Models/UniswapV2APIResponse_UniswapV2ExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="swapETHForExactTokens"></a>
# **swapETHForExactTokens**
> UniswapV2APIResponse_UniswapV2ExecuteFunctionResult_ swapETHForExactTokens(account, Authorization, UniswapV2InputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **account** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **UniswapV2InputBody** | [**UniswapV2InputBody**](../Models/UniswapV2InputBody.md)|  | |

### Return type

[**UniswapV2APIResponse_UniswapV2ExecuteFunctionResult_**](../Models/UniswapV2APIResponse_UniswapV2ExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="swapExactETHForTokens"></a>
# **swapExactETHForTokens**
> UniswapV2APIResponse_UniswapV2ExecuteFunctionResult_ swapExactETHForTokens(account, Authorization, UniswapV2InputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **account** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **UniswapV2InputBody** | [**UniswapV2InputBody**](../Models/UniswapV2InputBody.md)|  | |

### Return type

[**UniswapV2APIResponse_UniswapV2ExecuteFunctionResult_**](../Models/UniswapV2APIResponse_UniswapV2ExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="swapExactETHForTokensSupportingFeeOnTransferTokens"></a>
# **swapExactETHForTokensSupportingFeeOnTransferTokens**
> UniswapV2APIResponse_UniswapV2ExecuteFunctionResult_ swapExactETHForTokensSupportingFeeOnTransferTokens(account, Authorization, UniswapV2InputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **account** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **UniswapV2InputBody** | [**UniswapV2InputBody**](../Models/UniswapV2InputBody.md)|  | |

### Return type

[**UniswapV2APIResponse_UniswapV2ExecuteFunctionResult_**](../Models/UniswapV2APIResponse_UniswapV2ExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="swapExactTokensForETH"></a>
# **swapExactTokensForETH**
> UniswapV2APIResponse_UniswapV2ExecuteFunctionResult_ swapExactTokensForETH(account, Authorization, UniswapV2InputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **account** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **UniswapV2InputBody** | [**UniswapV2InputBody**](../Models/UniswapV2InputBody.md)|  | |

### Return type

[**UniswapV2APIResponse_UniswapV2ExecuteFunctionResult_**](../Models/UniswapV2APIResponse_UniswapV2ExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="swapExactTokensForETHSupportingFeeOnTransferTokens"></a>
# **swapExactTokensForETHSupportingFeeOnTransferTokens**
> UniswapV2APIResponse_UniswapV2ExecuteFunctionResult_ swapExactTokensForETHSupportingFeeOnTransferTokens(account, Authorization, UniswapV2InputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **account** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **UniswapV2InputBody** | [**UniswapV2InputBody**](../Models/UniswapV2InputBody.md)|  | |

### Return type

[**UniswapV2APIResponse_UniswapV2ExecuteFunctionResult_**](../Models/UniswapV2APIResponse_UniswapV2ExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="swapExactTokensForTokens"></a>
# **swapExactTokensForTokens**
> UniswapV2APIResponse_UniswapV2ExecuteFunctionResult_ swapExactTokensForTokens(account, Authorization, UniswapV2InputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **account** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **UniswapV2InputBody** | [**UniswapV2InputBody**](../Models/UniswapV2InputBody.md)|  | |

### Return type

[**UniswapV2APIResponse_UniswapV2ExecuteFunctionResult_**](../Models/UniswapV2APIResponse_UniswapV2ExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="swapExactTokensForTokensSupportingFeeOnTransferTokens"></a>
# **swapExactTokensForTokensSupportingFeeOnTransferTokens**
> UniswapV2APIResponse_UniswapV2ExecuteFunctionResult_ swapExactTokensForTokensSupportingFeeOnTransferTokens(account, Authorization, UniswapV2InputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **account** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **UniswapV2InputBody** | [**UniswapV2InputBody**](../Models/UniswapV2InputBody.md)|  | |

### Return type

[**UniswapV2APIResponse_UniswapV2ExecuteFunctionResult_**](../Models/UniswapV2APIResponse_UniswapV2ExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="swapTokensForExactETH"></a>
# **swapTokensForExactETH**
> UniswapV2APIResponse_UniswapV2ExecuteFunctionResult_ swapTokensForExactETH(account, Authorization, UniswapV2InputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **account** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **UniswapV2InputBody** | [**UniswapV2InputBody**](../Models/UniswapV2InputBody.md)|  | |

### Return type

[**UniswapV2APIResponse_UniswapV2ExecuteFunctionResult_**](../Models/UniswapV2APIResponse_UniswapV2ExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="swapTokensForExactTokens"></a>
# **swapTokensForExactTokens**
> UniswapV2APIResponse_UniswapV2ExecuteFunctionResult_ swapTokensForExactTokens(account, Authorization, UniswapV2InputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **account** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **UniswapV2InputBody** | [**UniswapV2InputBody**](../Models/UniswapV2InputBody.md)|  | |

### Return type

[**UniswapV2APIResponse_UniswapV2ExecuteFunctionResult_**](../Models/UniswapV2APIResponse_UniswapV2ExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

