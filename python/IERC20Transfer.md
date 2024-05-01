# IERC20Transfer

## Properties

| Name                      | Type                                          | Description | Notes       |
| ------------------------- | --------------------------------------------- | ----------- | ----------- |
| **transaction\_hash**     | **str**                                       |             |             |
| **contract**              | **str**                                       |             |             |
| **log\_index**            | **str**                                       |             |             |
| **var\_from**             | **str**                                       |             |             |
| **to**                    | **str**                                       |             |             |
| **value**                 | **str**                                       |             |             |
| **token\_decimals**       | **str**                                       |             |             |
| **token\_name**           | **str**                                       |             |             |
| **token\_symbol**         | **str**                                       |             |             |
| **value\_with\_decimals** | **str**                                       |             | \[optional] |
| **triggers**              | [**List\[TriggerOutput\]**](TriggerOutput.md) |             | \[optional] |

## Example

```python
from moonsdk.models.ierc20_transfer import IERC20Transfer

# TODO update the JSON string below
json = "{}"
# create an instance of IERC20Transfer from a JSON string
ierc20_transfer_instance = IERC20Transfer.from_json(json)
# print the JSON string representation of the object
print IERC20Transfer.to_json()

# convert the object into a dict
ierc20_transfer_dict = ierc20_transfer_instance.to_dict()
# create an instance of IERC20Transfer from a dict
ierc20_transfer_form_dict = ierc20_transfer.from_dict(ierc20_transfer_dict)
```

[\[Back to Model list\]](./#documentation-for-models) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to README\]](./)
