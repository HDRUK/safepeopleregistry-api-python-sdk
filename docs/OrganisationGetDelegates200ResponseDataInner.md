# OrganisationGetDelegates200ResponseDataInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | [optional] 
**first_name** | **str** |  | [optional] 
**last_name** | **str** |  | [optional] 
**email** | **str** |  | [optional] 
**created_at** | **datetime** |  | [optional] 
**updated_at** | **datetime** |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.organisation_get_delegates200_response_data_inner import OrganisationGetDelegates200ResponseDataInner

# TODO update the JSON string below
json = "{}"
# create an instance of OrganisationGetDelegates200ResponseDataInner from a JSON string
organisation_get_delegates200_response_data_inner_instance = OrganisationGetDelegates200ResponseDataInner.from_json(json)
# print the JSON string representation of the object
print(OrganisationGetDelegates200ResponseDataInner.to_json())

# convert the object into a dict
organisation_get_delegates200_response_data_inner_dict = organisation_get_delegates200_response_data_inner_instance.to_dict()
# create an instance of OrganisationGetDelegates200ResponseDataInner from a dict
organisation_get_delegates200_response_data_inner_from_dict = OrganisationGetDelegates200ResponseDataInner.from_dict(organisation_get_delegates200_response_data_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


