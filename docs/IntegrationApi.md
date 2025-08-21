# autoppia_backend_client.IntegrationApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**integration_admin_integration_attribute_create**](IntegrationApi.md#integration_admin_integration_attribute_create) | **POST** /integration/admin/integration_attribute/ | 
[**integration_admin_integration_attribute_delete**](IntegrationApi.md#integration_admin_integration_attribute_delete) | **DELETE** /integration/admin/integration_attribute/{id}/ | 
[**integration_admin_integration_attribute_list**](IntegrationApi.md#integration_admin_integration_attribute_list) | **GET** /integration/admin/integration_attribute/ | 
[**integration_admin_integration_attribute_partial_update**](IntegrationApi.md#integration_admin_integration_attribute_partial_update) | **PATCH** /integration/admin/integration_attribute/{id}/ | 
[**integration_admin_integration_attribute_read**](IntegrationApi.md#integration_admin_integration_attribute_read) | **GET** /integration/admin/integration_attribute/{id}/ | 
[**integration_admin_integration_attribute_update**](IntegrationApi.md#integration_admin_integration_attribute_update) | **PUT** /integration/admin/integration_attribute/{id}/ | 
[**integration_admin_integration_create**](IntegrationApi.md#integration_admin_integration_create) | **POST** /integration/admin/integration/ | 
[**integration_admin_integration_delete**](IntegrationApi.md#integration_admin_integration_delete) | **DELETE** /integration/admin/integration/{id}/ | 
[**integration_admin_integration_list**](IntegrationApi.md#integration_admin_integration_list) | **GET** /integration/admin/integration/ | 
[**integration_admin_integration_partial_update**](IntegrationApi.md#integration_admin_integration_partial_update) | **PATCH** /integration/admin/integration/{id}/ | 
[**integration_admin_integration_read**](IntegrationApi.md#integration_admin_integration_read) | **GET** /integration/admin/integration/{id}/ | 
[**integration_admin_integration_update**](IntegrationApi.md#integration_admin_integration_update) | **PUT** /integration/admin/integration/{id}/ | 
[**integration_api_categories_list**](IntegrationApi.md#integration_api_categories_list) | **GET** /integration/api/categories/ | 
[**integration_integration_list**](IntegrationApi.md#integration_integration_list) | **GET** /integration/integration/ | 
[**integration_integration_read**](IntegrationApi.md#integration_integration_read) | **GET** /integration/integration/{id}/ | 
[**integration_user_integration_create**](IntegrationApi.md#integration_user_integration_create) | **POST** /integration/user_integration/ | 
[**integration_user_integration_delete**](IntegrationApi.md#integration_user_integration_delete) | **DELETE** /integration/user_integration/{id}/ | 
[**integration_user_integration_list**](IntegrationApi.md#integration_user_integration_list) | **GET** /integration/user_integration/ | 
[**integration_user_integration_partial_update**](IntegrationApi.md#integration_user_integration_partial_update) | **PATCH** /integration/user_integration/{id}/ | 
[**integration_user_integration_read**](IntegrationApi.md#integration_user_integration_read) | **GET** /integration/user_integration/{id}/ | 
[**integration_user_integration_update**](IntegrationApi.md#integration_user_integration_update) | **PUT** /integration/user_integration/{id}/ | 
[**integration_webappintegration_list**](IntegrationApi.md#integration_webappintegration_list) | **GET** /integration/webappintegration/ | 


# **integration_admin_integration_attribute_create**
> IntegrationAttribute integration_admin_integration_attribute_create(data)



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
    api_instance = autoppia_backend_client.IntegrationApi(api_client)
    data = autoppia_backend_client.IntegrationAttribute() # IntegrationAttribute | 

    try:
        api_response = api_instance.integration_admin_integration_attribute_create(data)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling IntegrationApi->integration_admin_integration_attribute_create: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **data** | [**IntegrationAttribute**](IntegrationAttribute.md)|  | 

### Return type

[**IntegrationAttribute**](IntegrationAttribute.md)

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

# **integration_admin_integration_attribute_delete**
> integration_admin_integration_attribute_delete(id)



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
    api_instance = autoppia_backend_client.IntegrationApi(api_client)
    id = 56 # int | A unique integer value identifying this integration attribute.

    try:
        api_instance.integration_admin_integration_attribute_delete(id)
    except ApiException as e:
        print("Exception when calling IntegrationApi->integration_admin_integration_attribute_delete: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| A unique integer value identifying this integration attribute. | 

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

# **integration_admin_integration_attribute_list**
> list[IntegrationAttribute] integration_admin_integration_attribute_list()



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
    api_instance = autoppia_backend_client.IntegrationApi(api_client)
    
    try:
        api_response = api_instance.integration_admin_integration_attribute_list()
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling IntegrationApi->integration_admin_integration_attribute_list: %s\n" % e)
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**list[IntegrationAttribute]**](IntegrationAttribute.md)

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

# **integration_admin_integration_attribute_partial_update**
> IntegrationAttribute integration_admin_integration_attribute_partial_update(id, data)



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
    api_instance = autoppia_backend_client.IntegrationApi(api_client)
    id = 56 # int | A unique integer value identifying this integration attribute.
data = autoppia_backend_client.IntegrationAttribute() # IntegrationAttribute | 

    try:
        api_response = api_instance.integration_admin_integration_attribute_partial_update(id, data)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling IntegrationApi->integration_admin_integration_attribute_partial_update: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| A unique integer value identifying this integration attribute. | 
 **data** | [**IntegrationAttribute**](IntegrationAttribute.md)|  | 

### Return type

[**IntegrationAttribute**](IntegrationAttribute.md)

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

# **integration_admin_integration_attribute_read**
> IntegrationAttribute integration_admin_integration_attribute_read(id)



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
    api_instance = autoppia_backend_client.IntegrationApi(api_client)
    id = 56 # int | A unique integer value identifying this integration attribute.

    try:
        api_response = api_instance.integration_admin_integration_attribute_read(id)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling IntegrationApi->integration_admin_integration_attribute_read: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| A unique integer value identifying this integration attribute. | 

### Return type

[**IntegrationAttribute**](IntegrationAttribute.md)

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

# **integration_admin_integration_attribute_update**
> IntegrationAttribute integration_admin_integration_attribute_update(id, data)



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
    api_instance = autoppia_backend_client.IntegrationApi(api_client)
    id = 56 # int | A unique integer value identifying this integration attribute.
data = autoppia_backend_client.IntegrationAttribute() # IntegrationAttribute | 

    try:
        api_response = api_instance.integration_admin_integration_attribute_update(id, data)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling IntegrationApi->integration_admin_integration_attribute_update: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| A unique integer value identifying this integration attribute. | 
 **data** | [**IntegrationAttribute**](IntegrationAttribute.md)|  | 

### Return type

[**IntegrationAttribute**](IntegrationAttribute.md)

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

# **integration_admin_integration_create**
> Integration integration_admin_integration_create(data)



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
    api_instance = autoppia_backend_client.IntegrationApi(api_client)
    data = autoppia_backend_client.Integration() # Integration | 

    try:
        api_response = api_instance.integration_admin_integration_create(data)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling IntegrationApi->integration_admin_integration_create: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **data** | [**Integration**](Integration.md)|  | 

### Return type

[**Integration**](Integration.md)

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

# **integration_admin_integration_delete**
> integration_admin_integration_delete(id)



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
    api_instance = autoppia_backend_client.IntegrationApi(api_client)
    id = 56 # int | A unique integer value identifying this integration.

    try:
        api_instance.integration_admin_integration_delete(id)
    except ApiException as e:
        print("Exception when calling IntegrationApi->integration_admin_integration_delete: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| A unique integer value identifying this integration. | 

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

# **integration_admin_integration_list**
> list[Integration] integration_admin_integration_list()



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
    api_instance = autoppia_backend_client.IntegrationApi(api_client)
    
    try:
        api_response = api_instance.integration_admin_integration_list()
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling IntegrationApi->integration_admin_integration_list: %s\n" % e)
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**list[Integration]**](Integration.md)

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

# **integration_admin_integration_partial_update**
> Integration integration_admin_integration_partial_update(id, data)



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
    api_instance = autoppia_backend_client.IntegrationApi(api_client)
    id = 56 # int | A unique integer value identifying this integration.
data = autoppia_backend_client.Integration() # Integration | 

    try:
        api_response = api_instance.integration_admin_integration_partial_update(id, data)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling IntegrationApi->integration_admin_integration_partial_update: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| A unique integer value identifying this integration. | 
 **data** | [**Integration**](Integration.md)|  | 

### Return type

[**Integration**](Integration.md)

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

# **integration_admin_integration_read**
> Integration integration_admin_integration_read(id)



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
    api_instance = autoppia_backend_client.IntegrationApi(api_client)
    id = 56 # int | A unique integer value identifying this integration.

    try:
        api_response = api_instance.integration_admin_integration_read(id)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling IntegrationApi->integration_admin_integration_read: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| A unique integer value identifying this integration. | 

### Return type

[**Integration**](Integration.md)

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

# **integration_admin_integration_update**
> Integration integration_admin_integration_update(id, data)



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
    api_instance = autoppia_backend_client.IntegrationApi(api_client)
    id = 56 # int | A unique integer value identifying this integration.
data = autoppia_backend_client.Integration() # Integration | 

    try:
        api_response = api_instance.integration_admin_integration_update(id, data)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling IntegrationApi->integration_admin_integration_update: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| A unique integer value identifying this integration. | 
 **data** | [**Integration**](Integration.md)|  | 

### Return type

[**Integration**](Integration.md)

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

# **integration_api_categories_list**
> integration_api_categories_list()



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
    api_instance = autoppia_backend_client.IntegrationApi(api_client)
    
    try:
        api_instance.integration_api_categories_list()
    except ApiException as e:
        print("Exception when calling IntegrationApi->integration_api_categories_list: %s\n" % e)
```

### Parameters
This endpoint does not need any parameter.

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
**200** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **integration_integration_list**
> list[ListIntegration] integration_integration_list()



List all integrations

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
    api_instance = autoppia_backend_client.IntegrationApi(api_client)
    
    try:
        api_response = api_instance.integration_integration_list()
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling IntegrationApi->integration_integration_list: %s\n" % e)
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**list[ListIntegration]**](ListIntegration.md)

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

# **integration_integration_read**
> ListIntegration integration_integration_read(id)



Retrieve an integration by ID

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
    api_instance = autoppia_backend_client.IntegrationApi(api_client)
    id = 56 # int | A unique integer value identifying this integration.

    try:
        api_response = api_instance.integration_integration_read(id)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling IntegrationApi->integration_integration_read: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| A unique integer value identifying this integration. | 

### Return type

[**ListIntegration**](ListIntegration.md)

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

# **integration_user_integration_create**
> UserIntegration integration_user_integration_create(data)



Create a new user-specific integration

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
    api_instance = autoppia_backend_client.IntegrationApi(api_client)
    data = autoppia_backend_client.UserIntegration() # UserIntegration | 

    try:
        api_response = api_instance.integration_user_integration_create(data)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling IntegrationApi->integration_user_integration_create: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **data** | [**UserIntegration**](UserIntegration.md)|  | 

### Return type

[**UserIntegration**](UserIntegration.md)

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

# **integration_user_integration_delete**
> integration_user_integration_delete(id)



Delete a user-specific integration by ID

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
    api_instance = autoppia_backend_client.IntegrationApi(api_client)
    id = 56 # int | A unique integer value identifying this user integration.

    try:
        api_instance.integration_user_integration_delete(id)
    except ApiException as e:
        print("Exception when calling IntegrationApi->integration_user_integration_delete: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| A unique integer value identifying this user integration. | 

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

# **integration_user_integration_list**
> list[ListUserIntegration] integration_user_integration_list()



List user-specific integrations

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
    api_instance = autoppia_backend_client.IntegrationApi(api_client)
    
    try:
        api_response = api_instance.integration_user_integration_list()
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling IntegrationApi->integration_user_integration_list: %s\n" % e)
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**list[ListUserIntegration]**](ListUserIntegration.md)

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

# **integration_user_integration_partial_update**
> UserIntegration integration_user_integration_partial_update(id, data)



Partially update a user-specific integration by ID

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
    api_instance = autoppia_backend_client.IntegrationApi(api_client)
    id = 56 # int | A unique integer value identifying this user integration.
data = autoppia_backend_client.UserIntegration() # UserIntegration | 

    try:
        api_response = api_instance.integration_user_integration_partial_update(id, data)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling IntegrationApi->integration_user_integration_partial_update: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| A unique integer value identifying this user integration. | 
 **data** | [**UserIntegration**](UserIntegration.md)|  | 

### Return type

[**UserIntegration**](UserIntegration.md)

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

# **integration_user_integration_read**
> ListUserIntegration integration_user_integration_read(id)



Retrieve a user-specific integration by ID

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
    api_instance = autoppia_backend_client.IntegrationApi(api_client)
    id = 56 # int | A unique integer value identifying this user integration.

    try:
        api_response = api_instance.integration_user_integration_read(id)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling IntegrationApi->integration_user_integration_read: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| A unique integer value identifying this user integration. | 

### Return type

[**ListUserIntegration**](ListUserIntegration.md)

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

# **integration_user_integration_update**
> UserIntegration integration_user_integration_update(id, data)



Update a user-specific integration by ID

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
    api_instance = autoppia_backend_client.IntegrationApi(api_client)
    id = 56 # int | A unique integer value identifying this user integration.
data = autoppia_backend_client.UserIntegration() # UserIntegration | 

    try:
        api_response = api_instance.integration_user_integration_update(id, data)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling IntegrationApi->integration_user_integration_update: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| A unique integer value identifying this user integration. | 
 **data** | [**UserIntegration**](UserIntegration.md)|  | 

### Return type

[**UserIntegration**](UserIntegration.md)

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

# **integration_webappintegration_list**
> list[ListUserIntegration] integration_webappintegration_list()



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
    api_instance = autoppia_backend_client.IntegrationApi(api_client)
    
    try:
        api_response = api_instance.integration_webappintegration_list()
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling IntegrationApi->integration_webappintegration_list: %s\n" % e)
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**list[ListUserIntegration]**](ListUserIntegration.md)

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

