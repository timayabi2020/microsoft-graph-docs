---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : Device = {
	accountEnabled : true,
	alternativeSecurityIds : [
		{
			type : 99,
			identityProvider : "identityProvider-value",
			key : "base64Y3YxN2E1MWFlYw==",
		},
	],
	approximateLastSignInDateTime : new Date("2016-10-19T10:37:00Z"),
	deviceId : "deviceId-value",
	deviceMetadata : "deviceMetadata-value",
	deviceVersion : 99,
};

const result = async () => {
	await graphServiceClient.devices.post(requestBody);
}


```