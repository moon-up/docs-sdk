# DefaultApi

All URIs are relative to *https://beta.usemoon.ai*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**getMessage**](DefaultApi.md#getMessage) | **GET** /ping |  |
| [**getTools**](DefaultApi.md#getTools) | **GET** /lifi/tools |  |
| [**lIFIGetAllPossibleConnections**](DefaultApi.md#lIFIGetAllPossibleConnections) | **GET** /lifi/allPossibleConnections |  |
| [**lIFIGetChains**](DefaultApi.md#lIFIGetChains) | **GET** /lifi/chains |  |
| [**lIFIGetConnections**](DefaultApi.md#lIFIGetConnections) | **GET** /lifi/connections |  |
| [**lIFIGetQuote**](DefaultApi.md#lIFIGetQuote) | **GET** /lifi/quote |  |
| [**lIFIGetStatus**](DefaultApi.md#lIFIGetStatus) | **GET** /lifi/status |  |
| [**lIFIGetTokenDetails**](DefaultApi.md#lIFIGetTokenDetails) | **GET** /lifi/token |  |
| [**lIFIGetTokens**](DefaultApi.md#lIFIGetTokens) | **GET** /lifi/tokens |  |
| [**lIFIPostQuote**](DefaultApi.md#lIFIPostQuote) | **POST** /lifi/{accountName}/quote |  |


<a name="getMessage"></a>
# **getMessage**
> PingResponse getMessage()



### Parameters
This endpoint does not need any parameter.

### Return type

[**PingResponse**](../Models/PingResponse.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getTools"></a>
# **getTools**
> ApiResponse_ToolsResponse_ getTools(chains)



    Retrieves tools based on the provided chains.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **chains** | **String**| - Optional query parameter specifying the chains to filter tools. | [optional] [default to null] |

### Return type

[**ApiResponse_ToolsResponse_**](../Models/ApiResponse_ToolsResponse_.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="lIFIGetAllPossibleConnections"></a>
# **lIFIGetAllPossibleConnections**
> ApiResponse_TokenInfoByChainId_ lIFIGetAllPossibleConnections(toChain, toToken)



    Retrieves all possible connections for a given chain and token.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **toChain** | **String**| - The target chain identifier. | [default to null] |
| **toToken** | **String**| - The target token identifier. | [default to null] |

### Return type

[**ApiResponse_TokenInfoByChainId_**](../Models/ApiResponse_TokenInfoByChainId_.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="lIFIGetChains"></a>
# **lIFIGetChains**
> ApiResponse_ChainsResponse_ lIFIGetChains(optionalChainTypes)



    Retrieves a list of supported chains.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **optionalChainTypes** | **String**| - Optional parameter to filter chains by type (&#39;EVM&#39; or &#39;SOL&#39;). | [optional] [default to null] [enum: EVM, SOL] |

### Return type

[**ApiResponse_ChainsResponse_**](../Models/ApiResponse_ChainsResponse_.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="lIFIGetConnections"></a>
# **lIFIGetConnections**
> ApiResponse_ConnectionsResponse_ lIFIGetConnections(fromChain, toChain, fromToken, toToken, chainTypes)



    Retrieves connections between specified chains and tokens.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **fromChain** | **String**| - The source blockchain identifier. | [default to null] |
| **toChain** | **String**| - The destination blockchain identifier. | [default to null] |
| **fromToken** | **String**| - The source token identifier. | [default to null] |
| **toToken** | **String**| - The destination token identifier. | [default to null] |
| **chainTypes** | **String**| - Optional parameter to specify types of chains. | [optional] [default to null] |

### Return type

[**ApiResponse_ConnectionsResponse_**](../Models/ApiResponse_ConnectionsResponse_.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="lIFIGetQuote"></a>
# **lIFIGetQuote**
> ApiResponse_Quote_ lIFIGetQuote(fromChain, toChain, fromToken, toToken, fromAmount, fromAddress, toAddress, order, slippage, integrator, fee, referrer, allowBridges, allowExchanges, denyBridges, denyExchanges, preferBridges, preferExchanges)



    Retrieves a quote for a token swap between different chains.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **fromChain** | **String**| - The source blockchain identifier. | [default to null] |
| **toChain** | **String**| - The destination blockchain identifier. | [default to null] |
| **fromToken** | **String**| - The token address on the source chain. | [default to null] |
| **toToken** | **String**| - The token address on the destination chain. | [default to null] |
| **fromAmount** | **String**| - The amount of the source token to swap. | [default to null] |
| **fromAddress** | **String**| - The address of the sender on the source chain. | [default to null] |
| **toAddress** | **String**| - The address of the recipient on the destination chain (optional). | [optional] [default to null] |
| **order** | **String**| - The order preference for the quote (&#39;BEST_VALUE&#39;, &#39;BEST_FEE&#39;, &#39;BEST_FEE_GAS&#39;) (optional). | [optional] [default to null] [enum: BEST_VALUE, BEST_FEE, BEST_FEE_GAS] |
| **slippage** | **Double**| - The maximum acceptable slippage percentage (optional). | [optional] [default to null] |
| **integrator** | **String**| - The integrator identifier (optional). | [optional] [default to null] |
| **fee** | **Double**| - The fee amount (optional). | [optional] [default to null] |
| **referrer** | **String**| - The referrer identifier (optional). | [optional] [default to null] |
| **allowBridges** | [**List**](../Models/String.md)| - A list of allowed bridges (optional). | [optional] [default to null] |
| **allowExchanges** | [**List**](../Models/String.md)| - A list of allowed exchanges (optional). | [optional] [default to null] |
| **denyBridges** | [**List**](../Models/String.md)| - A list of denied bridges (optional). | [optional] [default to null] |
| **denyExchanges** | [**List**](../Models/String.md)| - A list of denied exchanges (optional). | [optional] [default to null] |
| **preferBridges** | [**List**](../Models/String.md)| - A list of preferred bridges (optional). | [optional] [default to null] |
| **preferExchanges** | [**List**](../Models/String.md)| - A list of preferred exchanges (optional). | [optional] [default to null] |

### Return type

[**ApiResponse_Quote_**](../Models/ApiResponse_Quote_.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="lIFIGetStatus"></a>
# **lIFIGetStatus**
> ApiResponse_StatusResponse_ lIFIGetStatus(txHash)



    Retrieves the status of a transaction based on the provided transaction hash.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **txHash** | **String**| - The hash of the transaction to retrieve the status for. | [default to null] |

### Return type

[**ApiResponse_StatusResponse_**](../Models/ApiResponse_StatusResponse_.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="lIFIGetTokenDetails"></a>
# **lIFIGetTokenDetails**
> ApiResponse_TokenDetails_ lIFIGetTokenDetails(chain, token)



    Fetches the details of a specified token on a given blockchain.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **chain** | **String**| - The blockchain on which the token resides. | [default to null] |
| **token** | **String**| - The address or symbol of the token to fetch details for. | [default to null] |

### Return type

[**ApiResponse_TokenDetails_**](../Models/ApiResponse_TokenDetails_.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="lIFIGetTokens"></a>
# **lIFIGetTokens**
> ApiResponse_TokensResponse_ lIFIGetTokens()



    Fetches tokens from the LiFi service.

### Parameters
This endpoint does not need any parameter.

### Return type

[**ApiResponse_TokensResponse_**](../Models/ApiResponse_TokensResponse_.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="lIFIPostQuote"></a>
# **lIFIPostQuote**
> ApiResponse_PostQuote_ lIFIPostQuote(accountName, Authorization, fromChain, toChain, fromToken, toToken, fromAmount, fromAddress, toAddress, order, slippage, integrator, fee, referrer, allowBridges, allowExchanges, denyBridges, denyExchanges, preferBridges, preferExchanges, dryRun, broadcast)



    Handles the retrieval of a quote for a token swap between different chains.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **accountName** | **String**| - The name of the account requesting the quote. | [default to null] |
| **Authorization** | **String**| - The authorization token for the request. | [default to null] |
| **fromChain** | **String**| - The chain from which the token swap will originate. | [default to null] |
| **toChain** | **String**| - The chain to which the token swap will be sent. | [default to null] |
| **fromToken** | **String**| - The token to be swapped from. | [default to null] |
| **toToken** | **String**| - The token to be swapped to. | [default to null] |
| **fromAmount** | **String**| - The amount of the token to be swapped from. | [default to null] |
| **fromAddress** | **String**| - The address from which the token swap will originate. | [default to null] |
| **toAddress** | **String**| - (Optional) The address to which the token swap will be sent. | [optional] [default to null] |
| **order** | **String**| - (Optional) The order preference for the quote (BEST_VALUE, BEST_FEE, BEST_FEE_GAS). | [optional] [default to null] [enum: BEST_VALUE, BEST_FEE, BEST_FEE_GAS] |
| **slippage** | **Double**| - (Optional) The acceptable slippage percentage for the swap. | [optional] [default to null] |
| **integrator** | **String**| - (Optional) The integrator identifier. | [optional] [default to null] |
| **fee** | **Double**| - (Optional) The fee for the swap. | [optional] [default to null] |
| **referrer** | **String**| - (Optional) The referrer identifier. | [optional] [default to null] |
| **allowBridges** | [**List**](../Models/String.md)| - (Optional) The list of allowed bridges for the swap. | [optional] [default to null] |
| **allowExchanges** | [**List**](../Models/String.md)| - (Optional) The list of allowed exchanges for the swap. | [optional] [default to null] |
| **denyBridges** | [**List**](../Models/String.md)| - (Optional) The list of denied bridges for the swap. | [optional] [default to null] |
| **denyExchanges** | [**List**](../Models/String.md)| - (Optional) The list of denied exchanges for the swap. | [optional] [default to null] |
| **preferBridges** | [**List**](../Models/String.md)| - (Optional) The list of preferred bridges for the swap. | [optional] [default to null] |
| **preferExchanges** | [**List**](../Models/String.md)| - (Optional) The list of preferred exchanges for the swap. | [optional] [default to null] |
| **dryRun** | **Boolean**|  | [optional] [default to null] |
| **broadcast** | **Boolean**|  | [optional] [default to null] |

### Return type

[**ApiResponse_PostQuote_**](../Models/ApiResponse_PostQuote_.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

