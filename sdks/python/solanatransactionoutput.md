# SolanaTransactionOutput

## Properties

| Name                  | Type    | Description | Notes       |
| --------------------- | ------- | ----------- | ----------- |
| **signed\_tx**        | **str** |             | \[optional] |
| **transaction\_hash** | **str** |             | \[optional] |

## Example

```python
from moonsdk.models.solana_transaction_output import SolanaTransactionOutput

# TODO update the JSON string below
json = "{}"
# create an instance of SolanaTransactionOutput from a JSON string
solana_transaction_output_instance = SolanaTransactionOutput.from_json(json)
# print the JSON string representation of the object
print(SolanaTransactionOutput.to_json())

# convert the object into a dict
solana_transaction_output_dict = solana_transaction_output_instance.to_dict()
# create an instance of SolanaTransactionOutput from a dict
solana_transaction_output_form_dict = solana_transaction_output.from_dict(solana_transaction_output_dict)
```

[\[Back to Model list\]](./#documentation-for-models) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to README\]](./)
