# Sector

Model representing sectors

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** | Unique identifier for the sector | [optional] 
**name** | **str** | Name of the sector | [optional] 
**created_at** | **datetime** | Timestamp when the sector was created | [optional] 
**updated_at** | **datetime** | Timestamp when the sector was last updated | [optional] 
**deleted_at** | **datetime** | Timestamp when the sector was deleted | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.sector import Sector

# TODO update the JSON string below
json = "{}"
# create an instance of Sector from a JSON string
sector_instance = Sector.from_json(json)
# print the JSON string representation of the object
print(Sector.to_json())

# convert the object into a dict
sector_dict = sector_instance.to_dict()
# create an instance of Sector from a dict
sector_from_dict = Sector.from_dict(sector_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


