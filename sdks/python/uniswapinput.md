# UniswapInput

## Properties

| Name                  | Type     | Description | Notes       |
| --------------------- | -------- | ----------- | ----------- |
| **to**                | **str**  |             | \[optional] |
| **data**              | **str**  |             | \[optional] |
| **input**             | **str**  |             | \[optional] |
| **value**             | **str**  |             | \[optional] |
| **nonce**             | **str**  |             | \[optional] |
| **gas**               | **str**  |             | \[optional] |
| **gas\_price**        | **str**  |             | \[optional] |
| **chain\_id**         | **str**  |             | \[optional] |
| **encoding**          | **str**  |             | \[optional] |
| **eoa**               | **bool** |             | \[optional] |
| **contract\_address** | **str**  |             | \[optional] |
| **token\_id**         | **str**  |             | \[optional] |
| **token\_ids**        | **str**  |             | \[optional] |
| **approved**          | **bool** |             | \[optional] |
| **broadcast**         | **bool** |             | \[optional] |
| **token\_a**          | **str**  |             | \[optional] |
| **token\_b**          | **str**  |             | \[optional] |
| **amount\_a**         | **str**  |             | \[optional] |
| **amount\_b**         | **str**  |             | \[optional] |

## Example

```python
from moonsdk.models.uniswap_input import UniswapInput

# TODO update the JSON string below
json = "{}"
# create an instance of UniswapInput from a JSON string
uniswap_input_instance = UniswapInput.from_json(json)
# print the JSON string representation of the object
print(UniswapInput.to_json())

# convert the object into a dict
uniswap_input_dict = uniswap_input_instance.to_dict()
# create an instance of UniswapInput from a dict
uniswap_input_form_dict = uniswap_input.from_dict(uniswap_input_dict)
```

[\[Back to Model list\]](./#documentation-for-models) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to README\]](./)
