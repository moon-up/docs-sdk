# INativeBalance

## Properties

| Name        | Type    | Description | Notes |
| ----------- | ------- | ----------- | ----- |
| **address** | **str** |             |       |
| **balance** | **str** |             |       |

## Example

```python
from moonsdk.models.i_native_balance import INativeBalance

# TODO update the JSON string below
json = "{}"
# create an instance of INativeBalance from a JSON string
i_native_balance_instance = INativeBalance.from_json(json)
# print the JSON string representation of the object
print INativeBalance.to_json()

# convert the object into a dict
i_native_balance_dict = i_native_balance_instance.to_dict()
# create an instance of INativeBalance from a dict
i_native_balance_form_dict = i_native_balance.from_dict(i_native_balance_dict)
```

[\[Back to Model list\]](./#documentation-for-models) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to README\]](./)
