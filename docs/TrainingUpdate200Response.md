# TrainingUpdate200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | [optional] 
**data** | [**Training**](Training.md) |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.training_update200_response import TrainingUpdate200Response

# TODO update the JSON string below
json = "{}"
# create an instance of TrainingUpdate200Response from a JSON string
training_update200_response_instance = TrainingUpdate200Response.from_json(json)
# print the JSON string representation of the object
print(TrainingUpdate200Response.to_json())

# convert the object into a dict
training_update200_response_dict = training_update200_response_instance.to_dict()
# create an instance of TrainingUpdate200Response from a dict
training_update200_response_from_dict = TrainingUpdate200Response.from_dict(training_update200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


