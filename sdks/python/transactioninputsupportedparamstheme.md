# TransactionInputSupportedParamsTheme

## Properties

| Name                       | Type      | Description | Notes |
| -------------------------- | --------- | ----------- | ----- |
| **border\_radius**         | **float** |             |       |
| **card\_color**            | **str**   |             |       |
| **secondary\_text\_color** | **str**   |             |       |
| **primary\_text\_color**   | **str**   |             |       |
| **secondary\_color**       | **str**   |             |       |
| **primary\_color**         | **str**   |             |       |
| **theme\_name**            | **str**   |             |       |
| **is\_dark**               | **bool**  |             |       |

## Example

```python
from moonsdk.models.transaction_input_supported_params_theme import TransactionInputSupportedParamsTheme

# TODO update the JSON string below
json = "{}"
# create an instance of TransactionInputSupportedParamsTheme from a JSON string
transaction_input_supported_params_theme_instance = TransactionInputSupportedParamsTheme.from_json(json)
# print the JSON string representation of the object
print(TransactionInputSupportedParamsTheme.to_json())

# convert the object into a dict
transaction_input_supported_params_theme_dict = transaction_input_supported_params_theme_instance.to_dict()
# create an instance of TransactionInputSupportedParamsTheme from a dict
transaction_input_supported_params_theme_form_dict = transaction_input_supported_params_theme.from_dict(transaction_input_supported_params_theme_dict)
```

[\[Back to Model list\]](./#documentation-for-models) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to README\]](./)
