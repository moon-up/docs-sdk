# BitcoincashApi

## moonsdk.BitcoincashApi

All URIs are relative to _https://beta.usemoon.ai_

| Method                                                                                     | HTTP request                                | Description |
| ------------------------------------------------------------------------------------------ | ------------------------------------------- | ----------- |
| [**create\_bitcoin\_cash\_account**](BitcoincashApi.md#create\_bitcoin\_cash\_account)     | **POST** /bitcoincash                       |             |
| [**get\_bitcoin\_cash\_account**](BitcoincashApi.md#get\_bitcoin\_cash\_account)           | **GET** /bitcoincash/{accountName}          |             |
| [**list\_bitcoin\_cash\_accounts**](BitcoincashApi.md#list\_bitcoin\_cash\_accounts)       | **GET** /bitcoincash                        |             |
| [**sign\_bitcoin\_cash\_transaction**](BitcoincashApi.md#sign\_bitcoin\_cash\_transaction) | **POST** /bitcoincash/{accountName}/sign-tx |             |

## **create\_bitcoin\_cash\_account**

> AccountAPIResponse create\_bitcoin\_cash\_account(authorization, bitcoin\_cash\_input)

#### Example

* Api Key Authentication (ApiKeyAuth):
* Api Key Authentication (BearerAuth):

```python
import moonsdk
from moonsdk.models.account_api_response import AccountAPIResponse
from moonsdk.models.bitcoin_cash_input import BitcoinCashInput
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
    api_instance = moonsdk.BitcoincashApi(api_client)
    authorization = 'authorization_example' # str | 
    bitcoin_cash_input = moonsdk.BitcoinCashInput() # BitcoinCashInput | 

    try:
        api_response = await api_instance.create_bitcoin_cash_account(authorization, bitcoin_cash_input)
        print("The response of BitcoincashApi->create_bitcoin_cash_account:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BitcoincashApi->create_bitcoin_cash_account: %s\n" % e)
```

#### Parameters

| Name                     | Type                                        | Description | Notes |
| ------------------------ | ------------------------------------------- | ----------- | ----- |
| **authorization**        | **str**                                     |             |       |
| **bitcoin\_cash\_input** | [**BitcoinCashInput**](BitcoinCashInput.md) |             |       |

#### Return type

[**AccountAPIResponse**](AccountAPIResponse.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

#### HTTP response details

| Status code | Description | Response headers |
| ----------- | ----------- | ---------------- |
| **200**     | Ok          | -                |

[\[Back to top\]](BitcoincashApi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## **get\_bitcoin\_cash\_account**

> AccountAPIResponse get\_bitcoin\_cash\_account(authorization, account\_name)

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
    api_instance = moonsdk.BitcoincashApi(api_client)
    authorization = 'authorization_example' # str | 
    account_name = 'account_name_example' # str | 

    try:
        api_response = await api_instance.get_bitcoin_cash_account(authorization, account_name)
        print("The response of BitcoincashApi->get_bitcoin_cash_account:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BitcoincashApi->get_bitcoin_cash_account: %s\n" % e)
```

#### Parameters

| Name              | Type    | Description | Notes |
| ----------------- | ------- | ----------- | ----- |
| **authorization** | **str** |             |       |
| **account\_name** | **str** |             |       |

#### Return type

[**AccountAPIResponse**](AccountAPIResponse.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: Not defined
* **Accept**: application/json

#### HTTP response details

| Status code | Description | Response headers |
| ----------- | ----------- | ---------------- |
| **200**     | Ok          | -                |

[\[Back to top\]](BitcoincashApi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## **list\_bitcoin\_cash\_accounts**

> AccountAPIResponse list\_bitcoin\_cash\_accounts(authorization)

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
    api_instance = moonsdk.BitcoincashApi(api_client)
    authorization = 'authorization_example' # str | 

    try:
        api_response = await api_instance.list_bitcoin_cash_accounts(authorization)
        print("The response of BitcoincashApi->list_bitcoin_cash_accounts:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BitcoincashApi->list_bitcoin_cash_accounts: %s\n" % e)
```

#### Parameters

| Name              | Type    | Description | Notes |
| ----------------- | ------- | ----------- | ----- |
| **authorization** | **str** |             |       |

#### Return type

[**AccountAPIResponse**](AccountAPIResponse.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: Not defined
* **Accept**: application/json

#### HTTP response details

| Status code | Description | Response headers |
| ----------- | ----------- | ---------------- |
| **200**     | Ok          | -                |

[\[Back to top\]](BitcoincashApi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## **sign\_bitcoin\_cash\_transaction**

> BitcoinCashAPIResponse sign\_bitcoin\_cash\_transaction(authorization, account\_name, bitcoin\_cash\_transaction\_input)

#### Example

* Api Key Authentication (ApiKeyAuth):
* Api Key Authentication (BearerAuth):

```python
import moonsdk
from moonsdk.models.bitcoin_cash_api_response import BitcoinCashAPIResponse
from moonsdk.models.bitcoin_cash_transaction_input import BitcoinCashTransactionInput
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
    api_instance = moonsdk.BitcoincashApi(api_client)
    authorization = 'authorization_example' # str | 
    account_name = 'account_name_example' # str | 
    bitcoin_cash_transaction_input = moonsdk.BitcoinCashTransactionInput() # BitcoinCashTransactionInput | 

    try:
        api_response = await api_instance.sign_bitcoin_cash_transaction(authorization, account_name, bitcoin_cash_transaction_input)
        print("The response of BitcoincashApi->sign_bitcoin_cash_transaction:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BitcoincashApi->sign_bitcoin_cash_transaction: %s\n" % e)
```

#### Parameters

| Name                                  | Type                                                              | Description | Notes |
| ------------------------------------- | ----------------------------------------------------------------- | ----------- | ----- |
| **authorization**                     | **str**                                                           |             |       |
| **account\_name**                     | **str**                                                           |             |       |
| **bitcoin\_cash\_transaction\_input** | [**BitcoinCashTransactionInput**](BitcoinCashTransactionInput.md) |             |       |

#### Return type

[**BitcoinCashAPIResponse**](BitcoinCashAPIResponse.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

#### HTTP response details

| Status code | Description | Response headers |
| ----------- | ----------- | ---------------- |
| **200**     | Ok          | -                |

[\[Back to top\]](BitcoincashApi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)
