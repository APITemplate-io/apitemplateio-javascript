# ApiTemplateIoApiReference.TemplateManagementApi

All URIs are relative to *https://rest.apitemplate.io*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getTemplate**](TemplateManagementApi.md#getTemplate) | **GET** /v2/get-template | Get PDF template
[**listTemplates**](TemplateManagementApi.md#listTemplates) | **GET** /v2/list-templates | List Templates
[**updateTemplate**](TemplateManagementApi.md#updateTemplate) | **POST** /v2/update-template | Update PDF Template



## getTemplate

> ResponseSuccessTemplate getTemplate(opts)

Get PDF template

Retrieves information of the PDF template (**This is an experimental API, contact support to learn more**) 

### Example

```javascript
import ApiTemplateIoApiReference from 'api_template_io_api_reference';
let defaultClient = ApiTemplateIoApiReference.ApiClient.instance;
// Configure API key authorization: ApiKeyAuth
let ApiKeyAuth = defaultClient.authentications['ApiKeyAuth'];
ApiKeyAuth.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//ApiKeyAuth.apiKeyPrefix = 'Token';

let apiInstance = new ApiTemplateIoApiReference.TemplateManagementApi();
let opts = {
  'templateId': 00377b2b1e0ee394 // String | Your template id, it can be obtained in the web console(Manage Templates)
};
apiInstance.getTemplate(opts, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **templateId** | **String**| Your template id, it can be obtained in the web console(Manage Templates) | [optional] 

### Return type

[**ResponseSuccessTemplate**](ResponseSuccessTemplate.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## listTemplates

> ResponseSuccessListTemplates listTemplates(opts)

List Templates

Retrieves the information of templates 

### Example

```javascript
import ApiTemplateIoApiReference from 'api_template_io_api_reference';
let defaultClient = ApiTemplateIoApiReference.ApiClient.instance;
// Configure API key authorization: ApiKeyAuth
let ApiKeyAuth = defaultClient.authentications['ApiKeyAuth'];
ApiKeyAuth.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//ApiKeyAuth.apiKeyPrefix = 'Token';

let apiInstance = new ApiTemplateIoApiReference.TemplateManagementApi();
let opts = {
  'limit': 300, // String | Retrieve only the number of records specified. Default to 300
  'offset': 0, // String | Offset is used to skip the number of records from the results. Default to 0
  'format': JPEG, // String | To filter the templates by either 'PDF' or 'JPEG'
  'templateId': 00377b2b1e0ee394, // String | To filter the templates by template id
  'groupName': custom, // String | To filter the templates by the group name
  'withLayerInfo': 0 // String | Return along with layer information for image templates, 0=false , 1=true. Default to '0'
};
apiInstance.listTemplates(opts, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **limit** | **String**| Retrieve only the number of records specified. Default to 300 | [optional] 
 **offset** | **String**| Offset is used to skip the number of records from the results. Default to 0 | [optional] 
 **format** | **String**| To filter the templates by either &#39;PDF&#39; or &#39;JPEG&#39; | [optional] 
 **templateId** | **String**| To filter the templates by template id | [optional] 
 **groupName** | **String**| To filter the templates by the group name | [optional] 
 **withLayerInfo** | **String**| Return along with layer information for image templates, 0&#x3D;false , 1&#x3D;true. Default to &#39;0&#39; | [optional] 

### Return type

[**ResponseSuccessListTemplates**](ResponseSuccessListTemplates.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## updateTemplate

> ResponseSuccess updateTemplate(updateTemplateRequest)

Update PDF Template

This endpoint updates PDF template (**This is an experimental API, contact support to learn more**)

### Example

```javascript
import ApiTemplateIoApiReference from 'api_template_io_api_reference';
let defaultClient = ApiTemplateIoApiReference.ApiClient.instance;
// Configure API key authorization: ApiKeyAuth
let ApiKeyAuth = defaultClient.authentications['ApiKeyAuth'];
ApiKeyAuth.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//ApiKeyAuth.apiKeyPrefix = 'Token';

let apiInstance = new ApiTemplateIoApiReference.TemplateManagementApi();
let updateTemplateRequest = new ApiTemplateIoApiReference.UpdateTemplateRequest(); // UpdateTemplateRequest | 
apiInstance.updateTemplate(updateTemplateRequest, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **updateTemplateRequest** | [**UpdateTemplateRequest**](UpdateTemplateRequest.md)|  | 

### Return type

[**ResponseSuccess**](ResponseSuccess.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

