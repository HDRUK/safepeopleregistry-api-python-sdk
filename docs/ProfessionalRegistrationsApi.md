# safepeopleregistry_api_sdk.ProfessionalRegistrationsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**professional_registrations_update**](ProfessionalRegistrationsApi.md#professional_registrations_update) | **PUT** /api/v1/professional_registrations/{id} | Professional Registrations@update


# **professional_registrations_update**
> ProfessionalRegistrationsUpdate200Response professional_registrations_update(id, professional_registrations_update_request)

Professional Registrations@update

Update a Professional Registrations entry

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.professional_registrations_update200_response import ProfessionalRegistrationsUpdate200Response
from safepeopleregistry_api_sdk.models.professional_registrations_update_request import ProfessionalRegistrationsUpdateRequest
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
    api_instance = safepeopleregistry_api_sdk.ProfessionalRegistrationsApi(api_client)
    id = 1 # int | Professional Registrations entry ID
    professional_registrations_update_request = safepeopleregistry_api_sdk.ProfessionalRegistrationsUpdateRequest() # ProfessionalRegistrationsUpdateRequest | Professional Registrations definition

    try:
        # Professional Registrations@update
        api_response = api_instance.professional_registrations_update(id, professional_registrations_update_request)
        print("The response of ProfessionalRegistrationsApi->professional_registrations_update:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ProfessionalRegistrationsApi->professional_registrations_update: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| Professional Registrations entry ID | 
 **professional_registrations_update_request** | [**ProfessionalRegistrationsUpdateRequest**](ProfessionalRegistrationsUpdateRequest.md)| Professional Registrations definition | 

### Return type

[**ProfessionalRegistrationsUpdate200Response**](ProfessionalRegistrationsUpdate200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success |  -  |
**400** | Invalid argument(s) |  -  |
**404** | Not found response |  -  |
**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

