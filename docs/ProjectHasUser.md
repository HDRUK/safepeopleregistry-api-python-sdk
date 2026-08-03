# ProjectHasUser


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**project** | [**Project**](Project.md) |  | [optional] 
**role** | [**ProjectRole**](ProjectRole.md) |  | [optional] 
**affiliation** | [**Affiliation**](Affiliation.md) |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.project_has_user import ProjectHasUser

# TODO update the JSON string below
json = "{}"
# create an instance of ProjectHasUser from a JSON string
project_has_user_instance = ProjectHasUser.from_json(json)
# print the JSON string representation of the object
print(ProjectHasUser.to_json())

# convert the object into a dict
project_has_user_dict = project_has_user_instance.to_dict()
# create an instance of ProjectHasUser from a dict
project_has_user_from_dict = ProjectHasUser.from_dict(project_has_user_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


