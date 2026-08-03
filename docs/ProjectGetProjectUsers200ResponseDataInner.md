# ProjectGetProjectUsers200ResponseDataInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**project_id** | **int** |  | [optional] 
**user_digital_ident** | **str** |  | [optional] 
**registry** | [**ProjectGetProjectUsers200ResponseDataInnerRegistry**](ProjectGetProjectUsers200ResponseDataInnerRegistry.md) |  | [optional] 
**role** | [**ProjectGetProjectUsers200ResponseDataInnerRole**](ProjectGetProjectUsers200ResponseDataInnerRole.md) |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.project_get_project_users200_response_data_inner import ProjectGetProjectUsers200ResponseDataInner

# TODO update the JSON string below
json = "{}"
# create an instance of ProjectGetProjectUsers200ResponseDataInner from a JSON string
project_get_project_users200_response_data_inner_instance = ProjectGetProjectUsers200ResponseDataInner.from_json(json)
# print the JSON string representation of the object
print(ProjectGetProjectUsers200ResponseDataInner.to_json())

# convert the object into a dict
project_get_project_users200_response_data_inner_dict = project_get_project_users200_response_data_inner_instance.to_dict()
# create an instance of ProjectGetProjectUsers200ResponseDataInner from a dict
project_get_project_users200_response_data_inner_from_dict = ProjectGetProjectUsers200ResponseDataInner.from_dict(project_get_project_users200_response_data_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


