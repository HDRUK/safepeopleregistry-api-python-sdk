# OrganisationGetUsers200ResponseData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**current_page** | **int** |  | [optional] 
**data** | [**List[OrganisationGetUsers200ResponseDataDataInner]**](OrganisationGetUsers200ResponseDataDataInner.md) |  | [optional] 
**first_page_url** | **str** |  | [optional] 
**var_from** | **int** |  | [optional] 
**last_page** | **int** |  | [optional] 
**last_page_url** | **str** |  | [optional] 
**next_page_url** | **str** |  | [optional] 
**path** | **str** |  | [optional] 
**per_page** | **int** |  | [optional] 
**prev_page_url** | **str** |  | [optional] 
**to** | **int** |  | [optional] 
**total** | **int** |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.organisation_get_users200_response_data import OrganisationGetUsers200ResponseData

# TODO update the JSON string below
json = "{}"
# create an instance of OrganisationGetUsers200ResponseData from a JSON string
organisation_get_users200_response_data_instance = OrganisationGetUsers200ResponseData.from_json(json)
# print the JSON string representation of the object
print(OrganisationGetUsers200ResponseData.to_json())

# convert the object into a dict
organisation_get_users200_response_data_dict = organisation_get_users200_response_data_instance.to_dict()
# create an instance of OrganisationGetUsers200ResponseData from a dict
organisation_get_users200_response_data_from_dict = OrganisationGetUsers200ResponseData.from_dict(organisation_get_users200_response_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


