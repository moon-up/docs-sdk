# TokenSwapParams

## Properties

| Name                     | Type      | Description | Notes       |
| ------------------------ | --------- | ----------- | ----------- |
| **to**                   | **str**   |             | \[optional] |
| **data**                 | **str**   |             | \[optional] |
| **input**                | **str**   |             | \[optional] |
| **value**                | **str**   |             | \[optional] |
| **nonce**                | **str**   |             | \[optional] |
| **gas**                  | **str**   |             | \[optional] |
| **gas\_price**           | **str**   |             | \[optional] |
| **chain\_id**            | **str**   |             | \[optional] |
| **encoding**             | **str**   |             | \[optional] |
| **eoa**                  | **bool**  |             | \[optional] |
| **contract\_address**    | **str**   |             | \[optional] |
| **token\_id**            | **str**   |             | \[optional] |
| **token\_ids**           | **str**   |             | \[optional] |
| **approved**             | **bool**  |             | \[optional] |
| **broadcast**            | **bool**  |             | \[optional] |
| **token\_in**            | **str**   |             |             |
| **token\_out**           | **str**   |             |             |
| **token\_in\_decimals**  | **float** |             |             |
| **token\_out\_decimals** | **float** |             |             |
| **amount\_in**           | **str**   |             |             |
| **slippage**             | **str**   |             |             |
| **recipient**            | **str**   |             |             |
| **referrer**             | **str**   |             |             |

## Example

```python
from moonsdk.models.token_swap_params import TokenSwapParams

# TODO update the JSON string below
json = "{}"
# create an instance of TokenSwapParams from a JSON string
token_swap_params_instance = TokenSwapParams.from_json(json)
# print the JSON string representation of the object
print(TokenSwapParams.to_json())

# convert the object into a dict
token_swap_params_dict = token_swap_params_instance.to_dict()
# create an instance of TokenSwapParams from a dict
token_swap_params_form_dict = token_swap_params.from_dict(token_swap_params_dict)
```

[\[Back to Model list\]](./#documentation-for-models) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to README\]](./)
