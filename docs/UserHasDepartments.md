# UserHasDepartments

Pivot model representing the relationship between users and departments

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**user_id** | **int** | ID of the user | [optional] 
**department_id** | **int** | ID of the department | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.user_has_departments import UserHasDepartments

# TODO update the JSON string below
json = "{}"
# create an instance of UserHasDepartments from a JSON string
user_has_departments_instance = UserHasDepartments.from_json(json)
# print the JSON string representation of the object
print(UserHasDepartments.to_json())

# convert the object into a dict
user_has_departments_dict = user_has_departments_instance.to_dict()
# create an instance of UserHasDepartments from a dict
user_has_departments_from_dict = UserHasDepartments.from_dict(user_has_departments_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


