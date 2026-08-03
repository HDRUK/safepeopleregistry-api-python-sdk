# UsersStore201ResponseData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | [optional] 
**created_at** | **str** |  | [optional] 
**updated_at** | **str** |  | [optional] 
**first_name** | **str** |  | [optional] 
**last_name** | **str** |  | [optional] 
**email** | **str** |  | [optional] 
**email_verified_at** | **str** |  | [optional] 
**consent_scrape** | **bool** |  | [optional] 
**public_opt_in** | **bool** |  | [optional] 
**declaration_signed** | **bool** |  | [optional] 
**organisation_id** | **int** |  | [optional] 
**orcid_scanning** | **int** |  | [optional] 
**orcid_scanning_completed_at** | **str** |  | [optional] 
**status** | **str** |  | [optional] 
**uksa_registered** | **bool** |  | [optional] 
**is_sro** | **bool** |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.users_store201_response_data import UsersStore201ResponseData

# TODO update the JSON string below
json = "{}"
# create an instance of UsersStore201ResponseData from a JSON string
users_store201_response_data_instance = UsersStore201ResponseData.from_json(json)
# print the JSON string representation of the object
print(UsersStore201ResponseData.to_json())

# convert the object into a dict
users_store201_response_data_dict = users_store201_response_data_instance.to_dict()
# create an instance of UsersStore201ResponseData from a dict
users_store201_response_data_from_dict = UsersStore201ResponseData.from_dict(users_store201_response_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


