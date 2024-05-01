# INFTTransfer

## Properties

| Name                      | Type                                          | Description | Notes       |
| ------------------------- | --------------------------------------------- | ----------- | ----------- |
| **transaction\_hash**     | **str**                                       |             |             |
| **contract**              | **str**                                       |             |             |
| **log\_index**            | **str**                                       |             |             |
| **token\_contract\_type** | **str**                                       |             |             |
| **token\_name**           | **str**                                       |             |             |
| **token\_symbol**         | **str**                                       |             |             |
| **triggers**              | [**List\[TriggerOutput\]**](triggeroutput.md) |             | \[optional] |
| **operator**              | **str**                                       |             |             |
| **var\_from**             | **str**                                       |             |             |
| **to**                    | **str**                                       |             |             |
| **token\_id**             | **str**                                       |             |             |
| **amount**                | **str**                                       |             |             |

## Example

```python
from moonsdk.models.inft_transfer import INFTTransfer

# TODO update the JSON string below
json = "{}"
# create an instance of INFTTransfer from a JSON string
inft_transfer_instance = INFTTransfer.from_json(json)
# print the JSON string representation of the object
print INFTTransfer.to_json()

# convert the object into a dict
inft_transfer_dict = inft_transfer_instance.to_dict()
# create an instance of INFTTransfer from a dict
inft_transfer_form_dict = inft_transfer.from_dict(inft_transfer_dict)
```

[\[Back to Model list\]](./#documentation-for-models) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to README\]](./)
