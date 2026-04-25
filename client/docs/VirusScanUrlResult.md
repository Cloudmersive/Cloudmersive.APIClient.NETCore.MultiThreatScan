# Cloudmersive.APIClient.NETCore.MultiThreatScan.Model.VirusScanUrlResult
Virus scan result for URL scanning

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Enabled** | **bool** | Whether this scan was enabled | [optional] 
**Successful** | **bool** | Whether this scan completed successfully | [optional] 
**CleanResult** | **bool** | True if no threats were found | [optional] 
**WebsiteThreatType** | **string** | Website threat type: None, Malware, Phishing, ForcedDownload, UnableToConnect | [optional] 
**FoundViruses** | [**List&lt;VirusFound&gt;**](VirusFound.md) | List of viruses found | [optional] 
**WebsiteHttpResponseCode** | **int** | HTTP response code from the website | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

