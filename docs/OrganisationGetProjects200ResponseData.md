# OrganisationGetProjects200ResponseData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | [optional] 
**created_at** | **str** |  | [optional] 
**updated_at** | **str** |  | [optional] 
**registry_id** | **int** |  | [optional] 
**name** | **str** |  | [optional] 
**public_benefit** | **str** |  | [optional] 
**runs_to** | **str** |  | [optional] 
**affiliate_id** | **int** |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.organisation_get_projects200_response_data import OrganisationGetProjects200ResponseData

# TODO update the JSON string below
json = "{}"
# create an instance of OrganisationGetProjects200ResponseData from a JSON string
organisation_get_projects200_response_data_instance = OrganisationGetProjects200ResponseData.from_json(json)
# print the JSON string representation of the object
print(OrganisationGetProjects200ResponseData.to_json())

# convert the object into a dict
organisation_get_projects200_response_data_dict = organisation_get_projects200_response_data_instance.to_dict()
# create an instance of OrganisationGetProjects200ResponseData from a dict
organisation_get_projects200_response_data_from_dict = OrganisationGetProjects200ResponseData.from_dict(organisation_get_projects200_response_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


