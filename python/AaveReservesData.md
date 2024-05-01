# AaveReservesData

## Properties

| Name                               | Type    | Description | Notes |
| ---------------------------------- | ------- | ----------- | ----- |
| **current\_atoken\_balance**       | **str** |             |       |
| **current\_borrow\_balance**       | **str** |             |       |
| **principal\_borrow\_balance**     | **str** |             |       |
| **borrow\_rate\_mode**             | **str** |             |       |
| **borrow\_rate**                   | **str** |             |       |
| **liquidity\_rate**                | **str** |             |       |
| **origination\_fee**               | **str** |             |       |
| **variable\_borrow\_index**        | **str** |             |       |
| **last\_update\_timestamp**        | **str** |             |       |
| **usage\_as\_collateral\_enabled** | **str** |             |       |

## Example

```python
from moonsdk.models.aave_reserves_data import AaveReservesData

# TODO update the JSON string below
json = "{}"
# create an instance of AaveReservesData from a JSON string
aave_reserves_data_instance = AaveReservesData.from_json(json)
# print the JSON string representation of the object
print(AaveReservesData.to_json())

# convert the object into a dict
aave_reserves_data_dict = aave_reserves_data_instance.to_dict()
# create an instance of AaveReservesData from a dict
aave_reserves_data_form_dict = aave_reserves_data.from_dict(aave_reserves_data_dict)
```

[\[Back to Model list\]](./#documentation-for-models) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to README\]](./)
