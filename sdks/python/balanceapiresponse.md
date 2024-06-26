# BalanceAPIResponse

## Properties

| Name        | Type                                      | Description | Notes       |
| ----------- | ----------------------------------------- | ----------- | ----------- |
| **success** | **bool**                                  |             |             |
| **message** | **str**                                   |             |             |
| **body**    | [**InputBody**](inputbody.md)             |             | \[optional] |
| **address** | **str**                                   |             | \[optional] |
| **data**    | [**BalanceResponse**](balanceresponse.md) |             | \[optional] |

## Example

```python
from moonsdk.models.balance_api_response import BalanceAPIResponse

# TODO update the JSON string below
json = "{}"
# create an instance of BalanceAPIResponse from a JSON string
balance_api_response_instance = BalanceAPIResponse.from_json(json)
# print the JSON string representation of the object
print(BalanceAPIResponse.to_json())

# convert the object into a dict
balance_api_response_dict = balance_api_response_instance.to_dict()
# create an instance of BalanceAPIResponse from a dict
balance_api_response_form_dict = balance_api_response.from_dict(balance_api_response_dict)
```

[\[Back to Model list\]](./#documentation-for-models) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to README\]](./)
