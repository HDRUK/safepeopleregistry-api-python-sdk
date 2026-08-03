# ExperienceIndex200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | [optional] 
**data** | [**ExperienceIndex200ResponseData**](ExperienceIndex200ResponseData.md) |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.experience_index200_response import ExperienceIndex200Response

# TODO update the JSON string below
json = "{}"
# create an instance of ExperienceIndex200Response from a JSON string
experience_index200_response_instance = ExperienceIndex200Response.from_json(json)
# print the JSON string representation of the object
print(ExperienceIndex200Response.to_json())

# convert the object into a dict
experience_index200_response_dict = experience_index200_response_instance.to_dict()
# create an instance of ExperienceIndex200Response from a dict
experience_index200_response_from_dict = ExperienceIndex200Response.from_dict(experience_index200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


