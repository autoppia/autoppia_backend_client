# autoppia_backend_client.CoworkersApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**coworkers_configuration_coworkers_create**](CoworkersApi.md#coworkers_configuration_coworkers_create) | **POST** /coworkers/configuration/coworkers/ | 
[**coworkers_configuration_coworkers_delete**](CoworkersApi.md#coworkers_configuration_coworkers_delete) | **DELETE** /coworkers/configuration/coworkers/{id}/ | 
[**coworkers_configuration_coworkers_list**](CoworkersApi.md#coworkers_configuration_coworkers_list) | **GET** /coworkers/configuration/coworkers/ | 
[**coworkers_configuration_coworkers_partial_update**](CoworkersApi.md#coworkers_configuration_coworkers_partial_update) | **PATCH** /coworkers/configuration/coworkers/{id}/ | 
[**coworkers_configuration_coworkers_read**](CoworkersApi.md#coworkers_configuration_coworkers_read) | **GET** /coworkers/configuration/coworkers/{id}/ | 
[**coworkers_configuration_coworkers_update**](CoworkersApi.md#coworkers_configuration_coworkers_update) | **PUT** /coworkers/configuration/coworkers/{id}/ | 


# **coworkers_configuration_coworkers_create**
> Coworker coworkers_configuration_coworkers_create(data)



### Example

* Basic Authentication (Basic):
```python
from __future__ import print_function
import time
import autoppia_backend_client
from autoppia_backend_client.rest import ApiException
from pprint import pprint
# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = autoppia_backend_client.Configuration(
    host = "http://localhost"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: Basic
configuration = autoppia_backend_client.Configuration(
    username = 'YOUR_USERNAME',
    password = 'YOUR_PASSWORD'
)

# Enter a context with an instance of the API client
with autoppia_backend_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = autoppia_backend_client.CoworkersApi(api_client)
    data = autoppia_backend_client.Coworker() # Coworker | 

    try:
        api_response = api_instance.coworkers_configuration_coworkers_create(data)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling CoworkersApi->coworkers_configuration_coworkers_create: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **data** | [**Coworker**](Coworker.md)|  | 

### Return type

[**Coworker**](Coworker.md)

### Authorization

[Basic](../README.md#Basic)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**201** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **coworkers_configuration_coworkers_delete**
> coworkers_configuration_coworkers_delete(id)



### Example

* Basic Authentication (Basic):
```python
from __future__ import print_function
import time
import autoppia_backend_client
from autoppia_backend_client.rest import ApiException
from pprint import pprint
# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = autoppia_backend_client.Configuration(
    host = "http://localhost"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: Basic
configuration = autoppia_backend_client.Configuration(
    username = 'YOUR_USERNAME',
    password = 'YOUR_PASSWORD'
)

# Enter a context with an instance of the API client
with autoppia_backend_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = autoppia_backend_client.CoworkersApi(api_client)
    id = 56 # int | A unique integer value identifying this coworker.

    try:
        api_instance.coworkers_configuration_coworkers_delete(id)
    except ApiException as e:
        print("Exception when calling CoworkersApi->coworkers_configuration_coworkers_delete: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| A unique integer value identifying this coworker. | 

### Return type

void (empty response body)

### Authorization

[Basic](../README.md#Basic)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**204** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **coworkers_configuration_coworkers_list**
> list[Coworker] coworkers_configuration_coworkers_list()



### Example

* Basic Authentication (Basic):
```python
from __future__ import print_function
import time
import autoppia_backend_client
from autoppia_backend_client.rest import ApiException
from pprint import pprint
# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = autoppia_backend_client.Configuration(
    host = "http://localhost"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: Basic
configuration = autoppia_backend_client.Configuration(
    username = 'YOUR_USERNAME',
    password = 'YOUR_PASSWORD'
)

# Enter a context with an instance of the API client
with autoppia_backend_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = autoppia_backend_client.CoworkersApi(api_client)
    
    try:
        api_response = api_instance.coworkers_configuration_coworkers_list()
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling CoworkersApi->coworkers_configuration_coworkers_list: %s\n" % e)
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**list[Coworker]**](Coworker.md)

### Authorization

[Basic](../README.md#Basic)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **coworkers_configuration_coworkers_partial_update**
> Coworker coworkers_configuration_coworkers_partial_update(id, data)



### Example

* Basic Authentication (Basic):
```python
from __future__ import print_function
import time
import autoppia_backend_client
from autoppia_backend_client.rest import ApiException
from pprint import pprint
# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = autoppia_backend_client.Configuration(
    host = "http://localhost"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: Basic
configuration = autoppia_backend_client.Configuration(
    username = 'YOUR_USERNAME',
    password = 'YOUR_PASSWORD'
)

# Enter a context with an instance of the API client
with autoppia_backend_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = autoppia_backend_client.CoworkersApi(api_client)
    id = 56 # int | A unique integer value identifying this coworker.
data = autoppia_backend_client.Coworker() # Coworker | 

    try:
        api_response = api_instance.coworkers_configuration_coworkers_partial_update(id, data)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling CoworkersApi->coworkers_configuration_coworkers_partial_update: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| A unique integer value identifying this coworker. | 
 **data** | [**Coworker**](Coworker.md)|  | 

### Return type

[**Coworker**](Coworker.md)

### Authorization

[Basic](../README.md#Basic)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **coworkers_configuration_coworkers_read**
> Coworker coworkers_configuration_coworkers_read(id)



### Example

* Basic Authentication (Basic):
```python
from __future__ import print_function
import time
import autoppia_backend_client
from autoppia_backend_client.rest import ApiException
from pprint import pprint
# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = autoppia_backend_client.Configuration(
    host = "http://localhost"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: Basic
configuration = autoppia_backend_client.Configuration(
    username = 'YOUR_USERNAME',
    password = 'YOUR_PASSWORD'
)

# Enter a context with an instance of the API client
with autoppia_backend_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = autoppia_backend_client.CoworkersApi(api_client)
    id = 56 # int | A unique integer value identifying this coworker.

    try:
        api_response = api_instance.coworkers_configuration_coworkers_read(id)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling CoworkersApi->coworkers_configuration_coworkers_read: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| A unique integer value identifying this coworker. | 

### Return type

[**Coworker**](Coworker.md)

### Authorization

[Basic](../README.md#Basic)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **coworkers_configuration_coworkers_update**
> Coworker coworkers_configuration_coworkers_update(id, data)



### Example

* Basic Authentication (Basic):
```python
from __future__ import print_function
import time
import autoppia_backend_client
from autoppia_backend_client.rest import ApiException
from pprint import pprint
# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = autoppia_backend_client.Configuration(
    host = "http://localhost"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: Basic
configuration = autoppia_backend_client.Configuration(
    username = 'YOUR_USERNAME',
    password = 'YOUR_PASSWORD'
)

# Enter a context with an instance of the API client
with autoppia_backend_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = autoppia_backend_client.CoworkersApi(api_client)
    id = 56 # int | A unique integer value identifying this coworker.
data = autoppia_backend_client.Coworker() # Coworker | 

    try:
        api_response = api_instance.coworkers_configuration_coworkers_update(id, data)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling CoworkersApi->coworkers_configuration_coworkers_update: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| A unique integer value identifying this coworker. | 
 **data** | [**Coworker**](Coworker.md)|  | 

### Return type

[**Coworker**](Coworker.md)

### Authorization

[Basic](../README.md#Basic)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

