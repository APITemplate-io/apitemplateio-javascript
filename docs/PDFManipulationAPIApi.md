# ApiTemplateIoApiReference.PDFManipulationAPIApi

All URIs are relative to *https://rest.apitemplate.io*

Method | HTTP request | Description
------------- | ------------- | -------------
[**mergePdfs**](PDFManipulationAPIApi.md#mergePdfs) | **POST** /v2/merge-pdfs | Join/Merge multiple PDFs



## mergePdfs

> ResponseSuccessSingleFile mergePdfs(mergePdfsRequest, opts)

Join/Merge multiple PDFs

This endpoint merges/joins multiple PDF URLs into a single PDF file

### Example

```javascript
import ApiTemplateIoApiReference from 'api_template_io_api_reference';
let defaultClient = ApiTemplateIoApiReference.ApiClient.instance;
// Configure API key authorization: ApiKeyAuth
let ApiKeyAuth = defaultClient.authentications['ApiKeyAuth'];
ApiKeyAuth.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//ApiKeyAuth.apiKeyPrefix = 'Token';

let apiInstance = new ApiTemplateIoApiReference.PDFManipulationAPIApi();
let mergePdfsRequest = new ApiTemplateIoApiReference.MergePdfsRequest(); // MergePdfsRequest | 
let opts = {
  'postactionS3Filekey': "postactionS3Filekey_example", // String | - This is to specify the file name for `Post Action(S3 Storage)`. - Please do not specify the file extension - Please make sure the file name is unique - You might use slash (/) as the folder delimiter 
  'postactionS3Bucket': "postactionS3Bucket_example", // String | - This is to overwrite the AWS Bucket for `Post Action(S3 Storage)`. 
  'meta': inv-iwj343jospig // String | - Specify an external reference ID for your own reference. It appears in the `list-objects` API. 
};
apiInstance.mergePdfs(mergePdfsRequest, opts, (error, data, response) => {
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
 **mergePdfsRequest** | [**MergePdfsRequest**](MergePdfsRequest.md)|  | 
 **postactionS3Filekey** | **String**| - This is to specify the file name for &#x60;Post Action(S3 Storage)&#x60;. - Please do not specify the file extension - Please make sure the file name is unique - You might use slash (/) as the folder delimiter  | [optional] 
 **postactionS3Bucket** | **String**| - This is to overwrite the AWS Bucket for &#x60;Post Action(S3 Storage)&#x60;.  | [optional] 
 **meta** | **String**| - Specify an external reference ID for your own reference. It appears in the &#x60;list-objects&#x60; API.  | [optional] 

### Return type

[**ResponseSuccessSingleFile**](ResponseSuccessSingleFile.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

