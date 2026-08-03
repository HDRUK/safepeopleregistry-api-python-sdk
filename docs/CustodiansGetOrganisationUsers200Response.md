# CustodiansGetOrganisationUsers200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | [optional] 
**data** | [**List[User]**](User.md) |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.custodians_get_organisation_users200_response import CustodiansGetOrganisationUsers200Response

# TODO update the JSON string below
json = "{}"
# create an instance of CustodiansGetOrganisationUsers200Response from a JSON string
custodians_get_organisation_users200_response_instance = CustodiansGetOrganisationUsers200Response.from_json(json)
# print the JSON string representation of the object
print(CustodiansGetOrganisationUsers200Response.to_json())

# convert the object into a dict
custodians_get_organisation_users200_response_dict = custodians_get_organisation_users200_response_instance.to_dict()
# create an instance of CustodiansGetOrganisationUsers200Response from a dict
custodians_get_organisation_users200_response_from_dict = CustodiansGetOrganisationUsers200Response.from_dict(custodians_get_organisation_users200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


