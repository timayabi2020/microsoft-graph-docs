---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : Device = {
	accountEnabled : false,
	alternativeSecurityIds : [
		{
			type : 2,
			key : "base64Y3YxN2E1MWFlYw==",
		},
	],
	deviceId : "4c299165-6e8f-4b45-a5ba-c5d250a707ff",
	displayName : "Test device",
	operatingSystem : "linux",
	operatingSystemVersion : "1",
};

const result = async () => {
	await graphServiceClient.devices.post(requestBody);
}


```