# EosApi

## moonsdk.EosApi

All URIs are relative to _https://beta.usemoon.ai_

| Method                                                         | HTTP request                        | Description |
| -------------------------------------------------------------- | ----------------------------------- | ----------- |
| [**create\_eos\_account**](eosapi.md#create\_eos\_account)     | **POST** /eos                       |             |
| [**get\_eos\_account**](eosapi.md#get\_eos\_account)           | **GET** /eos/{accountName}          |             |
| [**list\_eos\_accounts**](eosapi.md#list\_eos\_accounts)       | **GET** /eos                        |             |
| [**sign\_eos\_transaction**](eosapi.md#sign\_eos\_transaction) | **POST** /eos/{accountName}/sign-tx |             |

## **create\_eos\_account**

> AccountAPIResponse create\_eos\_account(authorization, eos\_input)

#### Example

* Api Key Authentication (ApiKeyAuth):
* Api Key Authentication (BearerAuth):

```python
import moonsdk
from moonsdk.models.account_api_response import AccountAPIResponse
from moonsdk.models.eos_input import EosInput
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
    api_instance = moonsdk.EosApi(api_client)
    authorization = 'authorization_example' # str | 
    eos_input = moonsdk.EosInput() # EosInput | 

    try:
        api_response = await api_instance.create_eos_account(authorization, eos_input)
        print("The response of EosApi->create_eos_account:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EosApi->create_eos_account: %s\n" % e)
```

#### Parameters

| Name              | Type                        | Description | Notes |
| ----------------- | --------------------------- | ----------- | ----- |
| **authorization** | **str**                     |             |       |
| **eos\_input**    | [**EosInput**](eosinput.md) |             |       |

#### Return type

[**AccountAPIResponse**](accountapiresponse.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

#### HTTP response details

| Status code | Description | Response headers |
| ----------- | ----------- | ---------------- |
| **200**     | Ok          | -                |

[\[Back to top\]](eosapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## **get\_eos\_account**

> AccountAPIResponse get\_eos\_account(authorization, account\_name)

#### Example

* Api Key Authentication (ApiKeyAuth):
* Api Key Authentication (BearerAuth):

```python
import moonsdk
from moonsdk.models.account_api_response import AccountAPIResponse
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
    api_instance = moonsdk.EosApi(api_client)
    authorization = 'authorization_example' # str | 
    account_name = 'account_name_example' # str | 

    try:
        api_response = await api_instance.get_eos_account(authorization, account_name)
        print("The response of EosApi->get_eos_account:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EosApi->get_eos_account: %s\n" % e)
```

#### Parameters

| Name              | Type    | Description | Notes |
| ----------------- | ------- | ----------- | ----- |
| **authorization** | **str** |             |       |
| **account\_name** | **str** |             |       |

#### Return type

[**AccountAPIResponse**](accountapiresponse.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: Not defined
* **Accept**: application/json

#### HTTP response details

| Status code | Description | Response headers |
| ----------- | ----------- | ---------------- |
| **200**     | Ok          | -                |

[\[Back to top\]](eosapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## **list\_eos\_accounts**

> AccountAPIResponse list\_eos\_accounts(authorization)

#### Example

* Api Key Authentication (ApiKeyAuth):
* Api Key Authentication (BearerAuth):

```python
import moonsdk
from moonsdk.models.account_api_response import AccountAPIResponse
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
    api_instance = moonsdk.EosApi(api_client)
    authorization = 'authorization_example' # str | 

    try:
        api_response = await api_instance.list_eos_accounts(authorization)
        print("The response of EosApi->list_eos_accounts:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EosApi->list_eos_accounts: %s\n" % e)
```

#### Parameters

| Name              | Type    | Description | Notes |
| ----------------- | ------- | ----------- | ----- |
| **authorization** | **str** |             |       |

#### Return type

[**AccountAPIResponse**](accountapiresponse.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: Not defined
* **Accept**: application/json

#### HTTP response details

| Status code | Description | Response headers |
| ----------- | ----------- | ---------------- |
| **200**     | Ok          | -                |

[\[Back to top\]](eosapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## **sign\_eos\_transaction**

> EosAPIResponse sign\_eos\_transaction(authorization, account\_name, eos\_transaction\_input)

#### Example

* Api Key Authentication (ApiKeyAuth):
* Api Key Authentication (BearerAuth):

```python
import moonsdk
from moonsdk.models.eos_api_response import EosAPIResponse
from moonsdk.models.eos_transaction_input import EosTransactionInput
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
    api_instance = moonsdk.EosApi(api_client)
    authorization = 'authorization_example' # str | 
    account_name = 'account_name_example' # str | 
    eos_transaction_input = moonsdk.EosTransactionInput() # EosTransactionInput | 

    try:
        api_response = await api_instance.sign_eos_transaction(authorization, account_name, eos_transaction_input)
        print("The response of EosApi->sign_eos_transaction:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EosApi->sign_eos_transaction: %s\n" % e)
```

#### Parameters

| Name                        | Type                                              | Description | Notes |
| --------------------------- | ------------------------------------------------- | ----------- | ----- |
| **authorization**           | **str**                                           |             |       |
| **account\_name**           | **str**                                           |             |       |
| **eos\_transaction\_input** | [**EosTransactionInput**](eostransactioninput.md) |             |       |

#### Return type

[**EosAPIResponse**](eosapiresponse.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

#### HTTP response details

| Status code | Description | Response headers |
| ----------- | ----------- | ---------------- |
| **200**     | Ok          | -                |

[\[Back to top\]](eosapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)
