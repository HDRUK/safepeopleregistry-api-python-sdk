# OrganisationGetUsers200ResponseDataDataInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | [optional] 
**first_name** | **str** |  | [optional] 
**last_name** | **str** |  | [optional] 
**email** | **str** |  | [optional] 
**created_at** | **str** |  | [optional] 
**updated_at** | **str** |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.organisation_get_users200_response_data_data_inner import OrganisationGetUsers200ResponseDataDataInner

# TODO update the JSON string below
json = "{}"
# create an instance of OrganisationGetUsers200ResponseDataDataInner from a JSON string
organisation_get_users200_response_data_data_inner_instance = OrganisationGetUsers200ResponseDataDataInner.from_json(json)
# print the JSON string representation of the object
print(OrganisationGetUsers200ResponseDataDataInner.to_json())

# convert the object into a dict
organisation_get_users200_response_data_data_inner_dict = organisation_get_users200_response_data_data_inner_instance.to_dict()
# create an instance of OrganisationGetUsers200ResponseDataDataInner from a dict
organisation_get_users200_response_data_data_inner_from_dict = OrganisationGetUsers200ResponseDataDataInner.from_dict(organisation_get_users200_response_data_data_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


