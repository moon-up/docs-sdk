# INFTApprovalERC721

## Properties

| Name                      | Type    | Description | Notes |
| ------------------------- | ------- | ----------- | ----- |
| **transaction\_hash**     | **str** |             |       |
| **contract**              | **str** |             |       |
| **log\_index**            | **str** |             |       |
| **owner**                 | **str** |             |       |
| **approved**              | **str** |             |       |
| **token\_id**             | **str** |             |       |
| **token\_contract\_type** | **str** |             |       |
| **token\_name**           | **str** |             |       |
| **token\_symbol**         | **str** |             |       |

## Example

```python
from moonsdk.models.inft_approval_erc721 import INFTApprovalERC721

# TODO update the JSON string below
json = "{}"
# create an instance of INFTApprovalERC721 from a JSON string
inft_approval_erc721_instance = INFTApprovalERC721.from_json(json)
# print the JSON string representation of the object
print INFTApprovalERC721.to_json()

# convert the object into a dict
inft_approval_erc721_dict = inft_approval_erc721_instance.to_dict()
# create an instance of INFTApprovalERC721 from a dict
inft_approval_erc721_form_dict = inft_approval_erc721.from_dict(inft_approval_erc721_dict)
```

[\[Back to Model list\]](./#documentation-for-models) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to README\]](./)
