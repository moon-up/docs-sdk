# SolanaApi

## moonsdk.SolanaApi

All URIs are relative to _https://beta.usemoon.ai_

| Method                                                                  | HTTP request                           | Description |
| ----------------------------------------------------------------------- | -------------------------------------- | ----------- |
| [**create\_solana\_account**](solanaapi.md#create\_solana\_account)     | **POST** /solana                       |             |
| [**get\_solana\_account**](solanaapi.md#get\_solana\_account)           | **GET** /solana/{accountName}          |             |
| [**list\_solana\_accounts**](solanaapi.md#list\_solana\_accounts)       | **GET** /solana                        |             |
| [**sign\_solana\_transaction**](solanaapi.md#sign\_solana\_transaction) | **POST** /solana/{accountName}/sign-tx |             |

## **create\_solana\_account**

> AccountAPIResponse create\_solana\_account(authorization, solana\_input)

#### Example

* Api Key Authentication (ApiKeyAuth):
* Api Key Authentication (BearerAuth):

```python
import moonsdk
from moonsdk.models.account_api_response import AccountAPIResponse
from moonsdk.models.solana_input import SolanaInput
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
    api_instance = moonsdk.SolanaApi(api_client)
    authorization = 'authorization_example' # str | 
    solana_input = moonsdk.SolanaInput() # SolanaInput | 

    try:
        api_response = await api_instance.create_solana_account(authorization, solana_input)
        print("The response of SolanaApi->create_solana_account:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SolanaApi->create_solana_account: %s\n" % e)
```

#### Parameters

| Name              | Type                              | Description | Notes |
| ----------------- | --------------------------------- | ----------- | ----- |
| **authorization** | **str**                           |             |       |
| **solana\_input** | [**SolanaInput**](solanainput.md) |             |       |

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

[\[Back to top\]](solanaapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## **get\_solana\_account**

> AccountAPIResponse get\_solana\_account(authorization, account\_name)

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
    api_instance = moonsdk.SolanaApi(api_client)
    authorization = 'authorization_example' # str | 
    account_name = 'account_name_example' # str | 

    try:
        api_response = await api_instance.get_solana_account(authorization, account_name)
        print("The response of SolanaApi->get_solana_account:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SolanaApi->get_solana_account: %s\n" % e)
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

[\[Back to top\]](solanaapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## **list\_solana\_accounts**

> AccountAPIResponse list\_solana\_accounts(authorization)

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
    api_instance = moonsdk.SolanaApi(api_client)
    authorization = 'authorization_example' # str | 

    try:
        api_response = await api_instance.list_solana_accounts(authorization)
        print("The response of SolanaApi->list_solana_accounts:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SolanaApi->list_solana_accounts: %s\n" % e)
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

[\[Back to top\]](solanaapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## **sign\_solana\_transaction**

> SolanaAPIResponse sign\_solana\_transaction(authorization, account\_name, solana\_transaction\_input)

#### Example

* Api Key Authentication (ApiKeyAuth):
* Api Key Authentication (BearerAuth):

```python
import moonsdk
from moonsdk.models.solana_api_response import SolanaAPIResponse
from moonsdk.models.solana_transaction_input import SolanaTransactionInput
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
    api_instance = moonsdk.SolanaApi(api_client)
    authorization = 'authorization_example' # str | 
    account_name = 'account_name_example' # str | 
    solana_transaction_input = moonsdk.SolanaTransactionInput() # SolanaTransactionInput | 

    try:
        api_response = await api_instance.sign_solana_transaction(authorization, account_name, solana_transaction_input)
        print("The response of SolanaApi->sign_solana_transaction:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SolanaApi->sign_solana_transaction: %s\n" % e)
```

#### Parameters

| Name                           | Type                                                    | Description | Notes |
| ------------------------------ | ------------------------------------------------------- | ----------- | ----- |
| **authorization**              | **str**                                                 |             |       |
| **account\_name**              | **str**                                                 |             |       |
| **solana\_transaction\_input** | [**SolanaTransactionInput**](solanatransactioninput.md) |             |       |

#### Return type

[**SolanaAPIResponse**](solanaapiresponse.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

#### HTTP response details

| Status code | Description | Response headers |
| ----------- | ----------- | ---------------- |
| **200**     | Ok          | -                |

[\[Back to top\]](solanaapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)
