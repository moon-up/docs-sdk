# Erc721Api

## moonsdk.Erc721Api

All URIs are relative to _https://beta.usemoon.ai_

| Method                                                              | HTTP request                                 | Description |
| ------------------------------------------------------------------- | -------------------------------------------- | ----------- |
| [**approve**](erc721api.md#approve)                                 | **POST** /erc721/{name}/approve              |             |
| [**balance\_of**](erc721api.md#balance\_of)                         | **POST** /erc721/{name}/balance-of           |             |
| [**get\_approved**](erc721api.md#get\_approved)                     | **POST** /erc721/{name}/get-approved         |             |
| [**is\_approved\_for\_all**](erc721api.md#is\_approved\_for\_all)   | **POST** /erc721/{name}/is-approved-for-all  |             |
| [**name**](erc721api.md#name)                                       | **POST** /erc721/{name}/name                 |             |
| [**owner\_of**](erc721api.md#owner\_of)                             | **POST** /erc721/{name}/owner-of             |             |
| [**safe\_transfer\_from**](erc721api.md#safe\_transfer\_from)       | **POST** /erc721/{name}/safe-transfer-from   |             |
| [**set\_approval\_for\_all**](erc721api.md#set\_approval\_for\_all) | **POST** /erc721/{name}/set-approval-for-all |             |
| [**symbol**](erc721api.md#symbol)                                   | **POST** /erc721/{name}/symbol               |             |
| [**token\_uri**](erc721api.md#token\_uri)                           | **POST** /erc721/{name}/token-uri            |             |
| [**transfer**](erc721api.md#transfer)                               | **POST** /erc721/{name}/transfer             |             |
| [**transfer\_from**](erc721api.md#transfer\_from)                   | **POST** /erc721/{name}/transfer-from        |             |

## **approve**

> TransactionAPIResponse approve(authorization, name, erc721\_request)

#### Example

* Api Key Authentication (ApiKeyAuth):
* Api Key Authentication (BearerAuth):

```python
import moonsdk
from moonsdk.models.erc721_request import Erc721Request
from moonsdk.models.transaction_api_response import TransactionAPIResponse
from moonsdk.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://beta.usemoon.ai
# See configuration.py for a list of all supported configuration parameters.
configuration = moonsdk.Configuration(
    host = "https://beta.usemoon.ai"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure API key authorization: ApiKeyAuth
configuration.api_key['ApiKeyAuth'] = os.environ["API_KEY"]

# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['ApiKeyAuth'] = 'Bearer'

# Configure API key authorization: BearerAuth
configuration.api_key['BearerAuth'] = os.environ["API_KEY"]

# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['BearerAuth'] = 'Bearer'

# Enter a context with an instance of the API client
async with moonsdk.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = moonsdk.Erc721Api(api_client)
    authorization = 'authorization_example' # str | 
    name = 'name_example' # str | 
    erc721_request = moonsdk.Erc721Request() # Erc721Request | 

    try:
        api_response = await api_instance.approve(authorization, name, erc721_request)
        print("The response of Erc721Api->approve:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling Erc721Api->approve: %s\n" % e)
```

#### Parameters

| Name                | Type                                  | Description | Notes |
| ------------------- | ------------------------------------- | ----------- | ----- |
| **authorization**   | **str**                               |             |       |
| **name**            | **str**                               |             |       |
| **erc721\_request** | [**Erc721Request**](erc721request.md) |             |       |

#### Return type

[**TransactionAPIResponse**](transactionapiresponse.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

#### HTTP response details

| Status code | Description | Response headers |
| ----------- | ----------- | ---------------- |
| **200**     | Ok          | -                |

[\[Back to top\]](erc721api.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## **balance\_of**

> TransactionAPIResponse balance\_of(authorization, name, erc721\_request)

#### Example

* Api Key Authentication (ApiKeyAuth):
* Api Key Authentication (BearerAuth):

```python
import moonsdk
from moonsdk.models.erc721_request import Erc721Request
from moonsdk.models.transaction_api_response import TransactionAPIResponse
from moonsdk.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://beta.usemoon.ai
# See configuration.py for a list of all supported configuration parameters.
configuration = moonsdk.Configuration(
    host = "https://beta.usemoon.ai"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure API key authorization: ApiKeyAuth
configuration.api_key['ApiKeyAuth'] = os.environ["API_KEY"]

# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['ApiKeyAuth'] = 'Bearer'

# Configure API key authorization: BearerAuth
configuration.api_key['BearerAuth'] = os.environ["API_KEY"]

# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['BearerAuth'] = 'Bearer'

# Enter a context with an instance of the API client
async with moonsdk.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = moonsdk.Erc721Api(api_client)
    authorization = 'authorization_example' # str | 
    name = 'name_example' # str | 
    erc721_request = moonsdk.Erc721Request() # Erc721Request | 

    try:
        api_response = await api_instance.balance_of(authorization, name, erc721_request)
        print("The response of Erc721Api->balance_of:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling Erc721Api->balance_of: %s\n" % e)
```

#### Parameters

| Name                | Type                                  | Description | Notes |
| ------------------- | ------------------------------------- | ----------- | ----- |
| **authorization**   | **str**                               |             |       |
| **name**            | **str**                               |             |       |
| **erc721\_request** | [**Erc721Request**](erc721request.md) |             |       |

#### Return type

[**TransactionAPIResponse**](transactionapiresponse.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

#### HTTP response details

| Status code | Description | Response headers |
| ----------- | ----------- | ---------------- |
| **200**     | Ok          | -                |

[\[Back to top\]](erc721api.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## **get\_approved**

> TransactionAPIResponse get\_approved(authorization, name, erc721\_request)

#### Example

* Api Key Authentication (ApiKeyAuth):
* Api Key Authentication (BearerAuth):

```python
import moonsdk
from moonsdk.models.erc721_request import Erc721Request
from moonsdk.models.transaction_api_response import TransactionAPIResponse
from moonsdk.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://beta.usemoon.ai
# See configuration.py for a list of all supported configuration parameters.
configuration = moonsdk.Configuration(
    host = "https://beta.usemoon.ai"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure API key authorization: ApiKeyAuth
configuration.api_key['ApiKeyAuth'] = os.environ["API_KEY"]

# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['ApiKeyAuth'] = 'Bearer'

# Configure API key authorization: BearerAuth
configuration.api_key['BearerAuth'] = os.environ["API_KEY"]

# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['BearerAuth'] = 'Bearer'

# Enter a context with an instance of the API client
async with moonsdk.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = moonsdk.Erc721Api(api_client)
    authorization = 'authorization_example' # str | 
    name = 'name_example' # str | 
    erc721_request = moonsdk.Erc721Request() # Erc721Request | 

    try:
        api_response = await api_instance.get_approved(authorization, name, erc721_request)
        print("The response of Erc721Api->get_approved:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling Erc721Api->get_approved: %s\n" % e)
```

#### Parameters

| Name                | Type                                  | Description | Notes |
| ------------------- | ------------------------------------- | ----------- | ----- |
| **authorization**   | **str**                               |             |       |
| **name**            | **str**                               |             |       |
| **erc721\_request** | [**Erc721Request**](erc721request.md) |             |       |

#### Return type

[**TransactionAPIResponse**](transactionapiresponse.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

#### HTTP response details

| Status code | Description | Response headers |
| ----------- | ----------- | ---------------- |
| **200**     | Ok          | -                |

[\[Back to top\]](erc721api.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## **is\_approved\_for\_all**

> TransactionAPIResponse is\_approved\_for\_all(authorization, name, erc721\_request)

#### Example

* Api Key Authentication (ApiKeyAuth):
* Api Key Authentication (BearerAuth):

```python
import moonsdk
from moonsdk.models.erc721_request import Erc721Request
from moonsdk.models.transaction_api_response import TransactionAPIResponse
from moonsdk.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://beta.usemoon.ai
# See configuration.py for a list of all supported configuration parameters.
configuration = moonsdk.Configuration(
    host = "https://beta.usemoon.ai"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure API key authorization: ApiKeyAuth
configuration.api_key['ApiKeyAuth'] = os.environ["API_KEY"]

# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['ApiKeyAuth'] = 'Bearer'

# Configure API key authorization: BearerAuth
configuration.api_key['BearerAuth'] = os.environ["API_KEY"]

# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['BearerAuth'] = 'Bearer'

# Enter a context with an instance of the API client
async with moonsdk.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = moonsdk.Erc721Api(api_client)
    authorization = 'authorization_example' # str | 
    name = 'name_example' # str | 
    erc721_request = moonsdk.Erc721Request() # Erc721Request | 

    try:
        api_response = await api_instance.is_approved_for_all(authorization, name, erc721_request)
        print("The response of Erc721Api->is_approved_for_all:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling Erc721Api->is_approved_for_all: %s\n" % e)
```

#### Parameters

| Name                | Type                                  | Description | Notes |
| ------------------- | ------------------------------------- | ----------- | ----- |
| **authorization**   | **str**                               |             |       |
| **name**            | **str**                               |             |       |
| **erc721\_request** | [**Erc721Request**](erc721request.md) |             |       |

#### Return type

[**TransactionAPIResponse**](transactionapiresponse.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

#### HTTP response details

| Status code | Description | Response headers |
| ----------- | ----------- | ---------------- |
| **200**     | Ok          | -                |

[\[Back to top\]](erc721api.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## **name**

> TransactionAPIResponse name(authorization, name, erc721\_request)

#### Example

* Api Key Authentication (ApiKeyAuth):
* Api Key Authentication (BearerAuth):

```python
import moonsdk
from moonsdk.models.erc721_request import Erc721Request
from moonsdk.models.transaction_api_response import TransactionAPIResponse
from moonsdk.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://beta.usemoon.ai
# See configuration.py for a list of all supported configuration parameters.
configuration = moonsdk.Configuration(
    host = "https://beta.usemoon.ai"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure API key authorization: ApiKeyAuth
configuration.api_key['ApiKeyAuth'] = os.environ["API_KEY"]

# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['ApiKeyAuth'] = 'Bearer'

# Configure API key authorization: BearerAuth
configuration.api_key['BearerAuth'] = os.environ["API_KEY"]

# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['BearerAuth'] = 'Bearer'

# Enter a context with an instance of the API client
async with moonsdk.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = moonsdk.Erc721Api(api_client)
    authorization = 'authorization_example' # str | 
    name = 'name_example' # str | 
    erc721_request = moonsdk.Erc721Request() # Erc721Request | 

    try:
        api_response = await api_instance.name(authorization, name, erc721_request)
        print("The response of Erc721Api->name:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling Erc721Api->name: %s\n" % e)
```

#### Parameters

| Name                | Type                                  | Description | Notes |
| ------------------- | ------------------------------------- | ----------- | ----- |
| **authorization**   | **str**                               |             |       |
| **name**            | **str**                               |             |       |
| **erc721\_request** | [**Erc721Request**](erc721request.md) |             |       |

#### Return type

[**TransactionAPIResponse**](transactionapiresponse.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

#### HTTP response details

| Status code | Description | Response headers |
| ----------- | ----------- | ---------------- |
| **200**     | Ok          | -                |

[\[Back to top\]](erc721api.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## **owner\_of**

> TransactionAPIResponse owner\_of(authorization, name, erc721\_request)

#### Example

* Api Key Authentication (ApiKeyAuth):
* Api Key Authentication (BearerAuth):

```python
import moonsdk
from moonsdk.models.erc721_request import Erc721Request
from moonsdk.models.transaction_api_response import TransactionAPIResponse
from moonsdk.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://beta.usemoon.ai
# See configuration.py for a list of all supported configuration parameters.
configuration = moonsdk.Configuration(
    host = "https://beta.usemoon.ai"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure API key authorization: ApiKeyAuth
configuration.api_key['ApiKeyAuth'] = os.environ["API_KEY"]

# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['ApiKeyAuth'] = 'Bearer'

# Configure API key authorization: BearerAuth
configuration.api_key['BearerAuth'] = os.environ["API_KEY"]

# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['BearerAuth'] = 'Bearer'

# Enter a context with an instance of the API client
async with moonsdk.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = moonsdk.Erc721Api(api_client)
    authorization = 'authorization_example' # str | 
    name = 'name_example' # str | 
    erc721_request = moonsdk.Erc721Request() # Erc721Request | 

    try:
        api_response = await api_instance.owner_of(authorization, name, erc721_request)
        print("The response of Erc721Api->owner_of:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling Erc721Api->owner_of: %s\n" % e)
```

#### Parameters

| Name                | Type                                  | Description | Notes |
| ------------------- | ------------------------------------- | ----------- | ----- |
| **authorization**   | **str**                               |             |       |
| **name**            | **str**                               |             |       |
| **erc721\_request** | [**Erc721Request**](erc721request.md) |             |       |

#### Return type

[**TransactionAPIResponse**](transactionapiresponse.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

#### HTTP response details

| Status code | Description | Response headers |
| ----------- | ----------- | ---------------- |
| **200**     | Ok          | -                |

[\[Back to top\]](erc721api.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## **safe\_transfer\_from**

> TransactionAPIResponse safe\_transfer\_from(authorization, name, erc721\_request)

#### Example

* Api Key Authentication (ApiKeyAuth):
* Api Key Authentication (BearerAuth):

```python
import moonsdk
from moonsdk.models.erc721_request import Erc721Request
from moonsdk.models.transaction_api_response import TransactionAPIResponse
from moonsdk.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://beta.usemoon.ai
# See configuration.py for a list of all supported configuration parameters.
configuration = moonsdk.Configuration(
    host = "https://beta.usemoon.ai"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure API key authorization: ApiKeyAuth
configuration.api_key['ApiKeyAuth'] = os.environ["API_KEY"]

# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['ApiKeyAuth'] = 'Bearer'

# Configure API key authorization: BearerAuth
configuration.api_key['BearerAuth'] = os.environ["API_KEY"]

# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['BearerAuth'] = 'Bearer'

# Enter a context with an instance of the API client
async with moonsdk.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = moonsdk.Erc721Api(api_client)
    authorization = 'authorization_example' # str | 
    name = 'name_example' # str | 
    erc721_request = moonsdk.Erc721Request() # Erc721Request | 

    try:
        api_response = await api_instance.safe_transfer_from(authorization, name, erc721_request)
        print("The response of Erc721Api->safe_transfer_from:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling Erc721Api->safe_transfer_from: %s\n" % e)
```

#### Parameters

| Name                | Type                                  | Description | Notes |
| ------------------- | ------------------------------------- | ----------- | ----- |
| **authorization**   | **str**                               |             |       |
| **name**            | **str**                               |             |       |
| **erc721\_request** | [**Erc721Request**](erc721request.md) |             |       |

#### Return type

[**TransactionAPIResponse**](transactionapiresponse.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

#### HTTP response details

| Status code | Description | Response headers |
| ----------- | ----------- | ---------------- |
| **200**     | Ok          | -                |

[\[Back to top\]](erc721api.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## **set\_approval\_for\_all**

> TransactionAPIResponse set\_approval\_for\_all(authorization, name, erc721\_request)

#### Example

* Api Key Authentication (ApiKeyAuth):
* Api Key Authentication (BearerAuth):

```python
import moonsdk
from moonsdk.models.erc721_request import Erc721Request
from moonsdk.models.transaction_api_response import TransactionAPIResponse
from moonsdk.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://beta.usemoon.ai
# See configuration.py for a list of all supported configuration parameters.
configuration = moonsdk.Configuration(
    host = "https://beta.usemoon.ai"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure API key authorization: ApiKeyAuth
configuration.api_key['ApiKeyAuth'] = os.environ["API_KEY"]

# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['ApiKeyAuth'] = 'Bearer'

# Configure API key authorization: BearerAuth
configuration.api_key['BearerAuth'] = os.environ["API_KEY"]

# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['BearerAuth'] = 'Bearer'

# Enter a context with an instance of the API client
async with moonsdk.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = moonsdk.Erc721Api(api_client)
    authorization = 'authorization_example' # str | 
    name = 'name_example' # str | 
    erc721_request = moonsdk.Erc721Request() # Erc721Request | 

    try:
        api_response = await api_instance.set_approval_for_all(authorization, name, erc721_request)
        print("The response of Erc721Api->set_approval_for_all:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling Erc721Api->set_approval_for_all: %s\n" % e)
```

#### Parameters

| Name                | Type                                  | Description | Notes |
| ------------------- | ------------------------------------- | ----------- | ----- |
| **authorization**   | **str**                               |             |       |
| **name**            | **str**                               |             |       |
| **erc721\_request** | [**Erc721Request**](erc721request.md) |             |       |

#### Return type

[**TransactionAPIResponse**](transactionapiresponse.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

#### HTTP response details

| Status code | Description | Response headers |
| ----------- | ----------- | ---------------- |
| **200**     | Ok          | -                |

[\[Back to top\]](erc721api.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## **symbol**

> TransactionAPIResponse symbol(authorization, name, erc721\_request)

#### Example

* Api Key Authentication (ApiKeyAuth):
* Api Key Authentication (BearerAuth):

```python
import moonsdk
from moonsdk.models.erc721_request import Erc721Request
from moonsdk.models.transaction_api_response import TransactionAPIResponse
from moonsdk.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://beta.usemoon.ai
# See configuration.py for a list of all supported configuration parameters.
configuration = moonsdk.Configuration(
    host = "https://beta.usemoon.ai"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure API key authorization: ApiKeyAuth
configuration.api_key['ApiKeyAuth'] = os.environ["API_KEY"]

# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['ApiKeyAuth'] = 'Bearer'

# Configure API key authorization: BearerAuth
configuration.api_key['BearerAuth'] = os.environ["API_KEY"]

# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['BearerAuth'] = 'Bearer'

# Enter a context with an instance of the API client
async with moonsdk.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = moonsdk.Erc721Api(api_client)
    authorization = 'authorization_example' # str | 
    name = 'name_example' # str | 
    erc721_request = moonsdk.Erc721Request() # Erc721Request | 

    try:
        api_response = await api_instance.symbol(authorization, name, erc721_request)
        print("The response of Erc721Api->symbol:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling Erc721Api->symbol: %s\n" % e)
```

#### Parameters

| Name                | Type                                  | Description | Notes |
| ------------------- | ------------------------------------- | ----------- | ----- |
| **authorization**   | **str**                               |             |       |
| **name**            | **str**                               |             |       |
| **erc721\_request** | [**Erc721Request**](erc721request.md) |             |       |

#### Return type

[**TransactionAPIResponse**](transactionapiresponse.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

#### HTTP response details

| Status code | Description | Response headers |
| ----------- | ----------- | ---------------- |
| **200**     | Ok          | -                |

[\[Back to top\]](erc721api.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## **token\_uri**

> TransactionAPIResponse token\_uri(authorization, name, erc721\_request)

#### Example

* Api Key Authentication (ApiKeyAuth):
* Api Key Authentication (BearerAuth):

```python
import moonsdk
from moonsdk.models.erc721_request import Erc721Request
from moonsdk.models.transaction_api_response import TransactionAPIResponse
from moonsdk.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://beta.usemoon.ai
# See configuration.py for a list of all supported configuration parameters.
configuration = moonsdk.Configuration(
    host = "https://beta.usemoon.ai"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure API key authorization: ApiKeyAuth
configuration.api_key['ApiKeyAuth'] = os.environ["API_KEY"]

# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['ApiKeyAuth'] = 'Bearer'

# Configure API key authorization: BearerAuth
configuration.api_key['BearerAuth'] = os.environ["API_KEY"]

# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['BearerAuth'] = 'Bearer'

# Enter a context with an instance of the API client
async with moonsdk.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = moonsdk.Erc721Api(api_client)
    authorization = 'authorization_example' # str | 
    name = 'name_example' # str | 
    erc721_request = moonsdk.Erc721Request() # Erc721Request | 

    try:
        api_response = await api_instance.token_uri(authorization, name, erc721_request)
        print("The response of Erc721Api->token_uri:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling Erc721Api->token_uri: %s\n" % e)
```

#### Parameters

| Name                | Type                                  | Description | Notes |
| ------------------- | ------------------------------------- | ----------- | ----- |
| **authorization**   | **str**                               |             |       |
| **name**            | **str**                               |             |       |
| **erc721\_request** | [**Erc721Request**](erc721request.md) |             |       |

#### Return type

[**TransactionAPIResponse**](transactionapiresponse.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

#### HTTP response details

| Status code | Description | Response headers |
| ----------- | ----------- | ---------------- |
| **200**     | Ok          | -                |

[\[Back to top\]](erc721api.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## **transfer**

> TransactionAPIResponse transfer(authorization, name, erc721\_request)

#### Example

* Api Key Authentication (ApiKeyAuth):
* Api Key Authentication (BearerAuth):

```python
import moonsdk
from moonsdk.models.erc721_request import Erc721Request
from moonsdk.models.transaction_api_response import TransactionAPIResponse
from moonsdk.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://beta.usemoon.ai
# See configuration.py for a list of all supported configuration parameters.
configuration = moonsdk.Configuration(
    host = "https://beta.usemoon.ai"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure API key authorization: ApiKeyAuth
configuration.api_key['ApiKeyAuth'] = os.environ["API_KEY"]

# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['ApiKeyAuth'] = 'Bearer'

# Configure API key authorization: BearerAuth
configuration.api_key['BearerAuth'] = os.environ["API_KEY"]

# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['BearerAuth'] = 'Bearer'

# Enter a context with an instance of the API client
async with moonsdk.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = moonsdk.Erc721Api(api_client)
    authorization = 'authorization_example' # str | 
    name = 'name_example' # str | 
    erc721_request = moonsdk.Erc721Request() # Erc721Request | 

    try:
        api_response = await api_instance.transfer(authorization, name, erc721_request)
        print("The response of Erc721Api->transfer:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling Erc721Api->transfer: %s\n" % e)
```

#### Parameters

| Name                | Type                                  | Description | Notes |
| ------------------- | ------------------------------------- | ----------- | ----- |
| **authorization**   | **str**                               |             |       |
| **name**            | **str**                               |             |       |
| **erc721\_request** | [**Erc721Request**](erc721request.md) |             |       |

#### Return type

[**TransactionAPIResponse**](transactionapiresponse.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

#### HTTP response details

| Status code | Description | Response headers |
| ----------- | ----------- | ---------------- |
| **200**     | Ok          | -                |

[\[Back to top\]](erc721api.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## **transfer\_from**

> TransactionAPIResponse transfer\_from(authorization, name, erc721\_request)

#### Example

* Api Key Authentication (ApiKeyAuth):
* Api Key Authentication (BearerAuth):

```python
import moonsdk
from moonsdk.models.erc721_request import Erc721Request
from moonsdk.models.transaction_api_response import TransactionAPIResponse
from moonsdk.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://beta.usemoon.ai
# See configuration.py for a list of all supported configuration parameters.
configuration = moonsdk.Configuration(
    host = "https://beta.usemoon.ai"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure API key authorization: ApiKeyAuth
configuration.api_key['ApiKeyAuth'] = os.environ["API_KEY"]

# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['ApiKeyAuth'] = 'Bearer'

# Configure API key authorization: BearerAuth
configuration.api_key['BearerAuth'] = os.environ["API_KEY"]

# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['BearerAuth'] = 'Bearer'

# Enter a context with an instance of the API client
async with moonsdk.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = moonsdk.Erc721Api(api_client)
    authorization = 'authorization_example' # str | 
    name = 'name_example' # str | 
    erc721_request = moonsdk.Erc721Request() # Erc721Request | 

    try:
        api_response = await api_instance.transfer_from(authorization, name, erc721_request)
        print("The response of Erc721Api->transfer_from:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling Erc721Api->transfer_from: %s\n" % e)
```

#### Parameters

| Name                | Type                                  | Description | Notes |
| ------------------- | ------------------------------------- | ----------- | ----- |
| **authorization**   | **str**                               |             |       |
| **name**            | **str**                               |             |       |
| **erc721\_request** | [**Erc721Request**](erc721request.md) |             |       |

#### Return type

[**TransactionAPIResponse**](transactionapiresponse.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

#### HTTP response details

| Status code | Description | Response headers |
| ----------- | ----------- | ---------------- |
| **200**     | Ok          | -                |

[\[Back to top\]](erc721api.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)
