# CustodianProjectOrganisationsGetStatus200ResponseData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | [optional] 
**name** | **str** |  | [optional] 
**model_state** | [**CustodianProjectOrganisationsGetStatus200ResponseDataModelState**](CustodianProjectOrganisationsGetStatus200ResponseDataModelState.md) |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.custodian_project_organisations_get_status200_response_data import CustodianProjectOrganisationsGetStatus200ResponseData

# TODO update the JSON string below
json = "{}"
# create an instance of CustodianProjectOrganisationsGetStatus200ResponseData from a JSON string
custodian_project_organisations_get_status200_response_data_instance = CustodianProjectOrganisationsGetStatus200ResponseData.from_json(json)
# print the JSON string representation of the object
print(CustodianProjectOrganisationsGetStatus200ResponseData.to_json())

# convert the object into a dict
custodian_project_organisations_get_status200_response_data_dict = custodian_project_organisations_get_status200_response_data_instance.to_dict()
# create an instance of CustodianProjectOrganisationsGetStatus200ResponseData from a dict
custodian_project_organisations_get_status200_response_data_from_dict = CustodianProjectOrganisationsGetStatus200ResponseData.from_dict(custodian_project_organisations_get_status200_response_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


