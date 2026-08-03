# Subsidiary

Model representing subsidiaries

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** | Unique identifier for the subsidiary | [optional] 
**name** | **str** | Name of the subsidiary | [optional] 
**address_1** | **str** | Primary address line of the subsidiary | [optional] 
**address_2** | **str** | Secondary address line of the subsidiary | [optional] 
**town** | **str** | Town where the subsidiary is located | [optional] 
**county** | **str** | County where the subsidiary is located | [optional] 
**country** | **str** | Country where the subsidiary is located | [optional] 
**postcode** | **str** | Postcode of the subsidiary | [optional] 
**website** | **str** | Website of the subsidiary | [optional] 
**is_parent** | **int** | Indicates if the subsidiary is a parent company | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.subsidiary import Subsidiary

# TODO update the JSON string below
json = "{}"
# create an instance of Subsidiary from a JSON string
subsidiary_instance = Subsidiary.from_json(json)
# print the JSON string representation of the object
print(Subsidiary.to_json())

# convert the object into a dict
subsidiary_dict = subsidiary_instance.to_dict()
# create an instance of Subsidiary from a dict
subsidiary_from_dict = Subsidiary.from_dict(subsidiary_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


