# TransactionInput

## Properties

| Name                  | Type                                                                      | Description | Notes |
| --------------------- | ------------------------------------------------------------------------- | ----------- | ----- |
| **supported\_params** | [**TransactionInputSupportedParams**](transactioninputsupportedparams.md) |             |       |
| **wallet**            | [**TransactionInputWallet**](transactioninputwallet.md)                   |             |       |
| **meta\_data**        | [**TransactionInputMetaData**](transactioninputmetadata.md)               |             |       |
| **originating\_host** | **str**                                                                   |             |       |
| **partner\_context**  | **str**                                                                   |             |       |
| **uuid**              | **str**                                                                   |             |       |
| **network**           | **str**                                                                   |             |       |
| **payment\_method**   | **str**                                                                   |             |       |
| **type**              | **str**                                                                   |             |       |
| **amount**            | **float**                                                                 |             |       |
| **destination**       | **str**                                                                   |             |       |
| **source**            | **str**                                                                   |             |       |
| **onramp**            | **str**                                                                   |             |       |

## Example

```python
from moonsdk.models.transaction_input import TransactionInput

# TODO update the JSON string below
json = "{}"
# create an instance of TransactionInput from a JSON string
transaction_input_instance = TransactionInput.from_json(json)
# print the JSON string representation of the object
print(TransactionInput.to_json())

# convert the object into a dict
transaction_input_dict = transaction_input_instance.to_dict()
# create an instance of TransactionInput from a dict
transaction_input_form_dict = transaction_input.from_dict(transaction_input_dict)
```

[\[Back to Model list\]](./#documentation-for-models) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to README\]](./)
