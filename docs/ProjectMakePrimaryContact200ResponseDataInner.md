# ProjectMakePrimaryContact200ResponseDataInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**project_id** | **int** |  | [optional] 
**user_digital_ident** | **str** |  | [optional] 
**registry** | [**ProjectMakePrimaryContact200ResponseDataInnerRegistry**](ProjectMakePrimaryContact200ResponseDataInnerRegistry.md) |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.project_make_primary_contact200_response_data_inner import ProjectMakePrimaryContact200ResponseDataInner

# TODO update the JSON string below
json = "{}"
# create an instance of ProjectMakePrimaryContact200ResponseDataInner from a JSON string
project_make_primary_contact200_response_data_inner_instance = ProjectMakePrimaryContact200ResponseDataInner.from_json(json)
# print the JSON string representation of the object
print(ProjectMakePrimaryContact200ResponseDataInner.to_json())

# convert the object into a dict
project_make_primary_contact200_response_data_inner_dict = project_make_primary_contact200_response_data_inner_instance.to_dict()
# create an instance of ProjectMakePrimaryContact200ResponseDataInner from a dict
project_make_primary_contact200_response_data_inner_from_dict = ProjectMakePrimaryContact200ResponseDataInner.from_dict(project_make_primary_contact200_response_data_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


