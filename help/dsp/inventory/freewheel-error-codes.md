---
title: Error Codes for FreeWheel Ad Submissions
description: Reference the error codes that are returned for ad submissions to FreeWheel.
feature: inventory, deal IDs
exl-id: 
---
# Error Codes for FreeWheel Ad Submissions

The error messages for failed ad submissions can come from either Advertising Cloud DSP or from FreeWheel. Error messages are shown in the API Response column in the [Freewheel Status](freewheel-check-status.md) dialog.

## Advertising Cloud DSP Internal Errors

|Error Message|Description|Next Steps|
|--- |--- |--- |
|Awaiting status response from Freewheel|Freewheel hasn't yet responded that the submission was successful or failed.|Check the status again in 10 minutes.|
|The submitted ad does not have a clock number assigned.|Freewheel doesn't accept UK ads without assigned clock numbers.|Assign a clock number to the ad, and then resubmit the ad.|
|The ad you are attempting to submit has not yet finished transcoding. Please wait ten minutes then try again.|The transcoder hadn't finished transcoding the ad when you attempted to submit the ad.|Wait ten minutes, and then resubmit the ad.|
|The deal id you input is not setup as a guaranteed feed. Please submit guaranteed deals only.|The submitted deal is not set up as a programmatic guaranteed deal. Freewheel accepts only guaranteed deals.|Set up the deal ID as a programmatic guaranteed deal. The ad is automatically submitted to Freewheel when you save the programmatic guaranteed default placement at the end of deal ID workflow.|
|Invalid external_deal_id: \<deal_id\>|The submitted deal ID either doesn't exist or isn't active on the Adobe end.|Make sure that the deal is active, and then resubmit the ad.|
|\[public_id=\<deal\>] does not exist|The submitted deal id doesn't exist on the Freewheel end.|Contact your Freewheel representative to confirm the deal ID.|
|Ad with identifier \<*ad name*\> was not found.|The submitted ad key either doesn't exist or isn't active on the Adobe end.|Find the correct ad key, and then resubmit the ad.|
|Pending Submission|The submission is still pending.|Refresh the page.|

## FreeWheel API Errors

|Code|Meaning|Description|Next Steps|
|--- |--- |--- |--- |
|401|Unauthorized|Incorrect, missing, or invalid access credentials.|Contact your Adobe account manager.|
|403|Forbidden|The server understood the request but refuses to authorize it.|Contact your Adobe account manager.|
|404|Not Found|The resource you requested is not available. If the Creative ID is not found in the PUT operation, a 404 is returned.|Contact your Adobe account manager.|
|405|Method Not Allowed|A request was made of a resource using a request method not supported by that resource (for example, using GET on a method that requires data to be sent by POST, or using PUT on a read-only resource).|Contact your Adobe account manager.|
|408|Request Timeout|A timeout occurred while this request was processing. Timeouts are usually caused by concurrent requests of exclusive access to certain resources.|Resubmit the request when you receive this status. If the issue persists, contact your Adobe account manager.|
|422|Unprocessable Entity|Invalid resource. This error happens when the request body is invalid or the created/updated resource is invalid (for example, if the Deal ID was not found). See [FreeWheel API 422 Errors](#freewheel-422-errors) for more information.|Contact your Adobe account manager.|
|500|Internal Server Error|API system error.|Contact your Adobe account manager.|

  ## FreeWheel API 422 Errors {#freewheel-422-errors}

|Code|HTTP Code|Description|
|--- |--- |--- |
|DATA_UNMARSHALL_FAILURE|422|The request data is invalid json format. Check the error message for details.|
|DATA_VALIDATION_FAILURE|422|The request data is missing required fields or has an invalid data type. Check the error message for details.|
|DATA_DEAL_INVALID|422|The deal is configured incorrectly or doesn't exist. Check the error message for details.|
|DATA_DEAL_GET_FAILURE|422|The deal wasn't found or its configuration has an issue. Check the error message for details.|
|DATA_CREATIVE_INGEST_FAILURE|422|The creative URL is invalid. Check the error message for details.|
|DATA_CREATIVE_LINK_FAILURE|422|The creative wasn't linked to the ad unit nodes of the deal. Check the error message for details.|
|DATA_CREATIVE_UPDATE_FAILURE|422|The creative wasn't updated. Check the error message for details.|
|DATA_DSP_GET_FAILURE|422|The DSP doesn't exist within the system.|
|DATA_CREATIVE_UNLINK_FAILURE|422|The creative wasn't unlinked from ad units.|
|DATA_CREATIVE_DELETE_FAILURE|422|The creative wasn't deleted.|
|DATA_CREATIVE_DETECTION_FAILURE|422|The URL wasn't detected.|
|DATA_ENTITY_NOT_FOUND|422|The creative doesn't exist.|

>[!MORELIKETHIS]
>
>* [Overview of Setting up Programmatic Guaranteed Deals in FreeWheel](/help/dsp/inventory/freewheel-overview.md)
>* [Accept a Deal in the Deal ID Inbox](deal-id-inbox-accept.md)
>* [Submit an Ad for a Programmatic Guaranteed Deal to FreeWheel](/help/dsp/inventory/freewheel-submit.md)
>* [Check the Status of Ads for Freewheel Programmatic Guaranteed Deals](/help/dsp/inventory/freewheel-check-status.md)
