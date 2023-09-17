# ApiTemplateIoApiReference.CreatePdfFromHtmlRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**body** | **String** | The HTML body content for the PDF. This property supports HTML markup and can include Jinja2 syntax (e.g {{name}}). The value of {{name}} will be replaced with the actual value provided in the data object.  | [optional] 
**css** | **String** | The CSS styles to be applied to the PDF. This property should contain valid CSS markup and should also include the style tag.  | [optional] 
**data** | **Object** | The data object containing values for dynamic content in the HTML body. This object should include properties with corresponding values.  | [optional] 
**settings** | [**PDFGenerationSettingsObject**](PDFGenerationSettingsObject.md) |  | [optional] 


