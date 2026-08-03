# ExperienceStoreRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | [optional] 
**created_at** | **str** |  | [optional] 
**updated_at** | **str** |  | [optional] 
**project_id** | **int** |  | [optional] 
**var_from** | **str** |  | [optional] 
**to** | **str** |  | [optional] 
**organisation_id** | **int** |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.experience_store_request import ExperienceStoreRequest

# TODO update the JSON string below
json = "{}"
# create an instance of ExperienceStoreRequest from a JSON string
experience_store_request_instance = ExperienceStoreRequest.from_json(json)
# print the JSON string representation of the object
print(ExperienceStoreRequest.to_json())

# convert the object into a dict
experience_store_request_dict = experience_store_request_instance.to_dict()
# create an instance of ExperienceStoreRequest from a dict
experience_store_request_from_dict = ExperienceStoreRequest.from_dict(experience_store_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


