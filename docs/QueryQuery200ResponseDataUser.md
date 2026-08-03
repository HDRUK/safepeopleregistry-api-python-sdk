# QueryQuery200ResponseDataUser

The User record linked to the matched Registry

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | [optional] 
**first_name** | **str** |  | [optional] 
**last_name** | **str** |  | [optional] 
**name** | **str** |  | [optional] 
**email** | **str** |  | [optional] 
**registry_id** | **int** |  | [optional] 
**created_at** | **str** |  | [optional] 
**updated_at** | **str** |  | [optional] 
**user_group** | **str** |  | [optional] 
**consent_scrape** | **bool** |  | [optional] 
**orc_id** | **str** |  | [optional] 
**unclaimed** | **int** |  | [optional] 
**feed_source** | **str** |  | [optional] 
**public_opt_in** | **int** |  | [optional] 
**declaration_signed** | **bool** |  | [optional] 
**organisation_id** | **int** |  | [optional] 
**orcid_scanning** | **bool** |  | [optional] 
**orcid_scanning_completed_at** | **str** |  | [optional] 
**is_delegate** | **int** |  | [optional] 
**is_org_admin** | **int** |  | [optional] 
**custodian_id** | **int** |  | [optional] 
**custodian_user_id** | **int** |  | [optional] 
**role** | **str** |  | [optional] 
**location** | **str** |  | [optional] 
**t_and_c_agreed** | **bool** |  | [optional] 
**t_and_c_agreement_date** | **str** |  | [optional] 
**uksa_registered** | **bool** |  | [optional] 
**is_sro** | **bool** |  | [optional] 
**invited_by** | **int** |  | [optional] 
**status** | **str** |  | [optional] 
**evaluation** | **str** |  | [optional] 
**identity** | [**Identity**](Identity.md) |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.query_query200_response_data_user import QueryQuery200ResponseDataUser

# TODO update the JSON string below
json = "{}"
# create an instance of QueryQuery200ResponseDataUser from a JSON string
query_query200_response_data_user_instance = QueryQuery200ResponseDataUser.from_json(json)
# print the JSON string representation of the object
print(QueryQuery200ResponseDataUser.to_json())

# convert the object into a dict
query_query200_response_data_user_dict = query_query200_response_data_user_instance.to_dict()
# create an instance of QueryQuery200ResponseDataUser from a dict
query_query200_response_data_user_from_dict = QueryQuery200ResponseDataUser.from_dict(query_query200_response_data_user_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


