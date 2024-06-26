# AbiInput

## Properties

| Name               | Type                                | Description | Notes       |
| ------------------ | ----------------------------------- | ----------- | ----------- |
| **name**           | **str**                             |             |             |
| **type**           | **str**                             |             |             |
| **indexed**        | **bool**                            |             | \[optional] |
| **components**     | [**List\[AbiInput\]**](abiinput.md) |             | \[optional] |
| **internal\_type** | **str**                             |             | \[optional] |

## Example

```python
from moonsdk.models.abi_input import AbiInput

# TODO update the JSON string below
json = "{}"
# create an instance of AbiInput from a JSON string
abi_input_instance = AbiInput.from_json(json)
# print the JSON string representation of the object
print AbiInput.to_json()

# convert the object into a dict
abi_input_dict = abi_input_instance.to_dict()
# create an instance of AbiInput from a dict
abi_input_form_dict = abi_input.from_dict(abi_input_dict)
```

[\[Back to Model list\]](./#documentation-for-models) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to README\]](./)
