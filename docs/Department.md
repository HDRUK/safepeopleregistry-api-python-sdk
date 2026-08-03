# Department

Model representing departments

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** | Unique identifier for the department | [optional] 
**name** | **str** | Name of the department | [optional] 
**category** | **str** | Category of the department | [optional] 
**created_at** | **datetime** | Timestamp when the department was created | [optional] 
**updated_at** | **datetime** | Timestamp when the department was last updated | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.department import Department

# TODO update the JSON string below
json = "{}"
# create an instance of Department from a JSON string
department_instance = Department.from_json(json)
# print the JSON string representation of the object
print(Department.to_json())

# convert the object into a dict
department_dict = department_instance.to_dict()
# create an instance of Department from a dict
department_from_dict = Department.from_dict(department_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


