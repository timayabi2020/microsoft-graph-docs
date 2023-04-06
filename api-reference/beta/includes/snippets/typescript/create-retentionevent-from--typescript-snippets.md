---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : RetentionEvent = {
	"@odata.type" : "#microsoft.graph.security.retentionEvent",
	displayName : "String",
	description : "String",
	eventQueries : [
		{
			"@odata.type" : "microsoft.graph.security.eventQueries",
		},
	],
	eventTriggerDateTime : new Date("String (timestamp)"),
	createdBy : {
		"@odata.type" : "microsoft.graph.identitySet",
	},
	eventPropagationResults : [
		{
			"@odata.type" : "microsoft.graph.security.eventPropagationResult",
		},
	],
	eventStatus : {
		"@odata.type" : "microsoft.graph.security.retentionEventStatus",
	},
	lastStatusUpdateDateTime : new Date("String (timestamp)"),
};

const result = async () => {
	await graphServiceClient.security.triggers.retentionEvents.post(requestBody);
}


```