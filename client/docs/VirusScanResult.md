# Cloudmersive.APIClient.NETCore.MultiThreatScan.Model.VirusScanResult
Virus scan result

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Enabled** | **bool** | Whether this scan was enabled | [optional] 
**Successful** | **bool** | Whether this scan completed successfully | [optional] 
**CleanResult** | **bool** | True if no threats were found | [optional] 
**ContainsExecutable** | **bool** | Contains executable content | [optional] 
**ContainsInvalidFile** | **bool** | Contains invalid file structure | [optional] 
**ContainsScript** | **bool** | Contains script content | [optional] 
**ContainsPasswordProtectedFile** | **bool** | File is password-protected | [optional] 
**ContainsRestrictedFileFormat** | **bool** | File format is restricted | [optional] 
**ContainsMacros** | **bool** | Contains macro code | [optional] 
**ContainsXmlExternalEntities** | **bool** | Contains XML external entities | [optional] 
**ContainsInsecureDeserialization** | **bool** | Contains insecure deserialization | [optional] 
**ContainsHtml** | **bool** | Contains HTML content | [optional] 
**ContainsUnsafeArchive** | **bool** | Contains unsafe archive structure | [optional] 
**ContainsOleEmbeddedObject** | **bool** | Contains OLE embedded objects | [optional] 
**ContainsUnwantedAction** | **bool** | Contains unwanted actions | [optional] 
**VerifiedFileFormat** | **string** | Content-verified file format | [optional] 
**FoundViruses** | [**List&lt;VirusFound&gt;**](VirusFound.md) | List of viruses found | [optional] 
**ContentInformation** | [**VirusScanContentInfo**](VirusScanContentInfo.md) |  | [optional] 
**ErrorMessage** | **string** | Error message if the scan failed | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

