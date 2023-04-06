---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : MuteAllPostRequestBody = {
	participants : [
		"",
	],
	clientContext : "clientContext-value",
};

const result = async () => {
	await graphServiceClient.communications.callsById("call-id").participants.muteAll.post(requestBody);
}


```