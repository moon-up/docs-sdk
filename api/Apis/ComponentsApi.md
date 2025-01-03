# ComponentsApi

All URIs are relative to *https://beta.usemoon.ai*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**componentsCreateComponent**](ComponentsApi.md#componentsCreateComponent) | **POST** /components |  |
| [**componentsForceEmbedding**](ComponentsApi.md#componentsForceEmbedding) | **POST** /components/{id}/embedding/force |  |
| [**componentsGetComponent**](ComponentsApi.md#componentsGetComponent) | **GET** /components/{id} |  |
| [**componentsGetComponentCapabilitiesDescription**](ComponentsApi.md#componentsGetComponentCapabilitiesDescription) | **GET** /components/capabilities |  |
| [**componentsGetComponents**](ComponentsApi.md#componentsGetComponents) | **GET** /components |  |
| [**componentsSearchComponents**](ComponentsApi.md#componentsSearchComponents) | **GET** /components/search |  |
| [**componentsUpdateComponent**](ComponentsApi.md#componentsUpdateComponent) | **POST** /components/{id} |  |
| [**componentsUpdateEmbedding**](ComponentsApi.md#componentsUpdateEmbedding) | **POST** /components/{id}/embedding |  |


<a name="componentsCreateComponent"></a>
# **componentsCreateComponent**
> ComponentAPIResponse_ComponentDefinition_ componentsCreateComponent(Authorization, body)



    Creates a new component in the database.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**| - The authorization token from the request header. | [default to null] |
| **body** | **Pick_ComponentDefinition.Exclude_keyofComponentDefinition.id__**| - The component data to be created, excluding the \&quot;id\&quot; field. | |

### Return type

[**ComponentAPIResponse_ComponentDefinition_**](../Models/ComponentAPIResponse_ComponentDefinition_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="componentsForceEmbedding"></a>
# **componentsForceEmbedding**
> ComponentAPIResponse_void_ componentsForceEmbedding(id, Authorization, Components\_updateEmbedding\_request)



    Forces the embedding of a description for a component.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **id** | **String**| - The ID of the component. | [default to null] |
| **Authorization** | **String**| - The authorization token. | [default to null] |
| **Components\_updateEmbedding\_request** | [**Components_updateEmbedding_request**](../Models/Components_updateEmbedding_request.md)| - The request body containing the description. | |

### Return type

[**ComponentAPIResponse_void_**](../Models/ComponentAPIResponse_void_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="componentsGetComponent"></a>
# **componentsGetComponent**
> ComponentAPIResponse_ComponentDefinition_ componentsGetComponent(id, Authorization)



    Retrieves a component by its ID.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **id** | **String**| - The ID of the component to retrieve. | [default to null] |
| **Authorization** | **String**| - The authorization token. | [default to null] |

### Return type

[**ComponentAPIResponse_ComponentDefinition_**](../Models/ComponentAPIResponse_ComponentDefinition_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="componentsGetComponentCapabilitiesDescription"></a>
# **componentsGetComponentCapabilitiesDescription**
> ComponentAPIResponse_Partial_ComponentDefinition_-Array_ componentsGetComponentCapabilitiesDescription(Authorization)



    Retrieves the capabilities description of components from the database.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**| - The authorization token provided in the request header. | [default to null] |

### Return type

[**ComponentAPIResponse_Partial_ComponentDefinition_-Array_**](../Models/ComponentAPIResponse_Partial_ComponentDefinition_-Array_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="componentsGetComponents"></a>
# **componentsGetComponents**
> ComponentAPIResponse_ComponentDefinition-Array_ componentsGetComponents(Authorization)



    Retrieves a list of components from the database.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**| - The authorization token from the request header. | [default to null] |

### Return type

[**ComponentAPIResponse_ComponentDefinition-Array_**](../Models/ComponentAPIResponse_ComponentDefinition-Array_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="componentsSearchComponents"></a>
# **componentsSearchComponents**
> ComponentAPIResponse_ComponentMatch-Array_ componentsSearchComponents(Authorization, query, threshold, limit)



    Searches for components similar to the specified query.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **Authorization** | **String**| - The authorization token. | [default to null] |
| **query** | **String**| - The query to search for. | [default to null] |
| **threshold** | **String**| - The similarity threshold for the search. | [optional] [default to null] |
| **limit** | **String**| - The maximum number of results to return. | [optional] [default to null] |

### Return type

[**ComponentAPIResponse_ComponentMatch-Array_**](../Models/ComponentAPIResponse_ComponentMatch-Array_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="componentsUpdateComponent"></a>
# **componentsUpdateComponent**
> ComponentAPIResponse_ComponentDefinition_ componentsUpdateComponent(id, Authorization, Partial\_ComponentDefinition\_)



     Updates a component in the database.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **id** | **String**| The ID of the component. | [default to null] |
| **Authorization** | **String**| The authorization token. | [default to null] |
| **Partial\_ComponentDefinition\_** | [**Partial_ComponentDefinition_**](../Models/Partial_ComponentDefinition_.md)| The partial component data to be updated. | |

### Return type

[**ComponentAPIResponse_ComponentDefinition_**](../Models/ComponentAPIResponse_ComponentDefinition_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="componentsUpdateEmbedding"></a>
# **componentsUpdateEmbedding**
> ComponentAPIResponse_void_ componentsUpdateEmbedding(id, Authorization, Components\_updateEmbedding\_request)



    Updates the embedding of a component&#39;s description.

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **id** | **String**| - The ID of the component. | [default to null] |
| **Authorization** | **String**| - The authorization token. | [default to null] |
| **Components\_updateEmbedding\_request** | [**Components_updateEmbedding_request**](../Models/Components_updateEmbedding_request.md)| - The request body containing the description. | |

### Return type

[**ComponentAPIResponse_void_**](../Models/ComponentAPIResponse_void_.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

