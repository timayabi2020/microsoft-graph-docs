---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : DriveItem = {
	name : "My Day at the Beach",
	bundle : {
		album : {
		},
	},
	children : [
		{
			id : "1234asdf",
		},
	],
	additionalData : {
		"@microsoft.graph.conflictBehavior" : "rename",
	},
};

const result = async () => {
	await graphServiceClient.drivesById("drive-id").bundles.post(requestBody);
}


```