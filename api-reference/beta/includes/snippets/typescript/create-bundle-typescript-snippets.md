---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : DriveItem = {
	name : "Just some files",
	bundle : {
	},
	children : [
		{
			id : "1234asdf",
		},
		{
			id : "1234qwerty",
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