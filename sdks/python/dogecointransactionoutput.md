# DogeCoinTransactionOutput

## Properties

| Name                  | Type    | Description | Notes       |
| --------------------- | ------- | ----------- | ----------- |
| **signed\_tx**        | **str** |             | \[optional] |
| **transaction\_hash** | **str** |             | \[optional] |

## Example

```python
from moonsdk.models.doge_coin_transaction_output import DogeCoinTransactionOutput

# TODO update the JSON string below
json = "{}"
# create an instance of DogeCoinTransactionOutput from a JSON string
doge_coin_transaction_output_instance = DogeCoinTransactionOutput.from_json(json)
# print the JSON string representation of the object
print(DogeCoinTransactionOutput.to_json())

# convert the object into a dict
doge_coin_transaction_output_dict = doge_coin_transaction_output_instance.to_dict()
# create an instance of DogeCoinTransactionOutput from a dict
doge_coin_transaction_output_form_dict = doge_coin_transaction_output.from_dict(doge_coin_transaction_output_dict)
```

[\[Back to Model list\]](./#documentation-for-models) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to README\]](./)
