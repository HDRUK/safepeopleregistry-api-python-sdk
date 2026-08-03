# EndorsementsStoreRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**reported_by** | **int** |  | [optional] 
**comment** | **str** |  | [optional] 
**raised_against** | **int** |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.endorsements_store_request import EndorsementsStoreRequest

# TODO update the JSON string below
json = "{}"
# create an instance of EndorsementsStoreRequest from a JSON string
endorsements_store_request_instance = EndorsementsStoreRequest.from_json(json)
# print the JSON string representation of the object
print(EndorsementsStoreRequest.to_json())

# convert the object into a dict
endorsements_store_request_dict = endorsements_store_request_instance.to_dict()
# create an instance of EndorsementsStoreRequest from a dict
endorsements_store_request_from_dict = EndorsementsStoreRequest.from_dict(endorsements_store_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


