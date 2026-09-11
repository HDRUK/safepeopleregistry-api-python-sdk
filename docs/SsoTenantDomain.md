# SsoTenantDomain

An email domain routed to a Registry SSO tenant's Identity Provider

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** | Model primary key | [optional] 
**sso_tenant_id** | **int** |  | [optional] 
**domain** | **str** |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.sso_tenant_domain import SsoTenantDomain

# TODO update the JSON string below
json = "{}"
# create an instance of SsoTenantDomain from a JSON string
sso_tenant_domain_instance = SsoTenantDomain.from_json(json)
# print the JSON string representation of the object
print(SsoTenantDomain.to_json())

# convert the object into a dict
sso_tenant_domain_dict = sso_tenant_domain_instance.to_dict()
# create an instance of SsoTenantDomain from a dict
sso_tenant_domain_from_dict = SsoTenantDomain.from_dict(sso_tenant_domain_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


