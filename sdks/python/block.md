# Block

## Properties

| Name          | Type    | Description | Notes |
| ------------- | ------- | ----------- | ----- |
| **number**    | **str** |             |       |
| **hash**      | **str** |             |       |
| **timestamp** | **str** |             |       |

## Example

```python
from moonsdk.models.block import Block

# TODO update the JSON string below
json = "{}"
# create an instance of Block from a JSON string
block_instance = Block.from_json(json)
# print the JSON string representation of the object
print Block.to_json()

# convert the object into a dict
block_dict = block_instance.to_dict()
# create an instance of Block from a dict
block_form_dict = block.from_dict(block_dict)
```

[\[Back to Model list\]](./#documentation-for-models) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to README\]](./)
