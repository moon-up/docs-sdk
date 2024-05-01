# PaymentApi

## moonsdk.PaymentApi

All URIs are relative to _https://vault-api.usemoon.ai_

| Method                                                                                       | HTTP request                         | Description |
| -------------------------------------------------------------------------------------------- | ------------------------------------ | ----------- |
| [**create\_payment\_intent\_config**](PaymentApi.md#create\_payment\_intent\_config)         | **POST** /payment/config             |             |
| [**delete\_payment\_intent\_config**](PaymentApi.md#delete\_payment\_intent\_config)         | **DELETE** /payment/config/{id}      |             |
| [**get\_all\_payment\_intent\_configs**](PaymentApi.md#get\_all\_payment\_intent\_configs)   | **GET** /payment/config              |             |
| [**get\_one\_payment\_intent\_configs**](PaymentApi.md#get\_one\_payment\_intent\_configs)   | **GET** /payment/config/{id}         |             |
| [**moralis\_webhook**](PaymentApi.md#moralis\_webhook)                                       | **POST** /payment/webhook/{id}       |             |
| [**payment\_create\_payment\_intent**](PaymentApi.md#payment\_create\_payment\_intent)       | **POST** /payment                    |             |
| [**payment\_delete\_payment\_intent**](PaymentApi.md#payment\_delete\_payment\_intent)       | **DELETE** /payment/{id}             |             |
| [**payment\_get\_all\_payment\_intents**](PaymentApi.md#payment\_get\_all\_payment\_intents) | **GET** /payment                     |             |
| [**payment\_get\_available\_chains**](PaymentApi.md#payment\_get\_available\_chains)         | **GET** /payment/chains              |             |
| [**payment\_get\_payment\_intent**](PaymentApi.md#payment\_get\_payment\_intent)             | **GET** /payment/{id}                |             |
| [**payment\_update\_payment\_intent**](PaymentApi.md#payment\_update\_payment\_intent)       | **PUT** /payment/{id}                |             |
| [**tatum\_webhook**](PaymentApi.md#tatum\_webhook)                                           | **POST** /payment/webhook/tatum/{id} |             |
| [**update\_payment\_intent\_config**](PaymentApi.md#update\_payment\_intent\_config)         | **PUT** /payment/config/{id}         |             |

## **create\_payment\_intent\_config**

> object create\_payment\_intent\_config(authorization, body)

#### Example

* Api Key Authentication (ApiKeyAuth):
* Api Key Authentication (BearerAuth):

```python
import time
import os
import moonsdk
from moonsdk.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://vault-api.usemoon.ai
# See configuration.py for a list of all supported configuration parameters.
configuration = moonsdk.Configuration(
    host = "https://vault-api.usemoon.ai"
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
    api_instance = moonsdk.PaymentApi(api_client)
    authorization = 'authorization_example' # str | 
    body = None # object | 

    try:
        api_response = await api_instance.create_payment_intent_config(authorization, body)
        print("The response of PaymentApi->create_payment_intent_config:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PaymentApi->create_payment_intent_config: %s\n" % e)
```

#### Parameters

| Name              | Type       | Description | Notes |
| ----------------- | ---------- | ----------- | ----- |
| **authorization** | **str**    |             |       |
| **body**          | **object** |             |       |

#### Return type

**object**

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

#### HTTP response details

| Status code | Description | Response headers |
| ----------- | ----------- | ---------------- |
| **200**     | Ok          | -                |

[\[Back to top\]](PaymentApi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## **delete\_payment\_intent\_config**

> PaymentIntentResponse delete\_payment\_intent\_config(authorization, id)

#### Example

* Api Key Authentication (ApiKeyAuth):
* Api Key Authentication (BearerAuth):

```python
import time
import os
import moonsdk
from moonsdk.models.payment_intent_response import PaymentIntentResponse
from moonsdk.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://vault-api.usemoon.ai
# See configuration.py for a list of all supported configuration parameters.
configuration = moonsdk.Configuration(
    host = "https://vault-api.usemoon.ai"
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
    api_instance = moonsdk.PaymentApi(api_client)
    authorization = 'authorization_example' # str | 
    id = 'id_example' # str | 

    try:
        api_response = await api_instance.delete_payment_intent_config(authorization, id)
        print("The response of PaymentApi->delete_payment_intent_config:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PaymentApi->delete_payment_intent_config: %s\n" % e)
```

#### Parameters

| Name              | Type    | Description | Notes |
| ----------------- | ------- | ----------- | ----- |
| **authorization** | **str** |             |       |
| **id**            | **str** |             |       |

#### Return type

[**PaymentIntentResponse**](PaymentIntentResponse.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: Not defined
* **Accept**: application/json

#### HTTP response details

| Status code | Description | Response headers |
| ----------- | ----------- | ---------------- |
| **200**     | Ok          | -                |

[\[Back to top\]](PaymentApi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## **get\_all\_payment\_intent\_configs**

> List\[PaymentIntentResponse] get\_all\_payment\_intent\_configs(authorization)

#### Example

* Api Key Authentication (ApiKeyAuth):
* Api Key Authentication (BearerAuth):

```python
import time
import os
import moonsdk
from moonsdk.models.payment_intent_response import PaymentIntentResponse
from moonsdk.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://vault-api.usemoon.ai
# See configuration.py for a list of all supported configuration parameters.
configuration = moonsdk.Configuration(
    host = "https://vault-api.usemoon.ai"
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
    api_instance = moonsdk.PaymentApi(api_client)
    authorization = 'authorization_example' # str | 

    try:
        api_response = await api_instance.get_all_payment_intent_configs(authorization)
        print("The response of PaymentApi->get_all_payment_intent_configs:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PaymentApi->get_all_payment_intent_configs: %s\n" % e)
```

#### Parameters

| Name              | Type    | Description | Notes |
| ----------------- | ------- | ----------- | ----- |
| **authorization** | **str** |             |       |

#### Return type

[**List\[PaymentIntentResponse\]**](PaymentIntentResponse.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: Not defined
* **Accept**: application/json

#### HTTP response details

| Status code | Description | Response headers |
| ----------- | ----------- | ---------------- |
| **200**     | Ok          | -                |

[\[Back to top\]](PaymentApi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## **get\_one\_payment\_intent\_configs**

> PaymentIntentResponse get\_one\_payment\_intent\_configs(authorization, id)

#### Example

* Api Key Authentication (ApiKeyAuth):
* Api Key Authentication (BearerAuth):

```python
import time
import os
import moonsdk
from moonsdk.models.payment_intent_response import PaymentIntentResponse
from moonsdk.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://vault-api.usemoon.ai
# See configuration.py for a list of all supported configuration parameters.
configuration = moonsdk.Configuration(
    host = "https://vault-api.usemoon.ai"
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
    api_instance = moonsdk.PaymentApi(api_client)
    authorization = 'authorization_example' # str | 
    id = 'id_example' # str | 

    try:
        api_response = await api_instance.get_one_payment_intent_configs(authorization, id)
        print("The response of PaymentApi->get_one_payment_intent_configs:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PaymentApi->get_one_payment_intent_configs: %s\n" % e)
```

#### Parameters

| Name              | Type    | Description | Notes |
| ----------------- | ------- | ----------- | ----- |
| **authorization** | **str** |             |       |
| **id**            | **str** |             |       |

#### Return type

[**PaymentIntentResponse**](PaymentIntentResponse.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: Not defined
* **Accept**: application/json

#### HTTP response details

| Status code | Description | Response headers |
| ----------- | ----------- | ---------------- |
| **200**     | Ok          | -                |

[\[Back to top\]](PaymentApi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## **moralis\_webhook**

> object moralis\_webhook(id, i\_webhook)

#### Example

* Api Key Authentication (ApiKeyAuth):
* Api Key Authentication (BearerAuth):

```python
import time
import os
import moonsdk
from moonsdk.models.i_webhook import IWebhook
from moonsdk.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://vault-api.usemoon.ai
# See configuration.py for a list of all supported configuration parameters.
configuration = moonsdk.Configuration(
    host = "https://vault-api.usemoon.ai"
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
    api_instance = moonsdk.PaymentApi(api_client)
    id = 'id_example' # str | 
    i_webhook = moonsdk.IWebhook() # IWebhook | 

    try:
        api_response = await api_instance.moralis_webhook(id, i_webhook)
        print("The response of PaymentApi->moralis_webhook:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PaymentApi->moralis_webhook: %s\n" % e)
```

#### Parameters

| Name           | Type                        | Description | Notes |
| -------------- | --------------------------- | ----------- | ----- |
| **id**         | **str**                     |             |       |
| **i\_webhook** | [**IWebhook**](IWebhook.md) |             |       |

#### Return type

**object**

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

#### HTTP response details

| Status code | Description | Response headers |
| ----------- | ----------- | ---------------- |
| **200**     | Ok          | -                |

[\[Back to top\]](PaymentApi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## **payment\_create\_payment\_intent**

> PaymentIntentResponse payment\_create\_payment\_intent(authorization, create\_payment\_intent\_input)

#### Example

* Api Key Authentication (ApiKeyAuth):
* Api Key Authentication (BearerAuth):

```python
import time
import os
import moonsdk
from moonsdk.models.create_payment_intent_input import CreatePaymentIntentInput
from moonsdk.models.payment_intent_response import PaymentIntentResponse
from moonsdk.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://vault-api.usemoon.ai
# See configuration.py for a list of all supported configuration parameters.
configuration = moonsdk.Configuration(
    host = "https://vault-api.usemoon.ai"
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
    api_instance = moonsdk.PaymentApi(api_client)
    authorization = 'authorization_example' # str | 
    create_payment_intent_input = moonsdk.CreatePaymentIntentInput() # CreatePaymentIntentInput | 

    try:
        api_response = await api_instance.payment_create_payment_intent(authorization, create_payment_intent_input)
        print("The response of PaymentApi->payment_create_payment_intent:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PaymentApi->payment_create_payment_intent: %s\n" % e)
```

#### Parameters

| Name                               | Type                                                        | Description | Notes |
| ---------------------------------- | ----------------------------------------------------------- | ----------- | ----- |
| **authorization**                  | **str**                                                     |             |       |
| **create\_payment\_intent\_input** | [**CreatePaymentIntentInput**](CreatePaymentIntentInput.md) |             |       |

#### Return type

[**PaymentIntentResponse**](PaymentIntentResponse.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

#### HTTP response details

| Status code | Description | Response headers |
| ----------- | ----------- | ---------------- |
| **200**     | Ok          | -                |

[\[Back to top\]](PaymentApi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## **payment\_delete\_payment\_intent**

> PaymentIntentResponse payment\_delete\_payment\_intent(authorization, id)

#### Example

* Api Key Authentication (ApiKeyAuth):
* Api Key Authentication (BearerAuth):

```python
import time
import os
import moonsdk
from moonsdk.models.payment_intent_response import PaymentIntentResponse
from moonsdk.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://vault-api.usemoon.ai
# See configuration.py for a list of all supported configuration parameters.
configuration = moonsdk.Configuration(
    host = "https://vault-api.usemoon.ai"
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
    api_instance = moonsdk.PaymentApi(api_client)
    authorization = 'authorization_example' # str | 
    id = 'id_example' # str | 

    try:
        api_response = await api_instance.payment_delete_payment_intent(authorization, id)
        print("The response of PaymentApi->payment_delete_payment_intent:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PaymentApi->payment_delete_payment_intent: %s\n" % e)
```

#### Parameters

| Name              | Type    | Description | Notes |
| ----------------- | ------- | ----------- | ----- |
| **authorization** | **str** |             |       |
| **id**            | **str** |             |       |

#### Return type

[**PaymentIntentResponse**](PaymentIntentResponse.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: Not defined
* **Accept**: application/json

#### HTTP response details

| Status code | Description | Response headers |
| ----------- | ----------- | ---------------- |
| **200**     | Ok          | -                |

[\[Back to top\]](PaymentApi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## **payment\_get\_all\_payment\_intents**

> List\[PaymentIntentResponse] payment\_get\_all\_payment\_intents(authorization)

#### Example

* Api Key Authentication (ApiKeyAuth):
* Api Key Authentication (BearerAuth):

```python
import time
import os
import moonsdk
from moonsdk.models.payment_intent_response import PaymentIntentResponse
from moonsdk.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://vault-api.usemoon.ai
# See configuration.py for a list of all supported configuration parameters.
configuration = moonsdk.Configuration(
    host = "https://vault-api.usemoon.ai"
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
    api_instance = moonsdk.PaymentApi(api_client)
    authorization = 'authorization_example' # str | 

    try:
        api_response = await api_instance.payment_get_all_payment_intents(authorization)
        print("The response of PaymentApi->payment_get_all_payment_intents:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PaymentApi->payment_get_all_payment_intents: %s\n" % e)
```

#### Parameters

| Name              | Type    | Description | Notes |
| ----------------- | ------- | ----------- | ----- |
| **authorization** | **str** |             |       |

#### Return type

[**List\[PaymentIntentResponse\]**](PaymentIntentResponse.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: Not defined
* **Accept**: application/json

#### HTTP response details

| Status code | Description | Response headers |
| ----------- | ----------- | ---------------- |
| **200**     | Ok          | -                |

[\[Back to top\]](PaymentApi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## **payment\_get\_available\_chains**

> List\[str] payment\_get\_available\_chains()

#### Example

* Api Key Authentication (ApiKeyAuth):
* Api Key Authentication (BearerAuth):

```python
import time
import os
import moonsdk
from moonsdk.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://vault-api.usemoon.ai
# See configuration.py for a list of all supported configuration parameters.
configuration = moonsdk.Configuration(
    host = "https://vault-api.usemoon.ai"
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
    api_instance = moonsdk.PaymentApi(api_client)

    try:
        api_response = await api_instance.payment_get_available_chains()
        print("The response of PaymentApi->payment_get_available_chains:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PaymentApi->payment_get_available_chains: %s\n" % e)
```

#### Parameters

This endpoint does not need any parameter.

#### Return type

**List\[str]**

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: Not defined
* **Accept**: application/json

#### HTTP response details

| Status code | Description | Response headers |
| ----------- | ----------- | ---------------- |
| **200**     | Ok          | -                |

[\[Back to top\]](PaymentApi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## **payment\_get\_payment\_intent**

> PaymentIntentResponse payment\_get\_payment\_intent(authorization, id)

#### Example

* Api Key Authentication (ApiKeyAuth):
* Api Key Authentication (BearerAuth):

```python
import time
import os
import moonsdk
from moonsdk.models.payment_intent_response import PaymentIntentResponse
from moonsdk.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://vault-api.usemoon.ai
# See configuration.py for a list of all supported configuration parameters.
configuration = moonsdk.Configuration(
    host = "https://vault-api.usemoon.ai"
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
    api_instance = moonsdk.PaymentApi(api_client)
    authorization = 'authorization_example' # str | 
    id = 'id_example' # str | 

    try:
        api_response = await api_instance.payment_get_payment_intent(authorization, id)
        print("The response of PaymentApi->payment_get_payment_intent:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PaymentApi->payment_get_payment_intent: %s\n" % e)
```

#### Parameters

| Name              | Type    | Description | Notes |
| ----------------- | ------- | ----------- | ----- |
| **authorization** | **str** |             |       |
| **id**            | **str** |             |       |

#### Return type

[**PaymentIntentResponse**](PaymentIntentResponse.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: Not defined
* **Accept**: application/json

#### HTTP response details

| Status code | Description | Response headers |
| ----------- | ----------- | ---------------- |
| **200**     | Ok          | -                |

[\[Back to top\]](PaymentApi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## **payment\_update\_payment\_intent**

> PaymentIntentResponse payment\_update\_payment\_intent(authorization, id, create\_payment\_intent\_input)

#### Example

* Api Key Authentication (ApiKeyAuth):
* Api Key Authentication (BearerAuth):

```python
import time
import os
import moonsdk
from moonsdk.models.create_payment_intent_input import CreatePaymentIntentInput
from moonsdk.models.payment_intent_response import PaymentIntentResponse
from moonsdk.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://vault-api.usemoon.ai
# See configuration.py for a list of all supported configuration parameters.
configuration = moonsdk.Configuration(
    host = "https://vault-api.usemoon.ai"
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
    api_instance = moonsdk.PaymentApi(api_client)
    authorization = 'authorization_example' # str | 
    id = 'id_example' # str | 
    create_payment_intent_input = moonsdk.CreatePaymentIntentInput() # CreatePaymentIntentInput | 

    try:
        api_response = await api_instance.payment_update_payment_intent(authorization, id, create_payment_intent_input)
        print("The response of PaymentApi->payment_update_payment_intent:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PaymentApi->payment_update_payment_intent: %s\n" % e)
```

#### Parameters

| Name                               | Type                                                        | Description | Notes |
| ---------------------------------- | ----------------------------------------------------------- | ----------- | ----- |
| **authorization**                  | **str**                                                     |             |       |
| **id**                             | **str**                                                     |             |       |
| **create\_payment\_intent\_input** | [**CreatePaymentIntentInput**](CreatePaymentIntentInput.md) |             |       |

#### Return type

[**PaymentIntentResponse**](PaymentIntentResponse.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

#### HTTP response details

| Status code | Description | Response headers |
| ----------- | ----------- | ---------------- |
| **200**     | Ok          | -                |

[\[Back to top\]](PaymentApi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## **tatum\_webhook**

> object tatum\_webhook(id, tatum\_transaction\_event)

#### Example

* Api Key Authentication (ApiKeyAuth):
* Api Key Authentication (BearerAuth):

```python
import time
import os
import moonsdk
from moonsdk.models.tatum_transaction_event import TatumTransactionEvent
from moonsdk.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://vault-api.usemoon.ai
# See configuration.py for a list of all supported configuration parameters.
configuration = moonsdk.Configuration(
    host = "https://vault-api.usemoon.ai"
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
    api_instance = moonsdk.PaymentApi(api_client)
    id = 'id_example' # str | 
    tatum_transaction_event = moonsdk.TatumTransactionEvent() # TatumTransactionEvent | 

    try:
        api_response = await api_instance.tatum_webhook(id, tatum_transaction_event)
        print("The response of PaymentApi->tatum_webhook:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PaymentApi->tatum_webhook: %s\n" % e)
```

#### Parameters

| Name                          | Type                                                  | Description | Notes |
| ----------------------------- | ----------------------------------------------------- | ----------- | ----- |
| **id**                        | **str**                                               |             |       |
| **tatum\_transaction\_event** | [**TatumTransactionEvent**](TatumTransactionEvent.md) |             |       |

#### Return type

**object**

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

#### HTTP response details

| Status code | Description | Response headers |
| ----------- | ----------- | ---------------- |
| **200**     | Ok          | -                |

[\[Back to top\]](PaymentApi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)

## **update\_payment\_intent\_config**

> PaymentIntentResponse update\_payment\_intent\_config(authorization, id, body)

#### Example

* Api Key Authentication (ApiKeyAuth):
* Api Key Authentication (BearerAuth):

```python
import time
import os
import moonsdk
from moonsdk.models.payment_intent_response import PaymentIntentResponse
from moonsdk.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://vault-api.usemoon.ai
# See configuration.py for a list of all supported configuration parameters.
configuration = moonsdk.Configuration(
    host = "https://vault-api.usemoon.ai"
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
    api_instance = moonsdk.PaymentApi(api_client)
    authorization = 'authorization_example' # str | 
    id = 'id_example' # str | 
    body = None # object | 

    try:
        api_response = await api_instance.update_payment_intent_config(authorization, id, body)
        print("The response of PaymentApi->update_payment_intent_config:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PaymentApi->update_payment_intent_config: %s\n" % e)
```

#### Parameters

| Name              | Type       | Description | Notes |
| ----------------- | ---------- | ----------- | ----- |
| **authorization** | **str**    |             |       |
| **id**            | **str**    |             |       |
| **body**          | **object** |             |       |

#### Return type

[**PaymentIntentResponse**](PaymentIntentResponse.md)

#### Authorization

[ApiKeyAuth](./#ApiKeyAuth), [BearerAuth](./#BearerAuth)

#### HTTP request headers

* **Content-Type**: application/json
* **Accept**: application/json

#### HTTP response details

| Status code | Description | Response headers |
| ----------- | ----------- | ---------------- |
| **200**     | Ok          | -                |

[\[Back to top\]](PaymentApi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)
