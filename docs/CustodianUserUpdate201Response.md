# CustodianUserUpdate201Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | [optional] 
**data** | [**CustodianUser**](CustodianUser.md) |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.custodian_user_update201_response import CustodianUserUpdate201Response

# TODO update the JSON string below
json = "{}"
# create an instance of CustodianUserUpdate201Response from a JSON string
custodian_user_update201_response_instance = CustodianUserUpdate201Response.from_json(json)
# print the JSON string representation of the object
print(CustodianUserUpdate201Response.to_json())

# convert the object into a dict
custodian_user_update201_response_dict = custodian_user_update201_response_instance.to_dict()
# create an instance of CustodianUserUpdate201Response from a dict
custodian_user_update201_response_from_dict = CustodianUserUpdate201Response.from_dict(custodian_user_update201_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


