# ApiTemplateIoApiReference.PDFGenerationSettingsObject

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**paperSize** | **String** | Specifies the paper size for the PDF. The available options are Letter, Legal, Tabloid, Ledger, A0, A1, A2, A3, A4, A5,A6 or custom. custom dimensions specified as \&quot;custom_width\&quot; and \&quot;custom_height\&quot;.  | [optional] 
**customWidth** | **String** | Custom width for the custom paper size. Valid units are mm, px and cm. eg: 30mm  | [optional] 
**customHeight** | **String** | Custom height for the custom paper size. Valid units are mm, px and cm. eg: 30mm  | [optional] 
**orientation** | **String** | Specifies the orientation of the PDF. The available options are \&quot;1\&quot; for portrait and \&quot;2\&quot; for landscape.  | [optional] 
**headerFontSize** | **String** | Specifies the font size for the header in the PDF.  | [optional] 
**marginTop** | **String** | Specify the top margin for the PDF in millimeters (mm).  | [optional] 
**marginRight** | **String** | Specify the right margin for the PDF in millimeters (mm).  | [optional] 
**marginBottom** | **String** | Specify the bottom margin for the PDF in millimeters (mm).  | [optional] 
**marginLeft** | **String** | Specify the left margin for the PDF in millimeters (mm).  | [optional] 
**printBackground** | **String** | Specifies whether to print the background graphics and colors in the PDF. Set to \&quot;1\&quot; to include backgrounds or \&quot;0\&quot; to exclude them.  | [optional] 
**displayHeaderFooter** | **Boolean** | Specifies whether to display the header and footer in the PDF. Set to true to include the header and footer or false to exclude them.  | [optional] 
**customHeader** | **String** | Specify custom HTML markup for the headerof the PDF. These properties should contain valid HTML markup, including any necessary CSS styles.  | [optional] 
**customFooter** | **String** | Specify custom HTML markup for the footer of the PDF. These properties should contain valid HTML markup, including any necessary CSS styles.  | [optional] 


