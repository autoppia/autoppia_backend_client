# autoppia_backend_client.LlmsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**llms_llm_create**](LlmsApi.md#llms_llm_create) | **POST** /llms/llm/ | 
[**llms_llm_delete**](LlmsApi.md#llms_llm_delete) | **DELETE** /llms/llm/{id}/ | 
[**llms_llm_list**](LlmsApi.md#llms_llm_list) | **GET** /llms/llm/ | 
[**llms_llm_partial_update**](LlmsApi.md#llms_llm_partial_update) | **PATCH** /llms/llm/{id}/ | 
[**llms_llm_provider_create**](LlmsApi.md#llms_llm_provider_create) | **POST** /llms/llm-provider/ | 
[**llms_llm_provider_delete**](LlmsApi.md#llms_llm_provider_delete) | **DELETE** /llms/llm-provider/{id}/ | 
[**llms_llm_provider_list**](LlmsApi.md#llms_llm_provider_list) | **GET** /llms/llm-provider/ | 
[**llms_llm_provider_partial_update**](LlmsApi.md#llms_llm_provider_partial_update) | **PATCH** /llms/llm-provider/{id}/ | 
[**llms_llm_provider_read**](LlmsApi.md#llms_llm_provider_read) | **GET** /llms/llm-provider/{id}/ | 
[**llms_llm_provider_update**](LlmsApi.md#llms_llm_provider_update) | **PUT** /llms/llm-provider/{id}/ | 
[**llms_llm_read**](LlmsApi.md#llms_llm_read) | **GET** /llms/llm/{id}/ | 
[**llms_llm_update**](LlmsApi.md#llms_llm_update) | **PUT** /llms/llm/{id}/ | 
[**llms_user_llm_create**](LlmsApi.md#llms_user_llm_create) | **POST** /llms/user-llm/ | 
[**llms_user_llm_delete**](LlmsApi.md#llms_user_llm_delete) | **DELETE** /llms/user-llm/{id}/ | 
[**llms_user_llm_list**](LlmsApi.md#llms_user_llm_list) | **GET** /llms/user-llm/ | 
[**llms_user_llm_partial_update**](LlmsApi.md#llms_user_llm_partial_update) | **PATCH** /llms/user-llm/{id}/ | 
[**llms_user_llm_read**](LlmsApi.md#llms_user_llm_read) | **GET** /llms/user-llm/{id}/ | 
[**llms_user_llm_update**](LlmsApi.md#llms_user_llm_update) | **PUT** /llms/user-llm/{id}/ | 


# **llms_llm_create**
> LLMModel llms_llm_create(data)



Create a new LLM model

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
    api_instance = autoppia_backend_client.LlmsApi(api_client)
    data = autoppia_backend_client.LLMModel() # LLMModel | 

    try:
        api_response = api_instance.llms_llm_create(data)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling LlmsApi->llms_llm_create: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **data** | [**LLMModel**](LLMModel.md)|  | 

### Return type

[**LLMModel**](LLMModel.md)

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

# **llms_llm_delete**
> llms_llm_delete(id)



Delete an LLM model by ID

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
    api_instance = autoppia_backend_client.LlmsApi(api_client)
    id = 56 # int | A unique integer value identifying this llm model.

    try:
        api_instance.llms_llm_delete(id)
    except ApiException as e:
        print("Exception when calling LlmsApi->llms_llm_delete: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| A unique integer value identifying this llm model. | 

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

# **llms_llm_list**
> list[LLMModel] llms_llm_list()



List all LLM models

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
    api_instance = autoppia_backend_client.LlmsApi(api_client)
    
    try:
        api_response = api_instance.llms_llm_list()
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling LlmsApi->llms_llm_list: %s\n" % e)
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**list[LLMModel]**](LLMModel.md)

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

# **llms_llm_partial_update**
> LLMModel llms_llm_partial_update(id, data)



Partially update an LLM model by ID

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
    api_instance = autoppia_backend_client.LlmsApi(api_client)
    id = 56 # int | A unique integer value identifying this llm model.
data = autoppia_backend_client.LLMModel() # LLMModel | 

    try:
        api_response = api_instance.llms_llm_partial_update(id, data)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling LlmsApi->llms_llm_partial_update: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| A unique integer value identifying this llm model. | 
 **data** | [**LLMModel**](LLMModel.md)|  | 

### Return type

[**LLMModel**](LLMModel.md)

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

# **llms_llm_provider_create**
> LLMProvider llms_llm_provider_create(data)



Create a new LLM provider

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
    api_instance = autoppia_backend_client.LlmsApi(api_client)
    data = autoppia_backend_client.LLMProvider() # LLMProvider | 

    try:
        api_response = api_instance.llms_llm_provider_create(data)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling LlmsApi->llms_llm_provider_create: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **data** | [**LLMProvider**](LLMProvider.md)|  | 

### Return type

[**LLMProvider**](LLMProvider.md)

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

# **llms_llm_provider_delete**
> llms_llm_provider_delete(id)



Delete an LLM provider by ID

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
    api_instance = autoppia_backend_client.LlmsApi(api_client)
    id = 56 # int | A unique integer value identifying this llm provider.

    try:
        api_instance.llms_llm_provider_delete(id)
    except ApiException as e:
        print("Exception when calling LlmsApi->llms_llm_provider_delete: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| A unique integer value identifying this llm provider. | 

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

# **llms_llm_provider_list**
> list[LLMProvider] llms_llm_provider_list()



List all LLM providers

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
    api_instance = autoppia_backend_client.LlmsApi(api_client)
    
    try:
        api_response = api_instance.llms_llm_provider_list()
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling LlmsApi->llms_llm_provider_list: %s\n" % e)
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**list[LLMProvider]**](LLMProvider.md)

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

# **llms_llm_provider_partial_update**
> LLMProvider llms_llm_provider_partial_update(id, data)



Partially update an LLM provider by ID

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
    api_instance = autoppia_backend_client.LlmsApi(api_client)
    id = 56 # int | A unique integer value identifying this llm provider.
data = autoppia_backend_client.LLMProvider() # LLMProvider | 

    try:
        api_response = api_instance.llms_llm_provider_partial_update(id, data)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling LlmsApi->llms_llm_provider_partial_update: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| A unique integer value identifying this llm provider. | 
 **data** | [**LLMProvider**](LLMProvider.md)|  | 

### Return type

[**LLMProvider**](LLMProvider.md)

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

# **llms_llm_provider_read**
> LLMProvider llms_llm_provider_read(id)



Retrieve an LLM provider by ID

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
    api_instance = autoppia_backend_client.LlmsApi(api_client)
    id = 56 # int | A unique integer value identifying this llm provider.

    try:
        api_response = api_instance.llms_llm_provider_read(id)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling LlmsApi->llms_llm_provider_read: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| A unique integer value identifying this llm provider. | 

### Return type

[**LLMProvider**](LLMProvider.md)

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

# **llms_llm_provider_update**
> LLMProvider llms_llm_provider_update(id, data)



Update an LLM provider by ID

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
    api_instance = autoppia_backend_client.LlmsApi(api_client)
    id = 56 # int | A unique integer value identifying this llm provider.
data = autoppia_backend_client.LLMProvider() # LLMProvider | 

    try:
        api_response = api_instance.llms_llm_provider_update(id, data)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling LlmsApi->llms_llm_provider_update: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| A unique integer value identifying this llm provider. | 
 **data** | [**LLMProvider**](LLMProvider.md)|  | 

### Return type

[**LLMProvider**](LLMProvider.md)

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

# **llms_llm_read**
> LLMModel llms_llm_read(id)



Retrieve an LLM model by ID

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
    api_instance = autoppia_backend_client.LlmsApi(api_client)
    id = 56 # int | A unique integer value identifying this llm model.

    try:
        api_response = api_instance.llms_llm_read(id)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling LlmsApi->llms_llm_read: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| A unique integer value identifying this llm model. | 

### Return type

[**LLMModel**](LLMModel.md)

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

# **llms_llm_update**
> LLMModel llms_llm_update(id, data)



Update an LLM model by ID

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
    api_instance = autoppia_backend_client.LlmsApi(api_client)
    id = 56 # int | A unique integer value identifying this llm model.
data = autoppia_backend_client.LLMModel() # LLMModel | 

    try:
        api_response = api_instance.llms_llm_update(id, data)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling LlmsApi->llms_llm_update: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| A unique integer value identifying this llm model. | 
 **data** | [**LLMModel**](LLMModel.md)|  | 

### Return type

[**LLMModel**](LLMModel.md)

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

# **llms_user_llm_create**
> UserLLMModel llms_user_llm_create(data)



Create a new user-specific LLM model

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
    api_instance = autoppia_backend_client.LlmsApi(api_client)
    data = autoppia_backend_client.UserLLMModel() # UserLLMModel | 

    try:
        api_response = api_instance.llms_user_llm_create(data)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling LlmsApi->llms_user_llm_create: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **data** | [**UserLLMModel**](UserLLMModel.md)|  | 

### Return type

[**UserLLMModel**](UserLLMModel.md)

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

# **llms_user_llm_delete**
> llms_user_llm_delete(id)



Delete a user-specific LLM model by ID

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
    api_instance = autoppia_backend_client.LlmsApi(api_client)
    id = 56 # int | A unique integer value identifying this user llm model.

    try:
        api_instance.llms_user_llm_delete(id)
    except ApiException as e:
        print("Exception when calling LlmsApi->llms_user_llm_delete: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| A unique integer value identifying this user llm model. | 

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

# **llms_user_llm_list**
> list[UserLLMModel] llms_user_llm_list()



List user-specific LLM models

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
    api_instance = autoppia_backend_client.LlmsApi(api_client)
    
    try:
        api_response = api_instance.llms_user_llm_list()
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling LlmsApi->llms_user_llm_list: %s\n" % e)
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**list[UserLLMModel]**](UserLLMModel.md)

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

# **llms_user_llm_partial_update**
> UserLLMModel llms_user_llm_partial_update(id, data)



Partially update a user-specific LLM model by ID

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
    api_instance = autoppia_backend_client.LlmsApi(api_client)
    id = 56 # int | A unique integer value identifying this user llm model.
data = autoppia_backend_client.UserLLMModel() # UserLLMModel | 

    try:
        api_response = api_instance.llms_user_llm_partial_update(id, data)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling LlmsApi->llms_user_llm_partial_update: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| A unique integer value identifying this user llm model. | 
 **data** | [**UserLLMModel**](UserLLMModel.md)|  | 

### Return type

[**UserLLMModel**](UserLLMModel.md)

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

# **llms_user_llm_read**
> UserLLMModel llms_user_llm_read(id)



Retrieve a user-specific LLM model by ID

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
    api_instance = autoppia_backend_client.LlmsApi(api_client)
    id = 56 # int | A unique integer value identifying this user llm model.

    try:
        api_response = api_instance.llms_user_llm_read(id)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling LlmsApi->llms_user_llm_read: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| A unique integer value identifying this user llm model. | 

### Return type

[**UserLLMModel**](UserLLMModel.md)

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

# **llms_user_llm_update**
> UserLLMModel llms_user_llm_update(id, data)



Update a user-specific LLM model by ID

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
    api_instance = autoppia_backend_client.LlmsApi(api_client)
    id = 56 # int | A unique integer value identifying this user llm model.
data = autoppia_backend_client.UserLLMModel() # UserLLMModel | 

    try:
        api_response = api_instance.llms_user_llm_update(id, data)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling LlmsApi->llms_user_llm_update: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| A unique integer value identifying this user llm model. | 
 **data** | [**UserLLMModel**](UserLLMModel.md)|  | 

### Return type

[**UserLLMModel**](UserLLMModel.md)

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

