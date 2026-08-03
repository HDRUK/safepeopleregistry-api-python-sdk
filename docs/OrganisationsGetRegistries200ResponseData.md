# OrganisationsGetRegistries200ResponseData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**current_page** | **int** |  | [optional] 
**data** | [**List[OrganisationsGetRegistries200ResponseDataDataInner]**](OrganisationsGetRegistries200ResponseDataDataInner.md) |  | [optional] 
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
from safepeopleregistry_api_sdk.models.organisations_get_registries200_response_data import OrganisationsGetRegistries200ResponseData

# TODO update the JSON string below
json = "{}"
# create an instance of OrganisationsGetRegistries200ResponseData from a JSON string
organisations_get_registries200_response_data_instance = OrganisationsGetRegistries200ResponseData.from_json(json)
# print the JSON string representation of the object
print(OrganisationsGetRegistries200ResponseData.to_json())

# convert the object into a dict
organisations_get_registries200_response_data_dict = organisations_get_registries200_response_data_instance.to_dict()
# create an instance of OrganisationsGetRegistries200ResponseData from a dict
organisations_get_registries200_response_data_from_dict = OrganisationsGetRegistries200ResponseData.from_dict(organisations_get_registries200_response_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


