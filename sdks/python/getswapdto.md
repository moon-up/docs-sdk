# GetSwapDto

## Properties

| Name                      | Type      | Description | Notes       |
| ------------------------- | --------- | ----------- | ----------- |
| **src**                   | **str**   |             |             |
| **dst**                   | **str**   |             |             |
| **amount**                | **str**   |             |             |
| **var\_from**             | **str**   |             |             |
| **slippage**              | **float** |             |             |
| **protocols**             | **str**   |             | \[optional] |
| **fee**                   | **str**   |             | \[optional] |
| **disable\_estimate**     | **bool**  |             | \[optional] |
| **permit**                | **str**   |             | \[optional] |
| **include\_tokens\_info** | **bool**  |             | \[optional] |
| **include\_protocols**    | **bool**  |             | \[optional] |
| **compatibility**         | **bool**  |             | \[optional] |
| **allow\_partial\_fill**  | **bool**  |             | \[optional] |
| **parts**                 | **str**   |             | \[optional] |
| **main\_route\_parts**    | **str**   |             | \[optional] |
| **connector\_tokens**     | **str**   |             | \[optional] |
| **complexity\_level**     | **str**   |             | \[optional] |
| **gas\_limit**            | **str**   |             | \[optional] |
| **gas\_price**            | **str**   |             | \[optional] |
| **referrer**              | **str**   |             | \[optional] |
| **receiver**              | **str**   |             | \[optional] |
| **chain\_id**             | **float** |             | \[optional] |

## Example

```python
from moonsdk.models.get_swap_dto import GetSwapDto

# TODO update the JSON string below
json = "{}"
# create an instance of GetSwapDto from a JSON string
get_swap_dto_instance = GetSwapDto.from_json(json)
# print the JSON string representation of the object
print(GetSwapDto.to_json())

# convert the object into a dict
get_swap_dto_dict = get_swap_dto_instance.to_dict()
# create an instance of GetSwapDto from a dict
get_swap_dto_form_dict = get_swap_dto.from_dict(get_swap_dto_dict)
```

[\[Back to Model list\]](./#documentation-for-models) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to README\]](./)
