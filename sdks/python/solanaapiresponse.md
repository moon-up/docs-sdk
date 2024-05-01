# SolanaAPIResponse

## Properties

| Name        | Type                                                      | Description | Notes       |
| ----------- | --------------------------------------------------------- | ----------- | ----------- |
| **success** | **bool**                                                  |             |             |
| **message** | **str**                                                   |             |             |
| **body**    | [**InputBody**](inputbody.md)                             |             | \[optional] |
| **address** | **str**                                                   |             | \[optional] |
| **data**    | [**SolanaTransactionOutput**](solanatransactionoutput.md) |             | \[optional] |

## Example

```python
from moonsdk.models.solana_api_response import SolanaAPIResponse

# TODO update the JSON string below
json = "{}"
# create an instance of SolanaAPIResponse from a JSON string
solana_api_response_instance = SolanaAPIResponse.from_json(json)
# print the JSON string representation of the object
print(SolanaAPIResponse.to_json())

# convert the object into a dict
solana_api_response_dict = solana_api_response_instance.to_dict()
# create an instance of SolanaAPIResponse from a dict
solana_api_response_form_dict = solana_api_response.from_dict(solana_api_response_dict)
```

[\[Back to Model list\]](./#documentation-for-models) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to README\]](./)
