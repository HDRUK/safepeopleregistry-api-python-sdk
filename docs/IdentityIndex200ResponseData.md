# IdentityIndex200ResponseData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | [optional] 
**created_at** | **str** |  | [optional] 
**updated_at** | **str** |  | [optional] 
**registry_id** | **int** |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.identity_index200_response_data import IdentityIndex200ResponseData

# TODO update the JSON string below
json = "{}"
# create an instance of IdentityIndex200ResponseData from a JSON string
identity_index200_response_data_instance = IdentityIndex200ResponseData.from_json(json)
# print the JSON string representation of the object
print(IdentityIndex200ResponseData.to_json())

# convert the object into a dict
identity_index200_response_data_dict = identity_index200_response_data_instance.to_dict()
# create an instance of IdentityIndex200ResponseData from a dict
identity_index200_response_data_from_dict = IdentityIndex200ResponseData.from_dict(identity_index200_response_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


