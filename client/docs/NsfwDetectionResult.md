# Cloudmersive.APIClient.NETCore.MultiThreatScan.Model.NsfwDetectionResult
NSFW detection result

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Enabled** | **bool** | Whether this scan was enabled | [optional] 
**Successful** | **bool** | Whether this scan completed successfully | [optional] 
**CleanResult** | **bool** | True if no NSFW content was found | [optional] 
**ContainsNudity** | **bool** | Image contains nudity | [optional] 
**ContainsGraphicViolence** | **bool** | Image contains graphic violence | [optional] 
**ContainsNonGraphicViolence** | **bool** | Image contains non-graphic violence | [optional] 
**ContainsSelfHarm** | **bool** | Image contains self-harm content | [optional] 
**ContainsHate** | **bool** | Image contains hate content | [optional] 
**ContainsPotentialIllegalActivity** | **bool** | Image contains potential illegal activity | [optional] 
**ContainsMedicalImagery** | **bool** | Image contains medical imagery | [optional] 
**ContainsProfanity** | **bool** | Image contains profanity | [optional] 
**Score** | **double** | NSFW score (0.0 to 1.0) | [optional] 
**ClassificationOutcome** | **string** | Classification outcome | [optional] 
**Skipped** | **bool** | Scan was skipped (unsupported format) | [optional] 
**SkipReason** | **string** | Reason the scan was skipped | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

