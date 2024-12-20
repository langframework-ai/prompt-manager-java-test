# DefaultApi

All URIs are relative to *https://goe0ty1i23.execute-api.us-east-1.amazonaws.com/default*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**apiV1PromptsCategoriesCallerIdOptions**](DefaultApi.md#apiV1PromptsCategoriesCallerIdOptions) | **OPTIONS** /api/v1/prompts/categories/{caller_id} |  |
| [**apiV1PromptsPromptPromptIdCallerCallerIdOptions**](DefaultApi.md#apiV1PromptsPromptPromptIdCallerCallerIdOptions) | **OPTIONS** /api/v1/prompts/prompt/{prompt_id}/caller/{caller_id} |  |
| [**apiV1PromptsPromptsCallerIdOptions**](DefaultApi.md#apiV1PromptsPromptsCallerIdOptions) | **OPTIONS** /api/v1/prompts/prompts/{caller_id} |  |
| [**createCategory**](DefaultApi.md#createCategory) | **POST** /api/v1/prompts/categories/{caller_id} |  |
| [**createPrompt**](DefaultApi.md#createPrompt) | **POST** /api/v1/prompts/prompts/{caller_id} |  |
| [**createUser**](DefaultApi.md#createUser) | **POST** /api/v1/prompts/users/{caller_id} |  |
| [**deleteCategory**](DefaultApi.md#deleteCategory) | **DELETE** /api/v1/prompts/category/{category_id}/caller/{caller_id} |  |
| [**deletePrompt**](DefaultApi.md#deletePrompt) | **DELETE** /api/v1/prompts/prompt/{prompt_id}/caller/{caller_id} |  |
| [**deleteUser**](DefaultApi.md#deleteUser) | **DELETE** /api/v1/prompts/user/{user_id}/caller/{caller_id} |  |
| [**getCategories**](DefaultApi.md#getCategories) | **GET** /api/v1/prompts/categories/{caller_id} |  |
| [**getCategoryByName**](DefaultApi.md#getCategoryByName) | **GET** /api/v1/prompts/category/name/{category_name}/caller/{caller_id} |  |
| [**getPromptComments**](DefaultApi.md#getPromptComments) | **GET** /api/v1/prompts/prompt/{prompt_id}/caller/{caller_id}/comments |  |
| [**getPromptDetails**](DefaultApi.md#getPromptDetails) | **GET** /api/v1/prompts/prompt/{prompt_id}/caller/{caller_id} |  |
| [**getPromptLikes**](DefaultApi.md#getPromptLikes) | **GET** /api/v1/prompts/prompt/{prompt_id}/caller/{caller_id}/likes |  |
| [**getPrompts**](DefaultApi.md#getPrompts) | **GET** /api/v1/prompts/prompts/{caller_id} |  |
| [**getPromptsByCategory**](DefaultApi.md#getPromptsByCategory) | **GET** /api/v1/prompts/prompts/category/{category_id}/caller/{caller_id} |  |
| [**getPromptsByUser**](DefaultApi.md#getPromptsByUser) | **GET** /api/v1/prompts/prompts/user/{user_id}/caller/{caller_id} |  |
| [**getUserDetails**](DefaultApi.md#getUserDetails) | **GET** /api/v1/prompts/user/{user_id}/caller/{caller_id} |  |
| [**getUsers**](DefaultApi.md#getUsers) | **GET** /api/v1/prompts/users/{caller_id} |  |
| [**likePrompt**](DefaultApi.md#likePrompt) | **POST** /api/v1/prompts/prompt/{prompt_id}/caller/{caller_id}/likes |  |
| [**postCommentOnPrompt**](DefaultApi.md#postCommentOnPrompt) | **POST** /api/v1/prompts/prompt/{prompt_id}/caller/{caller_id}/comments |  |
| [**searchPrompts**](DefaultApi.md#searchPrompts) | **GET** /api/v1/prompts/prompts/search/{caller_id} |  |
| [**updateCategory**](DefaultApi.md#updateCategory) | **PUT** /api/v1/prompts/category/{category_id}/caller/{caller_id} |  |
| [**updatePrompt**](DefaultApi.md#updatePrompt) | **PUT** /api/v1/prompts/prompt/{prompt_id}/caller/{caller_id} |  |
| [**updateUser**](DefaultApi.md#updateUser) | **PUT** /api/v1/prompts/user/{user_id}/caller/{caller_id} |  |


<a id="apiV1PromptsCategoriesCallerIdOptions"></a>
# **apiV1PromptsCategoriesCallerIdOptions**
> Object apiV1PromptsCategoriesCallerIdOptions(callerId)



### Example
```java
// Import classes:
import ai.langframework.promptmanager.client.ApiClient;
import ai.langframework.promptmanager.client.ApiException;
import ai.langframework.promptmanager.client.Configuration;
import ai.langframework.promptmanager.client.models.*;
import ai.langframework.promptmanager.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://goe0ty1i23.execute-api.us-east-1.amazonaws.com/default");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    String callerId = "callerId_example"; // String | 
    try {
      Object result = apiInstance.apiV1PromptsCategoriesCallerIdOptions(callerId);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#apiV1PromptsCategoriesCallerIdOptions");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **callerId** | **String**|  | |

### Return type

**Object**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | 200 response |  * Access-Control-Allow-Origin -  <br>  * Access-Control-Allow-Methods -  <br>  * Access-Control-Allow-Headers -  <br>  |

<a id="apiV1PromptsPromptPromptIdCallerCallerIdOptions"></a>
# **apiV1PromptsPromptPromptIdCallerCallerIdOptions**
> Object apiV1PromptsPromptPromptIdCallerCallerIdOptions(promptId, callerId)



### Example
```java
// Import classes:
import ai.langframework.promptmanager.client.ApiClient;
import ai.langframework.promptmanager.client.ApiException;
import ai.langframework.promptmanager.client.Configuration;
import ai.langframework.promptmanager.client.models.*;
import ai.langframework.promptmanager.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://goe0ty1i23.execute-api.us-east-1.amazonaws.com/default");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    String promptId = "promptId_example"; // String | 
    String callerId = "callerId_example"; // String | 
    try {
      Object result = apiInstance.apiV1PromptsPromptPromptIdCallerCallerIdOptions(promptId, callerId);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#apiV1PromptsPromptPromptIdCallerCallerIdOptions");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **promptId** | **String**|  | |
| **callerId** | **String**|  | |

### Return type

**Object**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | 200 response |  * Access-Control-Allow-Origin -  <br>  * Access-Control-Allow-Methods -  <br>  * Access-Control-Allow-Headers -  <br>  |

<a id="apiV1PromptsPromptsCallerIdOptions"></a>
# **apiV1PromptsPromptsCallerIdOptions**
> Object apiV1PromptsPromptsCallerIdOptions(callerId)



### Example
```java
// Import classes:
import ai.langframework.promptmanager.client.ApiClient;
import ai.langframework.promptmanager.client.ApiException;
import ai.langframework.promptmanager.client.Configuration;
import ai.langframework.promptmanager.client.models.*;
import ai.langframework.promptmanager.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://goe0ty1i23.execute-api.us-east-1.amazonaws.com/default");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    String callerId = "callerId_example"; // String | 
    try {
      Object result = apiInstance.apiV1PromptsPromptsCallerIdOptions(callerId);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#apiV1PromptsPromptsCallerIdOptions");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **callerId** | **String**|  | |

### Return type

**Object**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | 200 response |  * Access-Control-Allow-Origin -  <br>  * Access-Control-Allow-Methods -  <br>  * Access-Control-Allow-Headers -  <br>  |

<a id="createCategory"></a>
# **createCategory**
> Object createCategory(callerId, categoryModel)



### Example
```java
// Import classes:
import ai.langframework.promptmanager.client.ApiClient;
import ai.langframework.promptmanager.client.ApiException;
import ai.langframework.promptmanager.client.Configuration;
import ai.langframework.promptmanager.client.models.*;
import ai.langframework.promptmanager.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://goe0ty1i23.execute-api.us-east-1.amazonaws.com/default");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    String callerId = "callerId_example"; // String | 
    CategoryModel categoryModel = new CategoryModel(); // CategoryModel | 
    try {
      Object result = apiInstance.createCategory(callerId, categoryModel);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#createCategory");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **callerId** | **String**|  | |
| **categoryModel** | [**CategoryModel**](CategoryModel.md)|  | |

### Return type

**Object**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | 200 response |  -  |

<a id="createPrompt"></a>
# **createPrompt**
> createPrompt(callerId, promptModel)



### Example
```java
// Import classes:
import ai.langframework.promptmanager.client.ApiClient;
import ai.langframework.promptmanager.client.ApiException;
import ai.langframework.promptmanager.client.Configuration;
import ai.langframework.promptmanager.client.models.*;
import ai.langframework.promptmanager.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://goe0ty1i23.execute-api.us-east-1.amazonaws.com/default");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    String callerId = "callerId_example"; // String | 
    PromptModel promptModel = new PromptModel(); // PromptModel | 
    try {
      apiInstance.createPrompt(callerId, promptModel);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#createPrompt");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **callerId** | **String**|  | |
| **promptModel** | [**PromptModel**](PromptModel.md)|  | |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | 200 response |  -  |

<a id="createUser"></a>
# **createUser**
> Object createUser(callerId, userModel)



### Example
```java
// Import classes:
import ai.langframework.promptmanager.client.ApiClient;
import ai.langframework.promptmanager.client.ApiException;
import ai.langframework.promptmanager.client.Configuration;
import ai.langframework.promptmanager.client.models.*;
import ai.langframework.promptmanager.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://goe0ty1i23.execute-api.us-east-1.amazonaws.com/default");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    String callerId = "callerId_example"; // String | 
    UserModel userModel = new UserModel(); // UserModel | 
    try {
      Object result = apiInstance.createUser(callerId, userModel);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#createUser");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **callerId** | **String**|  | |
| **userModel** | [**UserModel**](UserModel.md)|  | |

### Return type

**Object**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | 200 response |  -  |

<a id="deleteCategory"></a>
# **deleteCategory**
> Object deleteCategory(callerId, categoryId)



### Example
```java
// Import classes:
import ai.langframework.promptmanager.client.ApiClient;
import ai.langframework.promptmanager.client.ApiException;
import ai.langframework.promptmanager.client.Configuration;
import ai.langframework.promptmanager.client.models.*;
import ai.langframework.promptmanager.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://goe0ty1i23.execute-api.us-east-1.amazonaws.com/default");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    String callerId = "callerId_example"; // String | 
    String categoryId = "categoryId_example"; // String | 
    try {
      Object result = apiInstance.deleteCategory(callerId, categoryId);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#deleteCategory");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **callerId** | **String**|  | |
| **categoryId** | **String**|  | |

### Return type

**Object**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | 200 response |  -  |

<a id="deletePrompt"></a>
# **deletePrompt**
> Object deletePrompt(promptId, callerId)



### Example
```java
// Import classes:
import ai.langframework.promptmanager.client.ApiClient;
import ai.langframework.promptmanager.client.ApiException;
import ai.langframework.promptmanager.client.Configuration;
import ai.langframework.promptmanager.client.models.*;
import ai.langframework.promptmanager.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://goe0ty1i23.execute-api.us-east-1.amazonaws.com/default");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    String promptId = "promptId_example"; // String | 
    String callerId = "callerId_example"; // String | 
    try {
      Object result = apiInstance.deletePrompt(promptId, callerId);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#deletePrompt");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **promptId** | **String**|  | |
| **callerId** | **String**|  | |

### Return type

**Object**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | 200 response |  -  |

<a id="deleteUser"></a>
# **deleteUser**
> Object deleteUser(userId, callerId)



### Example
```java
// Import classes:
import ai.langframework.promptmanager.client.ApiClient;
import ai.langframework.promptmanager.client.ApiException;
import ai.langframework.promptmanager.client.Configuration;
import ai.langframework.promptmanager.client.models.*;
import ai.langframework.promptmanager.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://goe0ty1i23.execute-api.us-east-1.amazonaws.com/default");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    String userId = "userId_example"; // String | 
    String callerId = "callerId_example"; // String | 
    try {
      Object result = apiInstance.deleteUser(userId, callerId);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#deleteUser");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **userId** | **String**|  | |
| **callerId** | **String**|  | |

### Return type

**Object**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | 200 response |  -  |

<a id="getCategories"></a>
# **getCategories**
> Object getCategories(callerId)



### Example
```java
// Import classes:
import ai.langframework.promptmanager.client.ApiClient;
import ai.langframework.promptmanager.client.ApiException;
import ai.langframework.promptmanager.client.Configuration;
import ai.langframework.promptmanager.client.models.*;
import ai.langframework.promptmanager.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://goe0ty1i23.execute-api.us-east-1.amazonaws.com/default");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    String callerId = "callerId_example"; // String | 
    try {
      Object result = apiInstance.getCategories(callerId);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#getCategories");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **callerId** | **String**|  | |

### Return type

**Object**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | 200 response |  -  |

<a id="getCategoryByName"></a>
# **getCategoryByName**
> Object getCategoryByName(categoryName, callerId)



### Example
```java
// Import classes:
import ai.langframework.promptmanager.client.ApiClient;
import ai.langframework.promptmanager.client.ApiException;
import ai.langframework.promptmanager.client.Configuration;
import ai.langframework.promptmanager.client.models.*;
import ai.langframework.promptmanager.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://goe0ty1i23.execute-api.us-east-1.amazonaws.com/default");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    String categoryName = "categoryName_example"; // String | 
    String callerId = "callerId_example"; // String | 
    try {
      Object result = apiInstance.getCategoryByName(categoryName, callerId);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#getCategoryByName");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **categoryName** | **String**|  | |
| **callerId** | **String**|  | |

### Return type

**Object**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | 200 response |  -  |

<a id="getPromptComments"></a>
# **getPromptComments**
> Object getPromptComments(promptId, callerId)



### Example
```java
// Import classes:
import ai.langframework.promptmanager.client.ApiClient;
import ai.langframework.promptmanager.client.ApiException;
import ai.langframework.promptmanager.client.Configuration;
import ai.langframework.promptmanager.client.models.*;
import ai.langframework.promptmanager.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://goe0ty1i23.execute-api.us-east-1.amazonaws.com/default");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    String promptId = "promptId_example"; // String | 
    String callerId = "callerId_example"; // String | 
    try {
      Object result = apiInstance.getPromptComments(promptId, callerId);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#getPromptComments");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **promptId** | **String**|  | |
| **callerId** | **String**|  | |

### Return type

**Object**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | 200 response |  -  |

<a id="getPromptDetails"></a>
# **getPromptDetails**
> Object getPromptDetails(promptId, callerId)



### Example
```java
// Import classes:
import ai.langframework.promptmanager.client.ApiClient;
import ai.langframework.promptmanager.client.ApiException;
import ai.langframework.promptmanager.client.Configuration;
import ai.langframework.promptmanager.client.models.*;
import ai.langframework.promptmanager.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://goe0ty1i23.execute-api.us-east-1.amazonaws.com/default");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    String promptId = "promptId_example"; // String | 
    String callerId = "callerId_example"; // String | 
    try {
      Object result = apiInstance.getPromptDetails(promptId, callerId);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#getPromptDetails");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **promptId** | **String**|  | |
| **callerId** | **String**|  | |

### Return type

**Object**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | 200 response |  -  |

<a id="getPromptLikes"></a>
# **getPromptLikes**
> Object getPromptLikes(promptId, callerId)



### Example
```java
// Import classes:
import ai.langframework.promptmanager.client.ApiClient;
import ai.langframework.promptmanager.client.ApiException;
import ai.langframework.promptmanager.client.Configuration;
import ai.langframework.promptmanager.client.models.*;
import ai.langframework.promptmanager.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://goe0ty1i23.execute-api.us-east-1.amazonaws.com/default");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    String promptId = "promptId_example"; // String | 
    String callerId = "callerId_example"; // String | 
    try {
      Object result = apiInstance.getPromptLikes(promptId, callerId);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#getPromptLikes");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **promptId** | **String**|  | |
| **callerId** | **String**|  | |

### Return type

**Object**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | 200 response |  -  |

<a id="getPrompts"></a>
# **getPrompts**
> Object getPrompts(callerId)



### Example
```java
// Import classes:
import ai.langframework.promptmanager.client.ApiClient;
import ai.langframework.promptmanager.client.ApiException;
import ai.langframework.promptmanager.client.Configuration;
import ai.langframework.promptmanager.client.models.*;
import ai.langframework.promptmanager.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://goe0ty1i23.execute-api.us-east-1.amazonaws.com/default");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    String callerId = "callerId_example"; // String | 
    try {
      Object result = apiInstance.getPrompts(callerId);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#getPrompts");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **callerId** | **String**|  | |

### Return type

**Object**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | 200 response |  -  |

<a id="getPromptsByCategory"></a>
# **getPromptsByCategory**
> Object getPromptsByCategory(callerId, categoryId)



### Example
```java
// Import classes:
import ai.langframework.promptmanager.client.ApiClient;
import ai.langframework.promptmanager.client.ApiException;
import ai.langframework.promptmanager.client.Configuration;
import ai.langframework.promptmanager.client.models.*;
import ai.langframework.promptmanager.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://goe0ty1i23.execute-api.us-east-1.amazonaws.com/default");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    String callerId = "callerId_example"; // String | 
    String categoryId = "categoryId_example"; // String | 
    try {
      Object result = apiInstance.getPromptsByCategory(callerId, categoryId);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#getPromptsByCategory");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **callerId** | **String**|  | |
| **categoryId** | **String**|  | |

### Return type

**Object**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | 200 response |  -  |

<a id="getPromptsByUser"></a>
# **getPromptsByUser**
> Object getPromptsByUser(userId, callerId)



### Example
```java
// Import classes:
import ai.langframework.promptmanager.client.ApiClient;
import ai.langframework.promptmanager.client.ApiException;
import ai.langframework.promptmanager.client.Configuration;
import ai.langframework.promptmanager.client.models.*;
import ai.langframework.promptmanager.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://goe0ty1i23.execute-api.us-east-1.amazonaws.com/default");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    String userId = "userId_example"; // String | 
    String callerId = "callerId_example"; // String | 
    try {
      Object result = apiInstance.getPromptsByUser(userId, callerId);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#getPromptsByUser");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **userId** | **String**|  | |
| **callerId** | **String**|  | |

### Return type

**Object**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | 200 response |  -  |

<a id="getUserDetails"></a>
# **getUserDetails**
> Object getUserDetails(userId, callerId)



### Example
```java
// Import classes:
import ai.langframework.promptmanager.client.ApiClient;
import ai.langframework.promptmanager.client.ApiException;
import ai.langframework.promptmanager.client.Configuration;
import ai.langframework.promptmanager.client.models.*;
import ai.langframework.promptmanager.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://goe0ty1i23.execute-api.us-east-1.amazonaws.com/default");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    String userId = "userId_example"; // String | 
    String callerId = "callerId_example"; // String | 
    try {
      Object result = apiInstance.getUserDetails(userId, callerId);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#getUserDetails");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **userId** | **String**|  | |
| **callerId** | **String**|  | |

### Return type

**Object**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | 200 response |  -  |

<a id="getUsers"></a>
# **getUsers**
> Object getUsers(callerId)



### Example
```java
// Import classes:
import ai.langframework.promptmanager.client.ApiClient;
import ai.langframework.promptmanager.client.ApiException;
import ai.langframework.promptmanager.client.Configuration;
import ai.langframework.promptmanager.client.models.*;
import ai.langframework.promptmanager.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://goe0ty1i23.execute-api.us-east-1.amazonaws.com/default");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    String callerId = "callerId_example"; // String | 
    try {
      Object result = apiInstance.getUsers(callerId);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#getUsers");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **callerId** | **String**|  | |

### Return type

**Object**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | 200 response |  -  |

<a id="likePrompt"></a>
# **likePrompt**
> Object likePrompt(promptId, callerId, likeModel)



### Example
```java
// Import classes:
import ai.langframework.promptmanager.client.ApiClient;
import ai.langframework.promptmanager.client.ApiException;
import ai.langframework.promptmanager.client.Configuration;
import ai.langframework.promptmanager.client.models.*;
import ai.langframework.promptmanager.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://goe0ty1i23.execute-api.us-east-1.amazonaws.com/default");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    String promptId = "promptId_example"; // String | 
    String callerId = "callerId_example"; // String | 
    LikeModel likeModel = new LikeModel(); // LikeModel | 
    try {
      Object result = apiInstance.likePrompt(promptId, callerId, likeModel);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#likePrompt");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **promptId** | **String**|  | |
| **callerId** | **String**|  | |
| **likeModel** | [**LikeModel**](LikeModel.md)|  | |

### Return type

**Object**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | 200 response |  -  |

<a id="postCommentOnPrompt"></a>
# **postCommentOnPrompt**
> Object postCommentOnPrompt(promptId, callerId, commentModel)



### Example
```java
// Import classes:
import ai.langframework.promptmanager.client.ApiClient;
import ai.langframework.promptmanager.client.ApiException;
import ai.langframework.promptmanager.client.Configuration;
import ai.langframework.promptmanager.client.models.*;
import ai.langframework.promptmanager.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://goe0ty1i23.execute-api.us-east-1.amazonaws.com/default");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    String promptId = "promptId_example"; // String | 
    String callerId = "callerId_example"; // String | 
    CommentModel commentModel = new CommentModel(); // CommentModel | 
    try {
      Object result = apiInstance.postCommentOnPrompt(promptId, callerId, commentModel);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#postCommentOnPrompt");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **promptId** | **String**|  | |
| **callerId** | **String**|  | |
| **commentModel** | [**CommentModel**](CommentModel.md)|  | |

### Return type

**Object**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | 200 response |  -  |

<a id="searchPrompts"></a>
# **searchPrompts**
> Object searchPrompts(callerId, search)



### Example
```java
// Import classes:
import ai.langframework.promptmanager.client.ApiClient;
import ai.langframework.promptmanager.client.ApiException;
import ai.langframework.promptmanager.client.Configuration;
import ai.langframework.promptmanager.client.models.*;
import ai.langframework.promptmanager.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://goe0ty1i23.execute-api.us-east-1.amazonaws.com/default");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    String callerId = "callerId_example"; // String | 
    String search = "search_example"; // String | 
    try {
      Object result = apiInstance.searchPrompts(callerId, search);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#searchPrompts");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **callerId** | **String**|  | |
| **search** | **String**|  | [optional] |

### Return type

**Object**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | 200 response |  -  |

<a id="updateCategory"></a>
# **updateCategory**
> Object updateCategory(callerId, categoryId, categoryModel)



### Example
```java
// Import classes:
import ai.langframework.promptmanager.client.ApiClient;
import ai.langframework.promptmanager.client.ApiException;
import ai.langframework.promptmanager.client.Configuration;
import ai.langframework.promptmanager.client.models.*;
import ai.langframework.promptmanager.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://goe0ty1i23.execute-api.us-east-1.amazonaws.com/default");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    String callerId = "callerId_example"; // String | 
    String categoryId = "categoryId_example"; // String | 
    CategoryModel categoryModel = new CategoryModel(); // CategoryModel | 
    try {
      Object result = apiInstance.updateCategory(callerId, categoryId, categoryModel);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#updateCategory");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **callerId** | **String**|  | |
| **categoryId** | **String**|  | |
| **categoryModel** | [**CategoryModel**](CategoryModel.md)|  | |

### Return type

**Object**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | 200 response |  -  |

<a id="updatePrompt"></a>
# **updatePrompt**
> Object updatePrompt(promptId, callerId, promptModel)



### Example
```java
// Import classes:
import ai.langframework.promptmanager.client.ApiClient;
import ai.langframework.promptmanager.client.ApiException;
import ai.langframework.promptmanager.client.Configuration;
import ai.langframework.promptmanager.client.models.*;
import ai.langframework.promptmanager.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://goe0ty1i23.execute-api.us-east-1.amazonaws.com/default");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    String promptId = "promptId_example"; // String | 
    String callerId = "callerId_example"; // String | 
    PromptModel promptModel = new PromptModel(); // PromptModel | 
    try {
      Object result = apiInstance.updatePrompt(promptId, callerId, promptModel);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#updatePrompt");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **promptId** | **String**|  | |
| **callerId** | **String**|  | |
| **promptModel** | [**PromptModel**](PromptModel.md)|  | |

### Return type

**Object**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | 200 response |  -  |

<a id="updateUser"></a>
# **updateUser**
> Object updateUser(userId, callerId, userModel)



### Example
```java
// Import classes:
import ai.langframework.promptmanager.client.ApiClient;
import ai.langframework.promptmanager.client.ApiException;
import ai.langframework.promptmanager.client.Configuration;
import ai.langframework.promptmanager.client.models.*;
import ai.langframework.promptmanager.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://goe0ty1i23.execute-api.us-east-1.amazonaws.com/default");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    String userId = "userId_example"; // String | 
    String callerId = "callerId_example"; // String | 
    UserModel userModel = new UserModel(); // UserModel | 
    try {
      Object result = apiInstance.updateUser(userId, callerId, userModel);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#updateUser");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **userId** | **String**|  | |
| **callerId** | **String**|  | |
| **userModel** | [**UserModel**](UserModel.md)|  | |

### Return type

**Object**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | 200 response |  -  |

