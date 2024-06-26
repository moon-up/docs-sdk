# BitcoinCashAPIResponse

## Properties

| Name        | Type                                                                | Description | Notes       |
| ----------- | ------------------------------------------------------------------- | ----------- | ----------- |
| **success** | **bool**                                                            |             |             |
| **message** | **str**                                                             |             |             |
| **body**    | [**InputBody**](inputbody.md)                                       |             | \[optional] |
| **address** | **str**                                                             |             | \[optional] |
| **data**    | [**BitcoinCashTransactionOutput**](bitcoincashtransactionoutput.md) |             | \[optional] |

## Example

```python
from moonsdk.models.bitcoin_cash_api_response import BitcoinCashAPIResponse

# TODO update the JSON string below
json = "{}"
# create an instance of BitcoinCashAPIResponse from a JSON string
bitcoin_cash_api_response_instance = BitcoinCashAPIResponse.from_json(json)
# print the JSON string representation of the object
print(BitcoinCashAPIResponse.to_json())

# convert the object into a dict
bitcoin_cash_api_response_dict = bitcoin_cash_api_response_instance.to_dict()
# create an instance of BitcoinCashAPIResponse from a dict
bitcoin_cash_api_response_form_dict = bitcoin_cash_api_response.from_dict(bitcoin_cash_api_response_dict)
```

[\[Back to Model list\]](./#documentation-for-models) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to README\]](./)
