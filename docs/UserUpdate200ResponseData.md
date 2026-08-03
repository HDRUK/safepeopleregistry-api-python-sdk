# UserUpdate200ResponseData


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
**orc_id** | **str** |  | [optional] 
**orcid_scanning** | **int** |  | [optional] 
**orcid_scanning_completed_at** | **str** |  | [optional] 
**t_and_c_agreed** | **bool** |  | [optional] 
**t_and_c_agreement_date** | **str** |  | [optional] 
**status** | **str** |  | [optional] 
**uksa_registered** | **bool** |  | [optional] 
**is_sro** | **bool** |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.user_update200_response_data import UserUpdate200ResponseData

# TODO update the JSON string below
json = "{}"
# create an instance of UserUpdate200ResponseData from a JSON string
user_update200_response_data_instance = UserUpdate200ResponseData.from_json(json)
# print the JSON string representation of the object
print(UserUpdate200ResponseData.to_json())

# convert the object into a dict
user_update200_response_data_dict = user_update200_response_data_instance.to_dict()
# create an instance of UserUpdate200ResponseData from a dict
user_update200_response_data_from_dict = UserUpdate200ResponseData.from_dict(user_update200_response_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


