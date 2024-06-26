# EosAPIResponse

## Properties

| Name        | Type                                                | Description | Notes       |
| ----------- | --------------------------------------------------- | ----------- | ----------- |
| **success** | **bool**                                            |             |             |
| **message** | **str**                                             |             |             |
| **body**    | [**InputBody**](inputbody.md)                       |             | \[optional] |
| **address** | **str**                                             |             | \[optional] |
| **data**    | [**EosTransactionOutput**](eostransactionoutput.md) |             | \[optional] |

## Example

```python
from moonsdk.models.eos_api_response import EosAPIResponse

# TODO update the JSON string below
json = "{}"
# create an instance of EosAPIResponse from a JSON string
eos_api_response_instance = EosAPIResponse.from_json(json)
# print the JSON string representation of the object
print(EosAPIResponse.to_json())

# convert the object into a dict
eos_api_response_dict = eos_api_response_instance.to_dict()
# create an instance of EosAPIResponse from a dict
eos_api_response_form_dict = eos_api_response.from_dict(eos_api_response_dict)
```

[\[Back to Model list\]](./#documentation-for-models) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to README\]](./)
