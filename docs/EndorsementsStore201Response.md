# EndorsementsStore201Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | [optional] 
**data** | **int** | ID of the created Endorsement entry | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.endorsements_store201_response import EndorsementsStore201Response

# TODO update the JSON string below
json = "{}"
# create an instance of EndorsementsStore201Response from a JSON string
endorsements_store201_response_instance = EndorsementsStore201Response.from_json(json)
# print the JSON string representation of the object
print(EndorsementsStore201Response.to_json())

# convert the object into a dict
endorsements_store201_response_dict = endorsements_store201_response_instance.to_dict()
# create an instance of EndorsementsStore201Response from a dict
endorsements_store201_response_from_dict = EndorsementsStore201Response.from_dict(endorsements_store201_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


