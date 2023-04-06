---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : SetCloudPcReviewStatusPostRequestBody = {
	reviewStatus : {
		inReview : true,
		userAccessLevel : CloudPcUserAccessLevel.Restricted,
		azureStorageAccountId : "/subscriptions/f68bd846-16ad-4b51-a7c6-c84944a3367c/resourceGroups/Review/providers/Microsoft.Storage/storageAccounts/snapshotsUnderReview",
	},
};

const result = async () => {
	await graphServiceClient.deviceManagement.managedDevicesById("managedDevice-id").setCloudPcReviewStatus.post(requestBody);
}


```