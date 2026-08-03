# Training

Training model

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | [optional] 
**created_at** | **str** |  | [optional] 
**updated_at** | **str** |  | [optional] 
**registry_id** | **int** |  | [optional] 
**provider** | **str** |  | [optional] 
**awarded_at** | **str** |  | [optional] 
**expires_at** | **str** |  | [optional] 
**expires_in_years** | **int** |  | [optional] 
**training_name** | **str** |  | [optional] 
**pro_registration** | **int** |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.training import Training

# TODO update the JSON string below
json = "{}"
# create an instance of Training from a JSON string
training_instance = Training.from_json(json)
# print the JSON string representation of the object
print(Training.to_json())

# convert the object into a dict
training_dict = training_instance.to_dict()
# create an instance of Training from a dict
training_from_dict = Training.from_dict(training_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


