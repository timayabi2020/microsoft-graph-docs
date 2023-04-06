---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : RetentionEventType = {
	"@odata.type" : "#microsoft.graph.security.retentionEventType",
	displayName : "String",
	description : "String",
	createdBy : {
		"@odata.type" : "microsoft.graph.identitySet",
	},
};

const result = async () => {
	await graphServiceClient.security.triggerTypes.retentionEventTypes.post(requestBody);
}


```