# ONSFile

Model representing ONS files

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** | Unique identifier for the ONS file | [optional] 
**name** | **str** | Name of the ONS file | [optional] 
**path** | **str** | Path to the ONS file | [optional] 
**status** | **str** | Status of the ONS file | [optional] 
**created_at** | **datetime** | Timestamp when the ONS file was created | [optional] 
**updated_at** | **datetime** | Timestamp when the ONS file was last updated | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.ons_file import ONSFile

# TODO update the JSON string below
json = "{}"
# create an instance of ONSFile from a JSON string
ons_file_instance = ONSFile.from_json(json)
# print the JSON string representation of the object
print(ONSFile.to_json())

# convert the object into a dict
ons_file_dict = ons_file_instance.to_dict()
# create an instance of ONSFile from a dict
ons_file_from_dict = ONSFile.from_dict(ons_file_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


