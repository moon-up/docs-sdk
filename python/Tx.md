# Tx

## Properties

| Name                    | Type           | Description | Notes       |
| ----------------------- | -------------- | ----------- | ----------- |
| **type**                | **float**      |             | \[optional] |
| **chain\_id**           | **float**      |             | \[optional] |
| **data**                | **str**        |             | \[optional] |
| **gas**                 | **str**        |             | \[optional] |
| **gas\_price**          | **str**        |             | \[optional] |
| **gas\_tip\_cap**       | **str**        |             | \[optional] |
| **gas\_fee\_cap**       | **str**        |             | \[optional] |
| **value**               | **str**        |             | \[optional] |
| **nonce**               | **float**      |             | \[optional] |
| **var\_from**           | **str**        |             | \[optional] |
| **to**                  | **str**        |             | \[optional] |
| **blob\_gas**           | **str**        |             | \[optional] |
| **blob\_gas\_fee\_cap** | **str**        |             | \[optional] |
| **blob\_hashes**        | **List\[str]** |             | \[optional] |
| **v**                   | **str**        |             | \[optional] |
| **r**                   | **str**        |             | \[optional] |
| **s**                   | **str**        |             | \[optional] |

## Example

```python
from moonsdk.models.tx import Tx

# TODO update the JSON string below
json = "{}"
# create an instance of Tx from a JSON string
tx_instance = Tx.from_json(json)
# print the JSON string representation of the object
print(Tx.to_json())

# convert the object into a dict
tx_dict = tx_instance.to_dict()
# create an instance of Tx from a dict
tx_form_dict = tx.from_dict(tx_dict)
```

[\[Back to Model list\]](./#documentation-for-models) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to README\]](./)
