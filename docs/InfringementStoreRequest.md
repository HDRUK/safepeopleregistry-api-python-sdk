# InfringementStoreRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**reported_by** | **int** |  | [optional] 
**comment** | **str** |  | [optional] 
**raised_against** | **int** |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.infringement_store_request import InfringementStoreRequest

# TODO update the JSON string below
json = "{}"
# create an instance of InfringementStoreRequest from a JSON string
infringement_store_request_instance = InfringementStoreRequest.from_json(json)
# print the JSON string representation of the object
print(InfringementStoreRequest.to_json())

# convert the object into a dict
infringement_store_request_dict = infringement_store_request_instance.to_dict()
# create an instance of InfringementStoreRequest from a dict
infringement_store_request_from_dict = InfringementStoreRequest.from_dict(infringement_store_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


