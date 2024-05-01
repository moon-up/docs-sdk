# INFTApproval

## Properties

| Name                      | Type     | Description | Notes |
| ------------------------- | -------- | ----------- | ----- |
| **transaction\_hash**     | **str**  |             |       |
| **contract**              | **str**  |             |       |
| **log\_index**            | **str**  |             |       |
| **token\_contract\_type** | **str**  |             |       |
| **token\_name**           | **str**  |             |       |
| **token\_symbol**         | **str**  |             |       |
| **account**               | **str**  |             |       |
| **operator**              | **str**  |             |       |
| **approved\_all**         | **bool** |             |       |
| **token\_id**             | **str**  |             |       |

## Example

```python
from moonsdk.models.inft_approval import INFTApproval

# TODO update the JSON string below
json = "{}"
# create an instance of INFTApproval from a JSON string
inft_approval_instance = INFTApproval.from_json(json)
# print the JSON string representation of the object
print INFTApproval.to_json()

# convert the object into a dict
inft_approval_dict = inft_approval_instance.to_dict()
# create an instance of INFTApproval from a dict
inft_approval_form_dict = inft_approval.from_dict(inft_approval_dict)
```

[\[Back to Model list\]](./#documentation-for-models) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to README\]](./)
