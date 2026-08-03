# TrainingShow200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | [optional] 
**data** | [**Training**](Training.md) |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.training_show200_response import TrainingShow200Response

# TODO update the JSON string below
json = "{}"
# create an instance of TrainingShow200Response from a JSON string
training_show200_response_instance = TrainingShow200Response.from_json(json)
# print the JSON string representation of the object
print(TrainingShow200Response.to_json())

# convert the object into a dict
training_show200_response_dict = training_show200_response_instance.to_dict()
# create an instance of TrainingShow200Response from a dict
training_show200_response_from_dict = TrainingShow200Response.from_dict(training_show200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


