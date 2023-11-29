# openapi_client.EmployeeApi

All URIs are relative to *https://localhost:7044*

Method | HTTP request | Description
------------- | ------------- | -------------
[**employee_get**](EmployeeApi.md#employee_get) | **GET** /employee | 
[**employee_id_delete**](EmployeeApi.md#employee_id_delete) | **DELETE** /employee/{id} | 
[**employee_id_get**](EmployeeApi.md#employee_id_get) | **GET** /employee/{id} | 
[**employee_id_put**](EmployeeApi.md#employee_id_put) | **PUT** /employee/{id} | 
[**employee_post**](EmployeeApi.md#employee_post) | **POST** /employee | 


# **employee_get**
> List[Employee] employee_get()



### Example

```python
import time
import os
import openapi_client
from openapi_client.models.employee import Employee
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://localhost:7044
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "https://localhost:7044"
)


# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.EmployeeApi(api_client)

    try:
        api_response = api_instance.employee_get()
        print("The response of EmployeeApi->employee_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EmployeeApi->employee_get: %s\n" % e)
```



### Parameters
This endpoint does not need any parameter.

### Return type

[**List[Employee]**](Employee.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: text/plain, application/json, text/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **employee_id_delete**
> employee_id_delete(id)



### Example

```python
import time
import os
import openapi_client
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://localhost:7044
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "https://localhost:7044"
)


# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.EmployeeApi(api_client)
    id = 56 # int | 

    try:
        api_instance.employee_id_delete(id)
    except Exception as e:
        print("Exception when calling EmployeeApi->employee_id_delete: %s\n" % e)
```



### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**|  | 

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **employee_id_get**
> Employee employee_id_get(id)



### Example

```python
import time
import os
import openapi_client
from openapi_client.models.employee import Employee
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://localhost:7044
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "https://localhost:7044"
)


# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.EmployeeApi(api_client)
    id = 56 # int | 

    try:
        api_response = api_instance.employee_id_get(id)
        print("The response of EmployeeApi->employee_id_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EmployeeApi->employee_id_get: %s\n" % e)
```



### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**|  | 

### Return type

[**Employee**](Employee.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: text/plain, application/json, text/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **employee_id_put**
> employee_id_put(id, employee=employee)



### Example

```python
import time
import os
import openapi_client
from openapi_client.models.employee import Employee
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://localhost:7044
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "https://localhost:7044"
)


# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.EmployeeApi(api_client)
    id = 56 # int | 
    employee = openapi_client.Employee() # Employee |  (optional)

    try:
        api_instance.employee_id_put(id, employee=employee)
    except Exception as e:
        print("Exception when calling EmployeeApi->employee_id_put: %s\n" % e)
```



### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**|  | 
 **employee** | [**Employee**](Employee.md)|  | [optional] 

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json, text/json, application/*+json
 - **Accept**: Not defined

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **employee_post**
> Employee employee_post(employee=employee)



### Example

```python
import time
import os
import openapi_client
from openapi_client.models.employee import Employee
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://localhost:7044
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "https://localhost:7044"
)


# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.EmployeeApi(api_client)
    employee = openapi_client.Employee() # Employee |  (optional)

    try:
        api_response = api_instance.employee_post(employee=employee)
        print("The response of EmployeeApi->employee_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EmployeeApi->employee_post: %s\n" % e)
```



### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **employee** | [**Employee**](Employee.md)|  | [optional] 

### Return type

[**Employee**](Employee.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json, text/json, application/*+json
 - **Accept**: text/plain, application/json, text/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

