---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : SecurityAction = {
	name : "BlockIp",
	actionReason : "Test",
	parameters : [
		{
			name : "IP",
			value : "1.2.3.4",
		},
	],
	vendorInformation : {
		provider : "Windows Defender ATP",
		vendor : "Microsoft",
	},
};

const result = async () => {
	await graphServiceClient.security.securityActions.post(requestBody);
}


```