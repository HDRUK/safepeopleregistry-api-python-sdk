# safepeopleregistry_api_sdk.CustodiansApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**custodians_create_custodian_validation_checks**](CustodiansApi.md#custodians_create_custodian_validation_checks) | **POST** /api/v1/custodians/{custodianId}/validation_checks | Assign a validation check to a custodian
[**custodians_get_custodian_users**](CustodiansApi.md#custodians_get_custodian_users) | **GET** /api/v1/custodians/{custodianId}/custodian_users | Get list of people for a custodian
[**custodians_get_custodian_validation_checks**](CustodiansApi.md#custodians_get_custodian_validation_checks) | **GET** /api/v1/custodians/{custodianId}/validation_checks | Get validation checks assigned to a custodian
[**custodians_get_organisation_users**](CustodiansApi.md#custodians_get_organisation_users) | **GET** /api/v1/custodians/{custodianId}/organisations/{organisationId}/users | Get list of people for organisation
[**custodians_get_rules**](CustodiansApi.md#custodians_get_rules) | **GET** /api/v1/custodians/{id}/rules | Get rules for a specific custodian
[**custodians_get_statuses_users**](CustodiansApi.md#custodians_get_statuses_users) | **GET** /api/v1/custodians/{custodianId}/projectUsers/{projectUserId}/statuses | Get statuses for a user in a project/organisation/custodian


# **custodians_create_custodian_validation_checks**
> ValidationCheck custodians_create_custodian_validation_checks(custodian_id, custodians_create_custodian_validation_checks_request)

Assign a validation check to a custodian

Creates a new validation check and assigns it to a specific custodian via the custodian_has_validation_check pivot table.

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.custodians_create_custodian_validation_checks_request import CustodiansCreateCustodianValidationChecksRequest
from safepeopleregistry_api_sdk.models.validation_check import ValidationCheck
from safepeopleregistry_api_sdk.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = safepeopleregistry_api_sdk.Configuration(
    host = "http://localhost"
)


# Enter a context with an instance of the API client
with safepeopleregistry_api_sdk.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = safepeopleregistry_api_sdk.CustodiansApi(api_client)
    custodian_id = 56 # int | ID of the custodian
    custodians_create_custodian_validation_checks_request = safepeopleregistry_api_sdk.CustodiansCreateCustodianValidationChecksRequest() # CustodiansCreateCustodianValidationChecksRequest | 

    try:
        # Assign a validation check to a custodian
        api_response = api_instance.custodians_create_custodian_validation_checks(custodian_id, custodians_create_custodian_validation_checks_request)
        print("The response of CustodiansApi->custodians_create_custodian_validation_checks:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CustodiansApi->custodians_create_custodian_validation_checks: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **custodian_id** | **int**| ID of the custodian | 
 **custodians_create_custodian_validation_checks_request** | [**CustodiansCreateCustodianValidationChecksRequest**](CustodiansCreateCustodianValidationChecksRequest.md)|  | 

### Return type

[**ValidationCheck**](ValidationCheck.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**201** | Validation check created and assigned successfully |  -  |
**400** | Invalid input |  -  |
**404** | Custodian not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **custodians_get_custodian_users**
> CustodiansGetCustodianUsers200Response custodians_get_custodian_users(custodian_id)

Get list of people for a custodian

Fetches the list of custodian users based on the custodian id.

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.custodians_get_custodian_users200_response import CustodiansGetCustodianUsers200Response
from safepeopleregistry_api_sdk.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = safepeopleregistry_api_sdk.Configuration(
    host = "http://localhost"
)


# Enter a context with an instance of the API client
with safepeopleregistry_api_sdk.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = safepeopleregistry_api_sdk.CustodiansApi(api_client)
    custodian_id = 56 # int | ID of the custodian

    try:
        # Get list of people for a custodian
        api_response = api_instance.custodians_get_custodian_users(custodian_id)
        print("The response of CustodiansApi->custodians_get_custodian_users:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CustodiansApi->custodians_get_custodian_users: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **custodian_id** | **int**| ID of the custodian | 

### Return type

[**CustodiansGetCustodianUsers200Response**](CustodiansGetCustodianUsers200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successfully retrieved custodian users |  -  |
**400** | Invalid argument(s) |  -  |
**404** | Custodian users not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **custodians_get_custodian_validation_checks**
> List[ValidationCheck] custodians_get_custodian_validation_checks(custodian_id)

Get validation checks assigned to a custodian

Returns the list of validation checks associated with a specific custodian.

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.validation_check import ValidationCheck
from safepeopleregistry_api_sdk.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = safepeopleregistry_api_sdk.Configuration(
    host = "http://localhost"
)


# Enter a context with an instance of the API client
with safepeopleregistry_api_sdk.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = safepeopleregistry_api_sdk.CustodiansApi(api_client)
    custodian_id = 56 # int | ID of the custodian

    try:
        # Get validation checks assigned to a custodian
        api_response = api_instance.custodians_get_custodian_validation_checks(custodian_id)
        print("The response of CustodiansApi->custodians_get_custodian_validation_checks:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CustodiansApi->custodians_get_custodian_validation_checks: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **custodian_id** | **int**| ID of the custodian | 

### Return type

[**List[ValidationCheck]**](ValidationCheck.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Validation checks retrieved successfully |  -  |
**400** | Invalid argument(s) |  -  |
**404** | Custodian not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **custodians_get_organisation_users**
> CustodiansGetOrganisationUsers200Response custodians_get_organisation_users(custodian_id, organisation_id)

Get list of people for organisation

Fetches the list of users associated with the given custodian and organisations IDs.

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.custodians_get_organisation_users200_response import CustodiansGetOrganisationUsers200Response
from safepeopleregistry_api_sdk.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = safepeopleregistry_api_sdk.Configuration(
    host = "http://localhost"
)


# Enter a context with an instance of the API client
with safepeopleregistry_api_sdk.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = safepeopleregistry_api_sdk.CustodiansApi(api_client)
    custodian_id = 56 # int | ID of the custodian
    organisation_id = 56 # int | ID of the organisation

    try:
        # Get list of people for organisation
        api_response = api_instance.custodians_get_organisation_users(custodian_id, organisation_id)
        print("The response of CustodiansApi->custodians_get_organisation_users:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CustodiansApi->custodians_get_organisation_users: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **custodian_id** | **int**| ID of the custodian | 
 **organisation_id** | **int**| ID of the organisation | 

### Return type

[**CustodiansGetOrganisationUsers200Response**](CustodiansGetOrganisationUsers200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successfully retrieved organisation users |  -  |
**400** | Invalid argument(s) |  -  |
**404** | Organisation users not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **custodians_get_rules**
> CustodiansGetRules200Response custodians_get_rules(id)

Get rules for a specific custodian

Fetches the list of rules associated with the given custodian ID.

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.custodians_get_rules200_response import CustodiansGetRules200Response
from safepeopleregistry_api_sdk.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = safepeopleregistry_api_sdk.Configuration(
    host = "http://localhost"
)


# Enter a context with an instance of the API client
with safepeopleregistry_api_sdk.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = safepeopleregistry_api_sdk.CustodiansApi(api_client)
    id = 56 # int | ID of the custodian

    try:
        # Get rules for a specific custodian
        api_response = api_instance.custodians_get_rules(id)
        print("The response of CustodiansApi->custodians_get_rules:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CustodiansApi->custodians_get_rules: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| ID of the custodian | 

### Return type

[**CustodiansGetRules200Response**](CustodiansGetRules200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successfully retrieved rules |  -  |
**400** | Invalid argument(s) |  -  |
**404** | Custodian not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **custodians_get_statuses_users**
> CustodiansGetOrganisationUsers200Response custodians_get_statuses_users(custodian_id, project_user_id)

Get statuses for a user in a project/organisation/custodian

Fetches the user statuses given custodian and organisations and project and user IDs.

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.custodians_get_organisation_users200_response import CustodiansGetOrganisationUsers200Response
from safepeopleregistry_api_sdk.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = safepeopleregistry_api_sdk.Configuration(
    host = "http://localhost"
)


# Enter a context with an instance of the API client
with safepeopleregistry_api_sdk.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = safepeopleregistry_api_sdk.CustodiansApi(api_client)
    custodian_id = 56 # int | ID of the custodian
    project_user_id = 56 # int | ID of the project user

    try:
        # Get statuses for a user in a project/organisation/custodian
        api_response = api_instance.custodians_get_statuses_users(custodian_id, project_user_id)
        print("The response of CustodiansApi->custodians_get_statuses_users:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CustodiansApi->custodians_get_statuses_users: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **custodian_id** | **int**| ID of the custodian | 
 **project_user_id** | **int**| ID of the project user | 

### Return type

[**CustodiansGetOrganisationUsers200Response**](CustodiansGetOrganisationUsers200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successfully retrieved organisation users |  -  |
**400** | Invalid argument(s) |  -  |
**404** | Organisation users not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

