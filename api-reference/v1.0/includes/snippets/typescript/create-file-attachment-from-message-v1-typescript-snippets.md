---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : Attachment = {
	"@odata.type" : "#microsoft.graph.fileAttachment",
	name : "smile",
	additionalData : {
		"contentBytes" : "R0lGODdhEAYEAA7",
	},
};

const result = async () => {
	await graphServiceClient.me.messagesById("message-id").attachments.post(requestBody);
}


```