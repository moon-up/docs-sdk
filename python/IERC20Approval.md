# IERC20Approval

## Properties

| Name                      | Type                                          | Description | Notes       |
| ------------------------- | --------------------------------------------- | ----------- | ----------- |
| **transaction\_hash**     | **str**                                       |             |             |
| **contract**              | **str**                                       |             |             |
| **log\_index**            | **str**                                       |             |             |
| **owner**                 | **str**                                       |             |             |
| **spender**               | **str**                                       |             |             |
| **value**                 | **str**                                       |             |             |
| **token\_decimals**       | **str**                                       |             |             |
| **token\_name**           | **str**                                       |             |             |
| **token\_symbol**         | **str**                                       |             |             |
| **value\_with\_decimals** | **str**                                       |             | \[optional] |
| **triggers**              | [**List\[TriggerOutput\]**](TriggerOutput.md) |             | \[optional] |

## Example

```python
from moonsdk.models.ierc20_approval import IERC20Approval

# TODO update the JSON string below
json = "{}"
# create an instance of IERC20Approval from a JSON string
ierc20_approval_instance = IERC20Approval.from_json(json)
# print the JSON string representation of the object
print IERC20Approval.to_json()

# convert the object into a dict
ierc20_approval_dict = ierc20_approval_instance.to_dict()
# create an instance of IERC20Approval from a dict
ierc20_approval_form_dict = ierc20_approval.from_dict(ierc20_approval_dict)
```

[\[Back to Model list\]](./#documentation-for-models) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to README\]](./)
