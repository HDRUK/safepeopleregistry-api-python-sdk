# Infringement

Model representing infringements

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** | Unique identifier for the infringement | [optional] 
**reported_by** | **int** | ID of the user who reported the infringement | [optional] 
**comment** | **str** | Optional comment provided by the reporter | [optional] 
**raised_against** | **int** | ID of the entity the infringement is raised against | [optional] 
**created_at** | **datetime** | Timestamp when the infringement was created | [optional] 
**updated_at** | **datetime** | Timestamp when the infringement was last updated | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.infringement import Infringement

# TODO update the JSON string below
json = "{}"
# create an instance of Infringement from a JSON string
infringement_instance = Infringement.from_json(json)
# print the JSON string representation of the object
print(Infringement.to_json())

# convert the object into a dict
infringement_dict = infringement_instance.to_dict()
# create an instance of Infringement from a dict
infringement_from_dict = Infringement.from_dict(infringement_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


