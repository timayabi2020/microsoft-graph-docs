---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : RestorePostRequestBody = {
	cloudPcSnapshotId : "A00009UV000_93aff428-61f2-467f-a879-1102af6fd4a8",
};

const result = async () => {
	await graphServiceClient.deviceManagement.virtualEndpoint.cloudPCsById("cloudPC-id").restore.post(requestBody);
}


```