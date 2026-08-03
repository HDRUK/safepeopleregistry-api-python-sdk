# CustodianGetProjectsUsers200ResponseDataDataInnerRegistry


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | [optional] 
**digi_ident** | **str** |  | [optional] 
**verified** | **bool** |  | [optional] 
**user** | [**CustodianGetProjectsUsers200ResponseDataDataInnerRegistryUser**](CustodianGetProjectsUsers200ResponseDataDataInnerRegistryUser.md) |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.custodian_get_projects_users200_response_data_data_inner_registry import CustodianGetProjectsUsers200ResponseDataDataInnerRegistry

# TODO update the JSON string below
json = "{}"
# create an instance of CustodianGetProjectsUsers200ResponseDataDataInnerRegistry from a JSON string
custodian_get_projects_users200_response_data_data_inner_registry_instance = CustodianGetProjectsUsers200ResponseDataDataInnerRegistry.from_json(json)
# print the JSON string representation of the object
print(CustodianGetProjectsUsers200ResponseDataDataInnerRegistry.to_json())

# convert the object into a dict
custodian_get_projects_users200_response_data_data_inner_registry_dict = custodian_get_projects_users200_response_data_data_inner_registry_instance.to_dict()
# create an instance of CustodianGetProjectsUsers200ResponseDataDataInnerRegistry from a dict
custodian_get_projects_users200_response_data_data_inner_registry_from_dict = CustodianGetProjectsUsers200ResponseDataDataInnerRegistry.from_dict(custodian_get_projects_users200_response_data_data_inner_registry_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


