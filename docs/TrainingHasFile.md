# TrainingHasFile

Pivot model representing the relationship between trainings and files

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**training_id** | **int** | ID of the training | [optional] 
**file_id** | **int** | ID of the file | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.training_has_file import TrainingHasFile

# TODO update the JSON string below
json = "{}"
# create an instance of TrainingHasFile from a JSON string
training_has_file_instance = TrainingHasFile.from_json(json)
# print the JSON string representation of the object
print(TrainingHasFile.to_json())

# convert the object into a dict
training_has_file_dict = training_has_file_instance.to_dict()
# create an instance of TrainingHasFile from a dict
training_has_file_from_dict = TrainingHasFile.from_dict(training_has_file_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


