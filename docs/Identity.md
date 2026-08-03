# Identity

Model representing identity records

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** | Unique identifier for the identity record | [optional] 
**registry_id** | **int** | ID of the registry associated with the identity record | [optional] 
**address_1** | **str** | First line of the address | [optional] 
**address_2** | **str** | Second line of the address | [optional] 
**town** | **str** | Town of the address | [optional] 
**county** | **str** | County of the address | [optional] 
**country** | **str** | Country of the address | [optional] 
**postcode** | **str** | Postcode of the address | [optional] 
**dob** | **date** | Date of birth | [optional] 
**idvt_success** | **int** | Indicates whether IDVT was successful (1 for success, 0 for failure) | [optional] 
**idvt_identification_number** | **str** | Identification number from IDVT | [optional] 
**idvt_document_type** | **str** | Type of document used for IDVT | [optional] 
**idvt_document_number** | **str** | Document number used for IDVT | [optional] 
**idvt_document_country** | **str** | Country of the document used for IDVT | [optional] 
**idvt_document_valid_until** | **date** | Validity date of the document used for IDVT | [optional] 
**idvt_attempt_id** | **str** | ID of the IDVT attempt | [optional] 
**idvt_context_id** | **str** | Context ID for IDVT | [optional] 
**idvt_document_dob** | **date** | Date of birth on the document used for IDVT | [optional] 
**idvt_context** | **str** | Context of the IDVT process | [optional] 
**idvt_completed_at** | **datetime** | Timestamp when IDVT was completed | [optional] 
**idvt_result_text** | **str** | Result text of the IDVT process | [optional] 
**idvt_started_at** | **datetime** | Timestamp when IDVT was started | [optional] 
**created_at** | **datetime** | Timestamp when the identity record was created | [optional] 
**updated_at** | **datetime** | Timestamp when the identity record was last updated | [optional] 
**deleted_at** | **datetime** | Timestamp when the identity record was deleted | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.identity import Identity

# TODO update the JSON string below
json = "{}"
# create an instance of Identity from a JSON string
identity_instance = Identity.from_json(json)
# print the JSON string representation of the object
print(Identity.to_json())

# convert the object into a dict
identity_dict = identity_instance.to_dict()
# create an instance of Identity from a dict
identity_from_dict = Identity.from_dict(identity_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


