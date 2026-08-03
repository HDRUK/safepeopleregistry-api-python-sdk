# ProjectStoreRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**registry_id** | **int** |  | [optional] 
**name** | **str** |  | [optional] 
**public_benefit** | **str** |  | [optional] 
**runs_to** | **str** |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.project_store_request import ProjectStoreRequest

# TODO update the JSON string below
json = "{}"
# create an instance of ProjectStoreRequest from a JSON string
project_store_request_instance = ProjectStoreRequest.from_json(json)
# print the JSON string representation of the object
print(ProjectStoreRequest.to_json())

# convert the object into a dict
project_store_request_dict = project_store_request_instance.to_dict()
# create an instance of ProjectStoreRequest from a dict
project_store_request_from_dict = ProjectStoreRequest.from_dict(project_store_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


