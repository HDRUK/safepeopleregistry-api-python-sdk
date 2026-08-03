# File

Model representing files

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** | Unique identifier for the file | [optional] 
**name** | **str** | Name of the file | [optional] 
**type** | **str** | Type of the file | [optional] 
**path** | **str** | Path to the file | [optional] 
**status** | **str** | Status of the file | [optional] 
**created_at** | **datetime** | Timestamp when the file was created | [optional] 
**updated_at** | **datetime** | Timestamp when the file was last updated | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.file import File

# TODO update the JSON string below
json = "{}"
# create an instance of File from a JSON string
file_instance = File.from_json(json)
# print the JSON string representation of the object
print(File.to_json())

# convert the object into a dict
file_dict = file_instance.to_dict()
# create an instance of File from a dict
file_from_dict = File.from_dict(file_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


