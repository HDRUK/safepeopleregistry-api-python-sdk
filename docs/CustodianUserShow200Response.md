# CustodianUserShow200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | [optional] 
**data** | [**CustodianUser**](CustodianUser.md) |  | [optional] 
**user_permissions** | [**List[CustodianUserShow200ResponseUserPermissionsInner]**](CustodianUserShow200ResponseUserPermissionsInner.md) |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.custodian_user_show200_response import CustodianUserShow200Response

# TODO update the JSON string below
json = "{}"
# create an instance of CustodianUserShow200Response from a JSON string
custodian_user_show200_response_instance = CustodianUserShow200Response.from_json(json)
# print the JSON string representation of the object
print(CustodianUserShow200Response.to_json())

# convert the object into a dict
custodian_user_show200_response_dict = custodian_user_show200_response_instance.to_dict()
# create an instance of CustodianUserShow200Response from a dict
custodian_user_show200_response_from_dict = CustodianUserShow200Response.from_dict(custodian_user_show200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


