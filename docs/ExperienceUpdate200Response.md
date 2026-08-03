# ExperienceUpdate200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | [optional] 
**data** | [**Experience**](Experience.md) |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.experience_update200_response import ExperienceUpdate200Response

# TODO update the JSON string below
json = "{}"
# create an instance of ExperienceUpdate200Response from a JSON string
experience_update200_response_instance = ExperienceUpdate200Response.from_json(json)
# print the JSON string representation of the object
print(ExperienceUpdate200Response.to_json())

# convert the object into a dict
experience_update200_response_dict = experience_update200_response_instance.to_dict()
# create an instance of ExperienceUpdate200Response from a dict
experience_update200_response_from_dict = ExperienceUpdate200Response.from_dict(experience_update200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


