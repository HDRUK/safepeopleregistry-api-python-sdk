# Endorsement

Model representing endorsements

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** | Unique identifier for the endorsement | [optional] 
**reported_by** | **int** | ID of the user who reported the endorsement | [optional] 
**comment** | **str** | Optional comment provided by the reporter | [optional] 
**raised_against** | **int** | ID of the entity the endorsement is raised against | [optional] 
**created_at** | **datetime** | Timestamp when the endorsement was created | [optional] 
**updated_at** | **datetime** | Timestamp when the endorsement was last updated | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.endorsement import Endorsement

# TODO update the JSON string below
json = "{}"
# create an instance of Endorsement from a JSON string
endorsement_instance = Endorsement.from_json(json)
# print the JSON string representation of the object
print(Endorsement.to_json())

# convert the object into a dict
endorsement_dict = endorsement_instance.to_dict()
# create an instance of Endorsement from a dict
endorsement_from_dict = Endorsement.from_dict(endorsement_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


