# ExperienceShow200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | [optional] 
**data** | [**Experience**](Experience.md) |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.experience_show200_response import ExperienceShow200Response

# TODO update the JSON string below
json = "{}"
# create an instance of ExperienceShow200Response from a JSON string
experience_show200_response_instance = ExperienceShow200Response.from_json(json)
# print the JSON string representation of the object
print(ExperienceShow200Response.to_json())

# convert the object into a dict
experience_show200_response_dict = experience_show200_response_instance.to_dict()
# create an instance of ExperienceShow200Response from a dict
experience_show200_response_from_dict = ExperienceShow200Response.from_dict(experience_show200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


