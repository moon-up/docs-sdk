# BitcoinApi

## moonsdk.BitcoinApi

All URIs are relative to _https://beta.usemoon.ai_

| Method                                                                     | HTTP request                            | Description |
| -------------------------------------------------------------------------- | --------------------------------------- | ----------- |
| [**create\_bitcoin\_account**](bitcoinapi.md#create\_bitcoin\_account)     | **POST** /bitcoin                       |             |
| [**get\_bitcoin\_account**](bitcoinapi.md#get\_bitcoin\_account)           | **GET** /bitcoin/{accountName}          |             |
| [**list\_bitcoin\_accounts**](bitcoinapi.md#list\_bitcoin\_accounts)       | **GET** /bitcoin                        |             |
| [**sign\_bitcoin\_transaction**](bitcoinapi.md#sign\_bitcoin\_transaction) | **POST** /bitcoin/{accountName}/sign-tx |             |

## **create\_bitcoin\_account**

> AccountAPIResponse create\_bitcoin\_account(authorization, bitcoin\_input)

#### Example

* Api Key Authentication (ApiKeyAuth):
* Api Key Authentication (BearerAuth):

```python
import moonsdk
from moonsdk.models.account_api_response import AccountAPIResponse
from moonsdk.models.bitcoin_input import BitcoinInput
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
    api_instance = moonsdk.BitcoinApi(api_client)
    authorization = 'authorization_example' # str | 
    bitcoin_input = moonsdk.BitcoinInput() # BitcoinInput | 

    try:
        api_response = await api_instance.create_bitcoin_account(authorization, bitcoin_input)
        print("The response of BitcoinApi->create_bitcoin_account:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BitcoinApi->create_bitcoin_account: %s\n" % e)
```

#### Parameters

| Name               | Type                                | Description | Notes |
| ------------------ | ----------------------------------- | ----------- | ----- |
| **authorization**  | **str**                             |             |       |
| **bitcoin\_input** | [**BitcoinInput**](bitcoininput.md) |             |       |

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

[\[Back to top\]](bitcoinapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## **get\_bitcoin\_account**

> AccountAPIResponse get\_bitcoin\_account(authorization, account\_name)

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
    api_instance = moonsdk.BitcoinApi(api_client)
    authorization = 'authorization_example' # str | 
    account_name = 'account_name_example' # str | 

    try:
        api_response = await api_instance.get_bitcoin_account(authorization, account_name)
        print("The response of BitcoinApi->get_bitcoin_account:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BitcoinApi->get_bitcoin_account: %s\n" % e)
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

[\[Back to top\]](bitcoinapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## **list\_bitcoin\_accounts**

> AccountAPIResponse list\_bitcoin\_accounts(authorization)

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
    api_instance = moonsdk.BitcoinApi(api_client)
    authorization = 'authorization_example' # str | 

    try:
        api_response = await api_instance.list_bitcoin_accounts(authorization)
        print("The response of BitcoinApi->list_bitcoin_accounts:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BitcoinApi->list_bitcoin_accounts: %s\n" % e)
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

[\[Back to top\]](bitcoinapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## **sign\_bitcoin\_transaction**

> BitcoinAPIResponse sign\_bitcoin\_transaction(authorization, account\_name, bitcoin\_transaction\_input)

#### Example

* Api Key Authentication (ApiKeyAuth):
* Api Key Authentication (BearerAuth):

```python
import moonsdk
from moonsdk.models.bitcoin_api_response import BitcoinAPIResponse
from moonsdk.models.bitcoin_transaction_input import BitcoinTransactionInput
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
    api_instance = moonsdk.BitcoinApi(api_client)
    authorization = 'authorization_example' # str | 
    account_name = 'account_name_example' # str | 
    bitcoin_transaction_input = moonsdk.BitcoinTransactionInput() # BitcoinTransactionInput | 

    try:
        api_response = await api_instance.sign_bitcoin_transaction(authorization, account_name, bitcoin_transaction_input)
        print("The response of BitcoinApi->sign_bitcoin_transaction:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BitcoinApi->sign_bitcoin_transaction: %s\n" % e)
```

#### Parameters

| Name                            | Type                                                      | Description | Notes |
| ------------------------------- | --------------------------------------------------------- | ----------- | ----- |
| **authorization**               | **str**                                                   |             |       |
| **account\_name**               | **str**                                                   |             |       |
| **bitcoin\_transaction\_input** | [**BitcoinTransactionInput**](bitcointransactioninput.md) |             |       |

#### Return type

[**BitcoinAPIResponse**](bitcoinapiresponse.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

#### HTTP response details

| Status code | Description | Response headers |
| ----------- | ----------- | ---------------- |
| **200**     | Ok          | -                |

[\[Back to top\]](bitcoinapi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)
