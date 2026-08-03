# IdentityStoreRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**registry_id** | **int** |  | [optional] 
**selfie_path** | **str** |  | [optional] 
**passport_path** | **str** |  | [optional] 
**drivers_license_path** | **str** |  | [optional] 
**address_1** | **str** |  | [optional] 
**address_2** | **str** |  | [optional] 
**town** | **str** |  | [optional] 
**county** | **str** |  | [optional] 
**country** | **str** |  | [optional] 
**postcode** | **str** |  | [optional] 
**dob** | **str** |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.identity_store_request import IdentityStoreRequest

# TODO update the JSON string below
json = "{}"
# create an instance of IdentityStoreRequest from a JSON string
identity_store_request_instance = IdentityStoreRequest.from_json(json)
# print the JSON string representation of the object
print(IdentityStoreRequest.to_json())

# convert the object into a dict
identity_store_request_dict = identity_store_request_instance.to_dict()
# create an instance of IdentityStoreRequest from a dict
identity_store_request_from_dict = IdentityStoreRequest.from_dict(identity_store_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


