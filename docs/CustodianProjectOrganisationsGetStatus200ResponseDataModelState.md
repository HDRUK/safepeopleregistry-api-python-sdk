# CustodianProjectOrganisationsGetStatus200ResponseDataModelState


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | [optional] 
**state** | [**CustodianProjectOrganisationsGetStatus200ResponseDataModelStateState**](CustodianProjectOrganisationsGetStatus200ResponseDataModelStateState.md) |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.custodian_project_organisations_get_status200_response_data_model_state import CustodianProjectOrganisationsGetStatus200ResponseDataModelState

# TODO update the JSON string below
json = "{}"
# create an instance of CustodianProjectOrganisationsGetStatus200ResponseDataModelState from a JSON string
custodian_project_organisations_get_status200_response_data_model_state_instance = CustodianProjectOrganisationsGetStatus200ResponseDataModelState.from_json(json)
# print the JSON string representation of the object
print(CustodianProjectOrganisationsGetStatus200ResponseDataModelState.to_json())

# convert the object into a dict
custodian_project_organisations_get_status200_response_data_model_state_dict = custodian_project_organisations_get_status200_response_data_model_state_instance.to_dict()
# create an instance of CustodianProjectOrganisationsGetStatus200ResponseDataModelState from a dict
custodian_project_organisations_get_status200_response_data_model_state_from_dict = CustodianProjectOrganisationsGetStatus200ResponseDataModelState.from_dict(custodian_project_organisations_get_status200_response_data_model_state_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


