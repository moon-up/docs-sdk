# UniSwapApi

All URIs are relative to *https://beta.usemoon.ai*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**addLiquidity**](UniSwapApi.md#addLiquidity) | **POST** /uniswap/{name}/add-liquidity |  |
| [**removeLiquidity**](UniSwapApi.md#removeLiquidity) | **POST** /uniswap/{name}/remove-liquidity |  |
| [**swapExactETHForTokens**](UniSwapApi.md#swapExactETHForTokens) | **POST** /uniswap/{name}/swap-exact-eth-for-tokens |  |
| [**swapExactTokensForTokens**](UniSwapApi.md#swapExactTokensForTokens) | **POST** /uniswap/{name}/swap-exact-tokens-for-tokens |  |


<a name="addLiquidity"></a>
# **addLiquidity**
> TransactionAPIResponse addLiquidity(Authorization, name, UniswapInput)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **name** | **String**|  | [default to null] |
| **UniswapInput** | [**UniswapInput**](../Models/UniswapInput.md)|  | |

### Return type

[**TransactionAPIResponse**](../Models/TransactionAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="removeLiquidity"></a>
# **removeLiquidity**
> TransactionAPIResponse removeLiquidity(Authorization, name, UniswapInput)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **name** | **String**|  | [default to null] |
| **UniswapInput** | [**UniswapInput**](../Models/UniswapInput.md)|  | |

### Return type

[**TransactionAPIResponse**](../Models/TransactionAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="swapExactETHForTokens"></a>
# **swapExactETHForTokens**
> TransactionAPIResponse swapExactETHForTokens(Authorization, name, UniswapInput)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **name** | **String**|  | [default to null] |
| **UniswapInput** | [**UniswapInput**](../Models/UniswapInput.md)|  | |

### Return type

[**TransactionAPIResponse**](../Models/TransactionAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="swapExactTokensForTokens"></a>
# **swapExactTokensForTokens**
> TransactionAPIResponse swapExactTokensForTokens(Authorization, name, UniswapInput)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **name** | **String**|  | [default to null] |
| **UniswapInput** | [**UniswapInput**](../Models/UniswapInput.md)|  | |

### Return type

[**TransactionAPIResponse**](../Models/TransactionAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

