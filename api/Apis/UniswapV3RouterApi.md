# UniswapV3RouterApi

All URIs are relative to *https://beta.usemoon.ai*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**exactInput**](UniswapV3RouterApi.md#exactInput) | **POST** /uniswap/v3/router/{address}/exactInput |  |
| [**exactInputSingle**](UniswapV3RouterApi.md#exactInputSingle) | **POST** /uniswap/v3/router/{address}/exactInputSingle |  |
| [**exactOutput**](UniswapV3RouterApi.md#exactOutput) | **POST** /uniswap/v3/router/{address}/exactOutput |  |
| [**exactOutputSingle**](UniswapV3RouterApi.md#exactOutputSingle) | **POST** /uniswap/v3/router/{address}/exactOutputSingle |  |
| [**factory**](UniswapV3RouterApi.md#factory) | **GET** /uniswap/v3/router/factory |  |
| [**multicall**](UniswapV3RouterApi.md#multicall) | **POST** /uniswap/v3/router/{address}/multicall |  |
| [**refundETH**](UniswapV3RouterApi.md#refundETH) | **POST** /uniswap/v3/router/{address}/refundETH |  |
| [**selfPermit**](UniswapV3RouterApi.md#selfPermit) | **POST** /uniswap/v3/router/{address}/selfPermit |  |
| [**selfPermitAllowed**](UniswapV3RouterApi.md#selfPermitAllowed) | **POST** /uniswap/v3/router/{address}/selfPermitAllowed |  |
| [**selfPermitAllowedIfNecessary**](UniswapV3RouterApi.md#selfPermitAllowedIfNecessary) | **POST** /uniswap/v3/router/{address}/selfPermitAllowedIfNecessary |  |
| [**selfPermitIfNecessary**](UniswapV3RouterApi.md#selfPermitIfNecessary) | **POST** /uniswap/v3/router/{address}/selfPermitIfNecessary |  |
| [**sweepToken**](UniswapV3RouterApi.md#sweepToken) | **POST** /uniswap/v3/router/{address}/sweepToken |  |
| [**sweepTokenWithFee**](UniswapV3RouterApi.md#sweepTokenWithFee) | **POST** /uniswap/v3/router/{address}/sweepTokenWithFee |  |
| [**unwrapWETH9**](UniswapV3RouterApi.md#unwrapWETH9) | **POST** /uniswap/v3/router/{address}/unwrapWETH9 |  |
| [**unwrapWETH9WithFee**](UniswapV3RouterApi.md#unwrapWETH9WithFee) | **POST** /uniswap/v3/router/{address}/unwrapWETH9WithFee |  |
| [**wETH9**](UniswapV3RouterApi.md#wETH9) | **GET** /uniswap/v3/router/WETH9 |  |


<a name="exactInput"></a>
# **exactInput**
> UniswapV3APIResponse_UniswapV3ExecuteFunctionResult_ exactInput(address, Authorization, UniswapV3InputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **UniswapV3InputBody** | [**UniswapV3InputBody**](../Models/UniswapV3InputBody.md)|  | |

### Return type

[**UniswapV3APIResponse_UniswapV3ExecuteFunctionResult_**](../Models/UniswapV3APIResponse_UniswapV3ExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="exactInputSingle"></a>
# **exactInputSingle**
> UniswapV3APIResponse_UniswapV3ExecuteFunctionResult_ exactInputSingle(address, Authorization, UniswapV3InputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **UniswapV3InputBody** | [**UniswapV3InputBody**](../Models/UniswapV3InputBody.md)|  | |

### Return type

[**UniswapV3APIResponse_UniswapV3ExecuteFunctionResult_**](../Models/UniswapV3APIResponse_UniswapV3ExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="exactOutput"></a>
# **exactOutput**
> UniswapV3APIResponse_UniswapV3ExecuteFunctionResult_ exactOutput(address, Authorization, UniswapV3InputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **UniswapV3InputBody** | [**UniswapV3InputBody**](../Models/UniswapV3InputBody.md)|  | |

### Return type

[**UniswapV3APIResponse_UniswapV3ExecuteFunctionResult_**](../Models/UniswapV3APIResponse_UniswapV3ExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="exactOutputSingle"></a>
# **exactOutputSingle**
> UniswapV3APIResponse_UniswapV3ExecuteFunctionResult_ exactOutputSingle(address, Authorization, UniswapV3InputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **UniswapV3InputBody** | [**UniswapV3InputBody**](../Models/UniswapV3InputBody.md)|  | |

### Return type

[**UniswapV3APIResponse_UniswapV3ExecuteFunctionResult_**](../Models/UniswapV3APIResponse_UniswapV3ExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="factory"></a>
# **factory**
> UniswapV3APIResponse_string_ factory(Authorization, chainId, address)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |

### Return type

[**UniswapV3APIResponse_string_**](../Models/UniswapV3APIResponse_string_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="multicall"></a>
# **multicall**
> UniswapV3APIResponse_UniswapV3ExecuteFunctionResult_ multicall(address, Authorization, UniswapV3InputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **UniswapV3InputBody** | [**UniswapV3InputBody**](../Models/UniswapV3InputBody.md)|  | |

### Return type

[**UniswapV3APIResponse_UniswapV3ExecuteFunctionResult_**](../Models/UniswapV3APIResponse_UniswapV3ExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="refundETH"></a>
# **refundETH**
> UniswapV3APIResponse_UniswapV3ExecuteFunctionResult_ refundETH(address, Authorization, UniswapV3InputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **UniswapV3InputBody** | [**UniswapV3InputBody**](../Models/UniswapV3InputBody.md)|  | |

### Return type

[**UniswapV3APIResponse_UniswapV3ExecuteFunctionResult_**](../Models/UniswapV3APIResponse_UniswapV3ExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="selfPermit"></a>
# **selfPermit**
> UniswapV3APIResponse_UniswapV3ExecuteFunctionResult_ selfPermit(address, Authorization, UniswapV3InputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **UniswapV3InputBody** | [**UniswapV3InputBody**](../Models/UniswapV3InputBody.md)|  | |

### Return type

[**UniswapV3APIResponse_UniswapV3ExecuteFunctionResult_**](../Models/UniswapV3APIResponse_UniswapV3ExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="selfPermitAllowed"></a>
# **selfPermitAllowed**
> UniswapV3APIResponse_UniswapV3ExecuteFunctionResult_ selfPermitAllowed(address, Authorization, UniswapV3InputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **UniswapV3InputBody** | [**UniswapV3InputBody**](../Models/UniswapV3InputBody.md)|  | |

### Return type

[**UniswapV3APIResponse_UniswapV3ExecuteFunctionResult_**](../Models/UniswapV3APIResponse_UniswapV3ExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="selfPermitAllowedIfNecessary"></a>
# **selfPermitAllowedIfNecessary**
> UniswapV3APIResponse_UniswapV3ExecuteFunctionResult_ selfPermitAllowedIfNecessary(address, Authorization, UniswapV3InputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **UniswapV3InputBody** | [**UniswapV3InputBody**](../Models/UniswapV3InputBody.md)|  | |

### Return type

[**UniswapV3APIResponse_UniswapV3ExecuteFunctionResult_**](../Models/UniswapV3APIResponse_UniswapV3ExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="selfPermitIfNecessary"></a>
# **selfPermitIfNecessary**
> UniswapV3APIResponse_UniswapV3ExecuteFunctionResult_ selfPermitIfNecessary(address, Authorization, UniswapV3InputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **UniswapV3InputBody** | [**UniswapV3InputBody**](../Models/UniswapV3InputBody.md)|  | |

### Return type

[**UniswapV3APIResponse_UniswapV3ExecuteFunctionResult_**](../Models/UniswapV3APIResponse_UniswapV3ExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="sweepToken"></a>
# **sweepToken**
> UniswapV3APIResponse_UniswapV3ExecuteFunctionResult_ sweepToken(address, Authorization, UniswapV3InputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **UniswapV3InputBody** | [**UniswapV3InputBody**](../Models/UniswapV3InputBody.md)|  | |

### Return type

[**UniswapV3APIResponse_UniswapV3ExecuteFunctionResult_**](../Models/UniswapV3APIResponse_UniswapV3ExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="sweepTokenWithFee"></a>
# **sweepTokenWithFee**
> UniswapV3APIResponse_UniswapV3ExecuteFunctionResult_ sweepTokenWithFee(address, Authorization, UniswapV3InputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **UniswapV3InputBody** | [**UniswapV3InputBody**](../Models/UniswapV3InputBody.md)|  | |

### Return type

[**UniswapV3APIResponse_UniswapV3ExecuteFunctionResult_**](../Models/UniswapV3APIResponse_UniswapV3ExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="unwrapWETH9"></a>
# **unwrapWETH9**
> UniswapV3APIResponse_UniswapV3ExecuteFunctionResult_ unwrapWETH9(address, Authorization, UniswapV3InputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **UniswapV3InputBody** | [**UniswapV3InputBody**](../Models/UniswapV3InputBody.md)|  | |

### Return type

[**UniswapV3APIResponse_UniswapV3ExecuteFunctionResult_**](../Models/UniswapV3APIResponse_UniswapV3ExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="unwrapWETH9WithFee"></a>
# **unwrapWETH9WithFee**
> UniswapV3APIResponse_UniswapV3ExecuteFunctionResult_ unwrapWETH9WithFee(address, Authorization, UniswapV3InputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **address** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **UniswapV3InputBody** | [**UniswapV3InputBody**](../Models/UniswapV3InputBody.md)|  | |

### Return type

[**UniswapV3APIResponse_UniswapV3ExecuteFunctionResult_**](../Models/UniswapV3APIResponse_UniswapV3ExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="wETH9"></a>
# **wETH9**
> UniswapV3APIResponse_string_ wETH9(Authorization, chainId, address)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |

### Return type

[**UniswapV3APIResponse_string_**](../Models/UniswapV3APIResponse_string_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

