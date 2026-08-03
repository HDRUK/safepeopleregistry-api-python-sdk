# Organisation

Organisation model

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** | Model primary key | [optional] 
**created_at** | **str** |  | [optional] 
**updated_at** | **str** |  | [optional] 
**organisation_name** | **str** |  | [optional] 
**address_1** | **str** |  | [optional] 
**address_2** | **str** |  | [optional] 
**town** | **str** |  | [optional] 
**county** | **str** |  | [optional] 
**country** | **str** |  | [optional] 
**postcode** | **str** |  | [optional] 
**lead_applicant_organisation_name** | **str** |  | [optional] 
**lead_applicant_email** | **str** |  | [optional] 
**organisation_unique_id** | **str** |  | [optional] 
**applicant_names** | **str** |  | [optional] 
**funders_and_sponsors** | **str** |  | [optional] 
**sub_license_arrangements** | **str** |  | [optional] 
**verified** | **bool** |  | [optional] 
**dsptk_ods_code** | **str** |  | [optional] 
**dsptk_certified** | **bool** |  | [optional] 
**dsptk_expiry_date** | **str** |  | [optional] 
**iso_27001_certified** | **bool** |  | [optional] 
**iso_27001_certification_num** | **str** |  | [optional] 
**iso_expiry_date** | **str** |  | [optional] 
**ce_certified** | **bool** |  | [optional] 
**ce_certification_num** | **str** |  | [optional] 
**ce_expiry_date** | **str** |  | [optional] 
**ce_plus_certified** | **bool** |  | [optional] 
**ce_plus_certification_num** | **str** |  | [optional] 
**ce_plus_expiry_date** | **str** |  | [optional] 
**idvt_result** | **int** |  | [optional] 
**idvt_result_perc** | **int** |  | [optional] 
**idvt_errors** | **str** |  | [optional] 
**idvt_completed_at** | **str** |  | [optional] 
**companies_house_no** | **str** |  | [optional] 
**sector_id** | **int** |  | [optional] 
**ror_id** | **str** | ROR.org identification for Research Organisations | [optional] 
**website** | **str** |  | [optional] 
**smb_status** | **bool** | Declaration of small/medium business | [optional] 
**organisation_size** | **int** | Organisation size. Integer denotes list index rather than absolute value | [optional] 
**unclaimed** | **bool** | Unclaimed | [optional] 
**system_approved** | **bool** | Whether this Organisation has been approved to use the system or not | [optional] 
**ods_id** | **str** |  | [optional] 
**dsptk_status** | **str** |  | [optional] 
**dsptk_date_last_published** | **str** |  | [optional] 
**ico_registration_id** | **str** |  | [optional] 
**ico_date_registered** | **str** |  | [optional] 
**ico_expiry_date** | **str** |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.organisation import Organisation

# TODO update the JSON string below
json = "{}"
# create an instance of Organisation from a JSON string
organisation_instance = Organisation.from_json(json)
# print the JSON string representation of the object
print(Organisation.to_json())

# convert the object into a dict
organisation_dict = organisation_instance.to_dict()
# create an instance of Organisation from a dict
organisation_from_dict = Organisation.from_dict(organisation_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


