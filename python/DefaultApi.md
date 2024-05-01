# DefaultApi

## moonsdk.DefaultApi

All URIs are relative to _https://beta.usemoon.ai_

| Method                                         | HTTP request  | Description |
| ---------------------------------------------- | ------------- | ----------- |
| [**get\_message**](DefaultApi.md#get\_message) | **GET** /ping |             |

## **get\_message**

> PingResponse get\_message()

#### Example

```python
import moonsdk
from moonsdk.models.ping_response import PingResponse
from moonsdk.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://beta.usemoon.ai
# See configuration.py for a list of all supported configuration parameters.
configuration = moonsdk.Configuration(
    host = "https://beta.usemoon.ai"
)


# Enter a context with an instance of the API client
async with moonsdk.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = moonsdk.DefaultApi(api_client)

    try:
        api_response = await api_instance.get_message()
        print("The response of DefaultApi->get_message:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->get_message: %s\n" % e)
```

#### Parameters

This endpoint does not need any parameter.

#### Return type

[**PingResponse**](PingResponse.md)

#### Authorization

No authorization required

#### HTTP request headers

* **Content-Type**: Not defined
* **Accept**: application/json

#### HTTP response details

| Status code | Description | Response headers |
| ----------- | ----------- | ---------------- |
| **200**     | Ok          | -                |

[\[Back to top\]](DefaultApi.md) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to Model list\]](./#documentation-for-models) [\[Back to README\]](./)
