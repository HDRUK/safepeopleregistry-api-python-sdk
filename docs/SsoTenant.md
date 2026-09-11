# SsoTenant

An enterprise customer's SAML Identity Provider connection

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** | Model primary key | [optional] 
**created_at** | **str** |  | [optional] 
**updated_at** | **str** |  | [optional] 
**name** | **str** |  | [optional] 
**idp_alias** | **str** |  | [optional] 
**metadata_url** | **str** |  | [optional] 
**entity_id** | **str** |  | [optional] 
**metadata_imported_at** | **str** |  | [optional] 
**enabled** | **bool** |  | [optional] 
**sp_entity_id** | **str** | Keycloak&#39;s own SP entity ID - null until approved. Register this as the SAML Identifier on the customer&#39;s IdP. | [optional] 
**sp_acs_url** | **str** | Keycloak&#39;s ACS/reply URL for this tenant - null until approved. | [optional] 
**sp_metadata_url** | **str** | Downloadable SP metadata descriptor most IdPs can import directly - null until approved. | [optional] 
**status** | **str** | One of pending, approved, rejected | [optional] 
**submitted_by_user_id** | **int** | ID of the user who submitted this tenant for approval | [optional] 
**rejected_reason** | **str** | Reason given when status is rejected - null otherwise | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.sso_tenant import SsoTenant

# TODO update the JSON string below
json = "{}"
# create an instance of SsoTenant from a JSON string
sso_tenant_instance = SsoTenant.from_json(json)
# print the JSON string representation of the object
print(SsoTenant.to_json())

# convert the object into a dict
sso_tenant_dict = sso_tenant_instance.to_dict()
# create an instance of SsoTenant from a dict
sso_tenant_from_dict = SsoTenant.from_dict(sso_tenant_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


