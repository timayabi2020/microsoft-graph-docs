---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : Attachment = {
	"@odata.type" : "#Microsoft.OutlookServices.ItemAttachment",
	name : "name-value",
	additionalData : {
		item : {
			"@odata.type" : "microsoft.graph.message",
		},
	},
};

const result = async () => {
	await graphServiceClient.me.eventsById("event-id").attachments.post(requestBody);
}


```