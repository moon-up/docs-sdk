# AccountResponse

## Properties

| Name     | Type                              | Description | Notes |
| -------- | --------------------------------- | ----------- | ----- |
| **data** | [**AccountData**](accountdata.md) |             |       |

## Example

```python
from moonsdk.models.account_response import AccountResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AccountResponse from a JSON string
account_response_instance = AccountResponse.from_json(json)
# print the JSON string representation of the object
print(AccountResponse.to_json())

# convert the object into a dict
account_response_dict = account_response_instance.to_dict()
# create an instance of AccountResponse from a dict
account_response_form_dict = account_response.from_dict(account_response_dict)
```

[\[Back to Model list\]](./#documentation-for-models) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to README\]](./)
