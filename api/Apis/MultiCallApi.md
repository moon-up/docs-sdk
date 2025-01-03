# MultiCallApi

All URIs are relative to *https://beta.usemoon.ai*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createFlow**](MultiCallApi.md#createFlow) | **POST** /multicall/flows |  |
| [**createJob**](MultiCallApi.md#createJob) | **POST** /multicall/create-job |  |
| [**createUserDefinedFunction**](MultiCallApi.md#createUserDefinedFunction) | **POST** /multicall/user-defined-functions |  |
| [**deleteFlow**](MultiCallApi.md#deleteFlow) | **DELETE** /multicall/flows/{flowId} |  |
| [**deleteJob**](MultiCallApi.md#deleteJob) | **DELETE** /multicall/job/{jobId} |  |
| [**deleteUserDefinedFunction**](MultiCallApi.md#deleteUserDefinedFunction) | **DELETE** /multicall/user-defined-functions/{functionId} |  |
| [**executeJob**](MultiCallApi.md#executeJob) | **POST** /multicall/execute-job/{jobId} |  |
| [**getFlow**](MultiCallApi.md#getFlow) | **GET** /multicall/flows/{flowId} |  |
| [**getJob**](MultiCallApi.md#getJob) | **GET** /multicall/job/{jobId} |  |
| [**getJobResult**](MultiCallApi.md#getJobResult) | **GET** /multicall/job-result/{jobId} |  |
| [**getNotifications**](MultiCallApi.md#getNotifications) | **GET** /multicall/notifications |  |
| [**getScheduledJobs**](MultiCallApi.md#getScheduledJobs) | **GET** /multicall/scheduled-jobs |  |
| [**listFlows**](MultiCallApi.md#listFlows) | **GET** /multicall/flows |  |
| [**listJobs**](MultiCallApi.md#listJobs) | **GET** /multicall/jobs |  |
| [**listUserDefinedFunctions**](MultiCallApi.md#listUserDefinedFunctions) | **GET** /multicall/user-defined-functions |  |
| [**markNotificationAsRead**](MultiCallApi.md#markNotificationAsRead) | **POST** /multicall/notifications/{notificationId}/mark-as-read |  |
| [**scheduleJob**](MultiCallApi.md#scheduleJob) | **POST** /multicall/schedule-job |  |
| [**unscheduleJob**](MultiCallApi.md#unscheduleJob) | **POST** /multicall/unschedule-job/{jobId} |  |
| [**updateFlow**](MultiCallApi.md#updateFlow) | **PUT** /multicall/flows/{flowId} |  |


<a name="createFlow"></a>
# **createFlow**
> MultiCallAPIResponse_string_ createFlow(Authorization, CreateFlowBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **CreateFlowBody** | [**CreateFlowBody**](../Models/CreateFlowBody.md)|  | |

### Return type

[**MultiCallAPIResponse_string_**](../Models/MultiCallAPIResponse_string_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="createJob"></a>
# **createJob**
> MultiCallAPIResponse_string_ createJob(Authorization, MultiCallInputBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **MultiCallInputBody** | [**MultiCallInputBody**](../Models/MultiCallInputBody.md)|  | |

### Return type

[**MultiCallAPIResponse_string_**](../Models/MultiCallAPIResponse_string_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="createUserDefinedFunction"></a>
# **createUserDefinedFunction**
> MultiCallAPIResponse createUserDefinedFunction(Authorization, CreateUserDefinedFunction\_request)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **CreateUserDefinedFunction\_request** | [**CreateUserDefinedFunction_request**](../Models/CreateUserDefinedFunction_request.md)|  | |

### Return type

[**MultiCallAPIResponse**](../Models/MultiCallAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="deleteFlow"></a>
# **deleteFlow**
> MultiCallAPIResponse deleteFlow(flowId, Authorization)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **flowId** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |

### Return type

[**MultiCallAPIResponse**](../Models/MultiCallAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="deleteJob"></a>
# **deleteJob**
> MultiCallAPIResponse deleteJob(jobId, Authorization)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **jobId** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |

### Return type

[**MultiCallAPIResponse**](../Models/MultiCallAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="deleteUserDefinedFunction"></a>
# **deleteUserDefinedFunction**
> MultiCallAPIResponse deleteUserDefinedFunction(functionId, Authorization)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **functionId** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |

### Return type

[**MultiCallAPIResponse**](../Models/MultiCallAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="executeJob"></a>
# **executeJob**
> MultiCallAPIResponse executeJob(jobId, Authorization)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **jobId** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |

### Return type

[**MultiCallAPIResponse**](../Models/MultiCallAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getFlow"></a>
# **getFlow**
> MultiCallAPIResponse_Flow_ getFlow(flowId, Authorization)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **flowId** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |

### Return type

[**MultiCallAPIResponse_Flow_**](../Models/MultiCallAPIResponse_Flow_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getJob"></a>
# **getJob**
> MultiCallAPIResponse_Jobs_ getJob(jobId, Authorization)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **jobId** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |

### Return type

[**MultiCallAPIResponse_Jobs_**](../Models/MultiCallAPIResponse_Jobs_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getJobResult"></a>
# **getJobResult**
> MultiCallAPIResponse_any_ getJobResult(jobId, Authorization)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **jobId** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |

### Return type

[**MultiCallAPIResponse_any_**](../Models/MultiCallAPIResponse_any_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getNotifications"></a>
# **getNotifications**
> MultiCallAPIResponse_any-Array_ getNotifications(Authorization)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |

### Return type

[**MultiCallAPIResponse_any-Array_**](../Models/MultiCallAPIResponse_any-Array_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getScheduledJobs"></a>
# **getScheduledJobs**
> MultiCallAPIResponse_any-Array_ getScheduledJobs(Authorization)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |

### Return type

[**MultiCallAPIResponse_any-Array_**](../Models/MultiCallAPIResponse_any-Array_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="listFlows"></a>
# **listFlows**
> MultiCallAPIResponse_Flow-Array_ listFlows(Authorization)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |

### Return type

[**MultiCallAPIResponse_Flow-Array_**](../Models/MultiCallAPIResponse_Flow-Array_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="listJobs"></a>
# **listJobs**
> MultiCallAPIResponse_Jobs-Array_ listJobs(Authorization)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |

### Return type

[**MultiCallAPIResponse_Jobs-Array_**](../Models/MultiCallAPIResponse_Jobs-Array_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="listUserDefinedFunctions"></a>
# **listUserDefinedFunctions**
> MultiCallAPIResponse_any-Array_ listUserDefinedFunctions(Authorization)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |

### Return type

[**MultiCallAPIResponse_any-Array_**](../Models/MultiCallAPIResponse_any-Array_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="markNotificationAsRead"></a>
# **markNotificationAsRead**
> MultiCallAPIResponse markNotificationAsRead(notificationId, Authorization)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **notificationId** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |

### Return type

[**MultiCallAPIResponse**](../Models/MultiCallAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="scheduleJob"></a>
# **scheduleJob**
> MultiCallAPIResponse scheduleJob(Authorization, ScheduleJobBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**|  | [default to null] |
| **ScheduleJobBody** | [**ScheduleJobBody**](../Models/ScheduleJobBody.md)|  | |

### Return type

[**MultiCallAPIResponse**](../Models/MultiCallAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="unscheduleJob"></a>
# **unscheduleJob**
> MultiCallAPIResponse unscheduleJob(jobId, Authorization)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **jobId** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |

### Return type

[**MultiCallAPIResponse**](../Models/MultiCallAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="updateFlow"></a>
# **updateFlow**
> MultiCallAPIResponse updateFlow(flowId, Authorization, UpdateFlowBody)



### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **flowId** | **String**|  | [default to null] |
| **Authorization** | **String**|  | [default to null] |
| **UpdateFlowBody** | [**UpdateFlowBody**](../Models/UpdateFlowBody.md)|  | |

### Return type

[**MultiCallAPIResponse**](../Models/MultiCallAPIResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

