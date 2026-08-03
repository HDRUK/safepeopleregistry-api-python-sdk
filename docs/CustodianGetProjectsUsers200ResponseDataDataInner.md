# CustodianGetProjectsUsers200ResponseDataDataInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**project_id** | **int** |  | [optional] 
**user_digital_ident** | **str** |  | [optional] 
**project_role_id** | **int** |  | [optional] 
**primary_contact** | **bool** |  | [optional] 
**affiliation_id** | **int** |  | [optional] 
**role** | [**CustodianGetProjectsUsers200ResponseDataDataInnerRole**](CustodianGetProjectsUsers200ResponseDataDataInnerRole.md) |  | [optional] 
**affiliation** | [**CustodianGetProjectsUsers200ResponseDataDataInnerAffiliation**](CustodianGetProjectsUsers200ResponseDataDataInnerAffiliation.md) |  | [optional] 
**registry** | [**CustodianGetProjectsUsers200ResponseDataDataInnerRegistry**](CustodianGetProjectsUsers200ResponseDataDataInnerRegistry.md) |  | [optional] 
**project** | [**CustodianGetProjectsUsers200ResponseDataDataInnerProject**](CustodianGetProjectsUsers200ResponseDataDataInnerProject.md) |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.custodian_get_projects_users200_response_data_data_inner import CustodianGetProjectsUsers200ResponseDataDataInner

# TODO update the JSON string below
json = "{}"
# create an instance of CustodianGetProjectsUsers200ResponseDataDataInner from a JSON string
custodian_get_projects_users200_response_data_data_inner_instance = CustodianGetProjectsUsers200ResponseDataDataInner.from_json(json)
# print the JSON string representation of the object
print(CustodianGetProjectsUsers200ResponseDataDataInner.to_json())

# convert the object into a dict
custodian_get_projects_users200_response_data_data_inner_dict = custodian_get_projects_users200_response_data_data_inner_instance.to_dict()
# create an instance of CustodianGetProjectsUsers200ResponseDataDataInner from a dict
custodian_get_projects_users200_response_data_data_inner_from_dict = CustodianGetProjectsUsers200ResponseDataDataInner.from_dict(custodian_get_projects_users200_response_data_data_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


