# safepeopleregistry_api_sdk.ONSSubmissionApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**o_ns_submission_receive_csv**](ONSSubmissionApi.md#o_ns_submission_receive_csv) | **POST** /api/v1/ons-submissions/csv | Upload a CSV file for ONS submission


# **o_ns_submission_receive_csv**
> ONSSubmissionReceiveCSV200Response o_ns_submission_receive_csv(file=file)

Upload a CSV file for ONS submission

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.ons_submission_receive_csv200_response import ONSSubmissionReceiveCSV200Response
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
    api_instance = safepeopleregistry_api_sdk.ONSSubmissionApi(api_client)
    file = None # bytes | CSV file to upload (optional)

    try:
        # Upload a CSV file for ONS submission
        api_response = api_instance.o_ns_submission_receive_csv(file=file)
        print("The response of ONSSubmissionApi->o_ns_submission_receive_csv:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ONSSubmissionApi->o_ns_submission_receive_csv: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **file** | **bytes**| CSV file to upload | [optional] 

### Return type

[**ONSSubmissionReceiveCSV200Response**](ONSSubmissionReceiveCSV200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: multipart/form-data
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | File uploaded successfully |  -  |
**400** | File upload failed |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

