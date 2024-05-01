# AccountControllerResponseData

## Properties

| Name                               | Type                                                    | Description | Notes       |
| ---------------------------------- | ------------------------------------------------------- | ----------- | ----------- |
| **nonce**                          | **float**                                               |             |             |
| **balance**                        | **str**                                                 |             |             |
| **transaction\_hash**              | **str**                                                 |             | \[optional] |
| **signed\_transaction**            | **str**                                                 |             | \[optional] |
| **raw\_transaction**               | **str**                                                 |             | \[optional] |
| **data**                           | **str**                                                 |             |             |
| **transactions**                   | [**List\[TransactionData\]**](TransactionData.md)       |             | \[optional] |
| **moon\_scan\_url**                | **str**                                                 |             | \[optional] |
| **signature**                      | **str**                                                 |             | \[optional] |
| **transaction**                    | [**Tx**](Tx.md)                                         |             | \[optional] |
| **user\_ops**                      | [**List\[TransactionRequest\]**](TransactionRequest.md) |             | \[optional] |
| **userop\_transaction**            | **str**                                                 |             | \[optional] |
| **keys**                           | **List\[str]**                                          |             | \[optional] |
| **address**                        | **str**                                                 |             |             |
| **name**                           | **str**                                                 |             | \[optional] |
| **encoding**                       | **str**                                                 |             | \[optional] |
| **header**                         | **bool**                                                |             | \[optional] |
| **signtype**                       | **bool**                                                |             | \[optional] |
| **domain**                         | **str**                                                 |             |             |
| **current\_atoken\_balance**       | **str**                                                 |             |             |
| **current\_borrow\_balance**       | **str**                                                 |             |             |
| **principal\_borrow\_balance**     | **str**                                                 |             |             |
| **borrow\_rate\_mode**             | **str**                                                 |             |             |
| **borrow\_rate**                   | **str**                                                 |             |             |
| **liquidity\_rate**                | **str**                                                 |             |             |
| **origination\_fee**               | **str**                                                 |             |             |
| **variable\_borrow\_index**        | **str**                                                 |             |             |
| **last\_update\_timestamp**        | **str**                                                 |             |             |
| **usage\_as\_collateral\_enabled** | **str**                                                 |             |             |
| **type**                           | **float**                                               |             | \[optional] |
| **chain\_id**                      | **float**                                               |             | \[optional] |
| **gas**                            | **str**                                                 |             | \[optional] |
| **gas\_price**                     | **str**                                                 |             | \[optional] |
| **gas\_tip\_cap**                  | **str**                                                 |             | \[optional] |
| **gas\_fee\_cap**                  | **str**                                                 |             | \[optional] |
| **value**                          | **str**                                                 |             | \[optional] |
| **var\_from**                      | **str**                                                 |             | \[optional] |
| **to**                             | **str**                                                 |             | \[optional] |
| **blob\_gas**                      | **str**                                                 |             | \[optional] |
| **blob\_gas\_fee\_cap**            | **str**                                                 |             | \[optional] |
| **blob\_hashes**                   | **List\[str]**                                          |             | \[optional] |
| **v**                              | **str**                                                 |             | \[optional] |
| **r**                              | **str**                                                 |             | \[optional] |
| **s**                              | **str**                                                 |             | \[optional] |
| **symbol**                         | **str**                                                 |             | \[optional] |
| **decimals**                       | **str**                                                 |             | \[optional] |
| **total\_supply**                  | **str**                                                 |             | \[optional] |
| **contract\_address**              | **str**                                                 |             | \[optional] |
| **balance\_of**                    | **str**                                                 |             | \[optional] |
| **allowance**                      | **str**                                                 |             | \[optional] |
| **balance\_of**                    | **str**                                                 |             | \[optional] |
| **balance\_of\_batch**             | **str**                                                 |             | \[optional] |
| **success**                        | **bool**                                                |             |             |
| **message**                        | **str**                                                 |             |             |
| **signed\_tx**                     | **str**                                                 |             | \[optional] |
| **owner\_of**                      | **str**                                                 |             | \[optional] |
| **token\_uri**                     | **str**                                                 |             | \[optional] |
| **is\_approved\_for\_all**         | **str**                                                 |             | \[optional] |

## Example

```python
from moonsdk.models.account_controller_response_data import AccountControllerResponseData

# TODO update the JSON string below
json = "{}"
# create an instance of AccountControllerResponseData from a JSON string
account_controller_response_data_instance = AccountControllerResponseData.from_json(json)
# print the JSON string representation of the object
print AccountControllerResponseData.to_json()

# convert the object into a dict
account_controller_response_data_dict = account_controller_response_data_instance.to_dict()
# create an instance of AccountControllerResponseData from a dict
account_controller_response_data_form_dict = account_controller_response_data.from_dict(account_controller_response_data_dict)
```

[\[Back to Model list\]](./#documentation-for-models) [\[Back to API list\]](./#documentation-for-api-endpoints) [\[Back to README\]](./)
