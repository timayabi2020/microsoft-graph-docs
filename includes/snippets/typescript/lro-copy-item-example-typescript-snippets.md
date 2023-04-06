---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : CopyPostRequestBody = {
	parentReference : {
		path : "/drive/root:/Documents",
	},
	name : "Copy of LargeFolder1",
};

const result = async () => {
	await graphServiceClient.drivesById("drive-id").itemsById("driveItem-id").copy.post(requestBody);
}


```