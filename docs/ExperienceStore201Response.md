# ExperienceStore201Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | [optional] 
**data** | **int** | ID of the newly created experience | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.experience_store201_response import ExperienceStore201Response

# TODO update the JSON string below
json = "{}"
# create an instance of ExperienceStore201Response from a JSON string
experience_store201_response_instance = ExperienceStore201Response.from_json(json)
# print the JSON string representation of the object
print(ExperienceStore201Response.to_json())

# convert the object into a dict
experience_store201_response_dict = experience_store201_response_instance.to_dict()
# create an instance of ExperienceStore201Response from a dict
experience_store201_response_from_dict = ExperienceStore201Response.from_dict(experience_store201_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


