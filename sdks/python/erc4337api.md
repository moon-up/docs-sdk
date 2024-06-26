# Erc4337Api

## moonsdk.Erc4337Api

All URIs are relative to _https://moon-vault-api-git-ew-supabase-migration-moonup.vercel.app_

| Method                                                                           | HTTP request                                             | Description |
| -------------------------------------------------------------------------------- | -------------------------------------------------------- | ----------- |
| [**get\_address**](erc4337api.md#get\_address)                                   | **POST** /erc4337/{accountName}/address                  |             |
| [**sign\_broadcast\_user\_op\_tx**](erc4337api.md#sign\_broadcast\_user\_op\_tx) | **POST** /erc4337/{accountName}/sign-broadcast-userop-tx |             |

## **get\_address**

> AccountAPIResponse get\_address(authorization, account\_name, input\_body)

#### Example

* Api Key Authentication (ApiKeyAuth):
* Api Key Authentication (BearerAuth):

```python
import time
import os
import moonsdk
from moonsdk.models.account_api_response import AccountAPIResponse
from moonsdk.models.input_body import InputBody
from moonsdk.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://moon-vault-api-git-ew-supabase-migration-moonup.vercel.app
# See configuration.py for a list of all supported configuration parameters.
configuration = moonsdk.Configuration(
    host = "https://moon-vault-api-git-ew-supabase-migration-moonup.vercel.app"
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
    api_instance = moonsdk.Erc4337Api(api_client)
    authorization = 'authorization_example' # str | 
    account_name = 'account_name_example' # str | 
    input_body = moonsdk.InputBody() # InputBody | 

    try:
        api_response = await api_instance.get_address(authorization, account_name, input_body)
        print("The response of Erc4337Api->get_address:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling Erc4337Api->get_address: %s\n" % e)
```

#### Parameters

| Name              | Type                          | Description | Notes |
| ----------------- | ----------------------------- | ----------- | ----- |
| **authorization** | **str**                       |             |       |
| **account\_name** | **str**                       |             |       |
| **input\_body**   | [**InputBody**](inputbody.md) |             |       |

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

[\[Back to top\]](erc4337api.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## **sign\_broadcast\_user\_op\_tx**

> TransactionAPIResponse sign\_broadcast\_user\_op\_tx(authorization, account\_name, input\_body)

#### Example

* Api Key Authentication (ApiKeyAuth):
* Api Key Authentication (BearerAuth):

```python
import time
import os
import moonsdk
from moonsdk.models.input_body import InputBody
from moonsdk.models.transaction_api_response import TransactionAPIResponse
from moonsdk.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://moon-vault-api-git-ew-supabase-migration-moonup.vercel.app
# See configuration.py for a list of all supported configuration parameters.
configuration = moonsdk.Configuration(
    host = "https://moon-vault-api-git-ew-supabase-migration-moonup.vercel.app"
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
    api_instance = moonsdk.Erc4337Api(api_client)
    authorization = 'authorization_example' # str | 
    account_name = 'account_name_example' # str | 
    input_body = moonsdk.InputBody() # InputBody | 

    try:
        api_response = await api_instance.sign_broadcast_user_op_tx(authorization, account_name, input_body)
        print("The response of Erc4337Api->sign_broadcast_user_op_tx:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling Erc4337Api->sign_broadcast_user_op_tx: %s\n" % e)
```

#### Parameters

| Name              | Type                          | Description | Notes |
| ----------------- | ----------------------------- | ----------- | ----- |
| **authorization** | **str**                       |             |       |
| **account\_name** | **str**                       |             |       |
| **input\_body**   | [**InputBody**](inputbody.md) |             |       |

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

[\[Back to top\]](erc4337api.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)
