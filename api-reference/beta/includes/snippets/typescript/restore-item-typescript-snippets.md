---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : RestorePostRequestBody = {
	parentReference : {
		id : "String",
	},
	name : "String",
};

const result = async () => {
	await graphServiceClient.drivesById("drive-id").itemsById("driveItem-id").restore.post(requestBody);
}


```