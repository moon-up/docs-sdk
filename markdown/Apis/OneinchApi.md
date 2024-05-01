# OneinchApi

All URIs are relative to *https://beta.usemoon.ai*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**approveCallData**](OneinchApi.md#approveCallData) | **POST** /oneinch/approve-call-data |  |
| [**approveSpender**](OneinchApi.md#approveSpender) | **POST** /oneinch/approve-spender |  |
| [**protocols**](OneinchApi.md#protocols) | **POST** /oneinch/protocols |  |
| [**quote**](OneinchApi.md#quote) | **POST** /oneinch/quote |  |
| [**swap**](OneinchApi.md#swap) | **POST** /oneinch/{accountName}/swap |  |
| [**tokens**](OneinchApi.md#tokens) | **POST** /oneinch/tokens |  |


<a name="approveCallData"></a>
# **approveCallData**
> oas_any_type_not_mapped approveCallData(body)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **body** | **oas_any_type_not_mapped**|  | |

### Return type

[**oas_any_type_not_mapped**](../Models/AnyType.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="approveSpender"></a>
# **approveSpender**
> oas_any_type_not_mapped approveSpender(body)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **body** | **oas_any_type_not_mapped**|  | |

### Return type

[**oas_any_type_not_mapped**](../Models/AnyType.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="protocols"></a>
# **protocols**
> oas_any_type_not_mapped protocols(body)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **body** | **oas_any_type_not_mapped**|  | |

### Return type

[**oas_any_type_not_mapped**](../Models/AnyType.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="quote"></a>
# **quote**
> oas_any_type_not_mapped quote(body)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **body** | **oas_any_type_not_mapped**|  | |

### Return type

[**oas_any_type_not_mapped**](../Models/AnyType.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="swap"></a>
# **swap**
> oas_any_type_not_mapped swap(accountName, Authorization, GetSwapDto)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **accountName** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **GetSwapDto** | [**GetSwapDto**](../Models/GetSwapDto.md)|  | |

### Return type

[**oas_any_type_not_mapped**](../Models/AnyType.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="tokens"></a>
# **tokens**
> oas_any_type_not_mapped tokens(body)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **body** | **oas_any_type_not_mapped**|  | |

### Return type

[**oas_any_type_not_mapped**](../Models/AnyType.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

