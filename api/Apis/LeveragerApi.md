# LeveragerApi

All URIs are relative to *https://beta.usemoon.ai*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**leveragerDeleverageERC20**](LeveragerApi.md#leveragerDeleverageERC20) | **POST** /leverager/{accountName}/deleverage-erc20 |  |
| [**leveragerDeleverageNative**](LeveragerApi.md#leveragerDeleverageNative) | **POST** /leverager/{accountName}/deleverage-native |  |
| [**leveragerExecuteOperation**](LeveragerApi.md#leveragerExecuteOperation) | **POST** /leverager/{accountName}/execute-operation |  |
| [**leveragerGetAddressesProvider**](LeveragerApi.md#leveragerGetAddressesProvider) | **GET** /leverager/addresses-provider |  |
| [**leveragerGetDefaultAdminRole**](LeveragerApi.md#leveragerGetDefaultAdminRole) | **GET** /leverager/default-admin-role |  |
| [**leveragerGetLendingPool**](LeveragerApi.md#leveragerGetLendingPool) | **GET** /leverager/lending-pool |  |
| [**leveragerGetMinHF**](LeveragerApi.md#leveragerGetMinHF) | **GET** /leverager/min-hf |  |
| [**leveragerGetRoleAdmin**](LeveragerApi.md#leveragerGetRoleAdmin) | **GET** /leverager/role-admin |  |
| [**leveragerGetWETH**](LeveragerApi.md#leveragerGetWETH) | **GET** /leverager/weth |  |
| [**leveragerGrantRole**](LeveragerApi.md#leveragerGrantRole) | **POST** /leverager/{accountName}/grant-role |  |
| [**leveragerHasRole**](LeveragerApi.md#leveragerHasRole) | **GET** /leverager/has-role |  |
| [**leveragerIsPaused**](LeveragerApi.md#leveragerIsPaused) | **GET** /leverager/paused |  |
| [**leveragerLeverageERC20**](LeveragerApi.md#leveragerLeverageERC20) | **POST** /leverager/{accountName}/leverage-erc20 |  |
| [**leveragerLeverageNative**](LeveragerApi.md#leveragerLeverageNative) | **POST** /leverager/{accountName}/leverage-native |  |
| [**leveragerPause**](LeveragerApi.md#leveragerPause) | **POST** /leverager/{accountName}/pause |  |
| [**leveragerRenounceRole**](LeveragerApi.md#leveragerRenounceRole) | **POST** /leverager/{accountName}/renounce-role |  |
| [**leveragerRevokeRole**](LeveragerApi.md#leveragerRevokeRole) | **POST** /leverager/{accountName}/revoke-role |  |
| [**leveragerSupportsInterface**](LeveragerApi.md#leveragerSupportsInterface) | **GET** /leverager/supports-interface |  |
| [**leveragerUnpause**](LeveragerApi.md#leveragerUnpause) | **POST** /leverager/{accountName}/unpause |  |


<a name="leveragerDeleverageERC20"></a>
# **leveragerDeleverageERC20**
> LeveragerAPIResponse_LeveragerExecuteFunctionResult_ leveragerDeleverageERC20(accountName, Authorization, LeveragerInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **accountName** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **LeveragerInputBody** | [**LeveragerInputBody**](../Models/LeveragerInputBody.md)|  | |

### Return type

[**LeveragerAPIResponse_LeveragerExecuteFunctionResult_**](../Models/LeveragerAPIResponse_LeveragerExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="leveragerDeleverageNative"></a>
# **leveragerDeleverageNative**
> LeveragerAPIResponse_LeveragerExecuteFunctionResult_ leveragerDeleverageNative(accountName, Authorization, LeveragerInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **accountName** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **LeveragerInputBody** | [**LeveragerInputBody**](../Models/LeveragerInputBody.md)|  | |

### Return type

[**LeveragerAPIResponse_LeveragerExecuteFunctionResult_**](../Models/LeveragerAPIResponse_LeveragerExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="leveragerExecuteOperation"></a>
# **leveragerExecuteOperation**
> LeveragerAPIResponse_LeveragerExecuteFunctionResult_ leveragerExecuteOperation(accountName, Authorization, LeveragerInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **accountName** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **LeveragerInputBody** | [**LeveragerInputBody**](../Models/LeveragerInputBody.md)|  | |

### Return type

[**LeveragerAPIResponse_LeveragerExecuteFunctionResult_**](../Models/LeveragerAPIResponse_LeveragerExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="leveragerGetAddressesProvider"></a>
# **leveragerGetAddressesProvider**
> LeveragerAPIResponse_string_ leveragerGetAddressesProvider(Authorization, address, chainId)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |

### Return type

[**LeveragerAPIResponse_string_**](../Models/LeveragerAPIResponse_string_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="leveragerGetDefaultAdminRole"></a>
# **leveragerGetDefaultAdminRole**
> LeveragerAPIResponse_string_ leveragerGetDefaultAdminRole(Authorization, address, chainId)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |

### Return type

[**LeveragerAPIResponse_string_**](../Models/LeveragerAPIResponse_string_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="leveragerGetLendingPool"></a>
# **leveragerGetLendingPool**
> LeveragerAPIResponse_string_ leveragerGetLendingPool(Authorization, address, chainId)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |

### Return type

[**LeveragerAPIResponse_string_**](../Models/LeveragerAPIResponse_string_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="leveragerGetMinHF"></a>
# **leveragerGetMinHF**
> LeveragerAPIResponse_string_ leveragerGetMinHF(Authorization, address, chainId)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |

### Return type

[**LeveragerAPIResponse_string_**](../Models/LeveragerAPIResponse_string_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="leveragerGetRoleAdmin"></a>
# **leveragerGetRoleAdmin**
> LeveragerAPIResponse_string_ leveragerGetRoleAdmin(Authorization, address, chainId, role)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **role** | **String**|  | [default to null] |

### Return type

[**LeveragerAPIResponse_string_**](../Models/LeveragerAPIResponse_string_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="leveragerGetWETH"></a>
# **leveragerGetWETH**
> LeveragerAPIResponse_string_ leveragerGetWETH(Authorization, address, chainId)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |

### Return type

[**LeveragerAPIResponse_string_**](../Models/LeveragerAPIResponse_string_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="leveragerGrantRole"></a>
# **leveragerGrantRole**
> LeveragerAPIResponse_LeveragerExecuteFunctionResult_ leveragerGrantRole(accountName, Authorization, LeveragerInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **accountName** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **LeveragerInputBody** | [**LeveragerInputBody**](../Models/LeveragerInputBody.md)|  | |

### Return type

[**LeveragerAPIResponse_LeveragerExecuteFunctionResult_**](../Models/LeveragerAPIResponse_LeveragerExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="leveragerHasRole"></a>
# **leveragerHasRole**
> LeveragerAPIResponse_boolean_ leveragerHasRole(Authorization, address, chainId, role, account)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **role** | **String**|  | [default to null] |
| **account** | **String**|  | [default to null] |

### Return type

[**LeveragerAPIResponse_boolean_**](../Models/LeveragerAPIResponse_boolean_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="leveragerIsPaused"></a>
# **leveragerIsPaused**
> LeveragerAPIResponse_boolean_ leveragerIsPaused(Authorization, address, chainId)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |

### Return type

[**LeveragerAPIResponse_boolean_**](../Models/LeveragerAPIResponse_boolean_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="leveragerLeverageERC20"></a>
# **leveragerLeverageERC20**
> LeveragerAPIResponse_LeveragerExecuteFunctionResult_ leveragerLeverageERC20(accountName, Authorization, LeveragerInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **accountName** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **LeveragerInputBody** | [**LeveragerInputBody**](../Models/LeveragerInputBody.md)|  | |

### Return type

[**LeveragerAPIResponse_LeveragerExecuteFunctionResult_**](../Models/LeveragerAPIResponse_LeveragerExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="leveragerLeverageNative"></a>
# **leveragerLeverageNative**
> LeveragerAPIResponse_LeveragerExecuteFunctionResult_ leveragerLeverageNative(accountName, Authorization, LeveragerInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **accountName** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **LeveragerInputBody** | [**LeveragerInputBody**](../Models/LeveragerInputBody.md)|  | |

### Return type

[**LeveragerAPIResponse_LeveragerExecuteFunctionResult_**](../Models/LeveragerAPIResponse_LeveragerExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="leveragerPause"></a>
# **leveragerPause**
> LeveragerAPIResponse_LeveragerExecuteFunctionResult_ leveragerPause(accountName, Authorization, LeveragerInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **accountName** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **LeveragerInputBody** | [**LeveragerInputBody**](../Models/LeveragerInputBody.md)|  | |

### Return type

[**LeveragerAPIResponse_LeveragerExecuteFunctionResult_**](../Models/LeveragerAPIResponse_LeveragerExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="leveragerRenounceRole"></a>
# **leveragerRenounceRole**
> LeveragerAPIResponse_LeveragerExecuteFunctionResult_ leveragerRenounceRole(accountName, Authorization, LeveragerInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **accountName** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **LeveragerInputBody** | [**LeveragerInputBody**](../Models/LeveragerInputBody.md)|  | |

### Return type

[**LeveragerAPIResponse_LeveragerExecuteFunctionResult_**](../Models/LeveragerAPIResponse_LeveragerExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="leveragerRevokeRole"></a>
# **leveragerRevokeRole**
> LeveragerAPIResponse_LeveragerExecuteFunctionResult_ leveragerRevokeRole(accountName, Authorization, LeveragerInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **accountName** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **LeveragerInputBody** | [**LeveragerInputBody**](../Models/LeveragerInputBody.md)|  | |

### Return type

[**LeveragerAPIResponse_LeveragerExecuteFunctionResult_**](../Models/LeveragerAPIResponse_LeveragerExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="leveragerSupportsInterface"></a>
# **leveragerSupportsInterface**
> LeveragerAPIResponse_boolean_ leveragerSupportsInterface(Authorization, address, chainId, interfaceId)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **address** | **String**|  | [default to null] |
| **chainId** | **String**|  | [default to null] |
| **interfaceId** | **String**|  | [default to null] |

### Return type

[**LeveragerAPIResponse_boolean_**](../Models/LeveragerAPIResponse_boolean_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="leveragerUnpause"></a>
# **leveragerUnpause**
> LeveragerAPIResponse_LeveragerExecuteFunctionResult_ leveragerUnpause(accountName, Authorization, LeveragerInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **accountName** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **LeveragerInputBody** | [**LeveragerInputBody**](../Models/LeveragerInputBody.md)|  | |

### Return type

[**LeveragerAPIResponse_LeveragerExecuteFunctionResult_**](../Models/LeveragerAPIResponse_LeveragerExecuteFunctionResult_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

