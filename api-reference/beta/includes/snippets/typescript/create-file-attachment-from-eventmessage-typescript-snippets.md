---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : Attachment = {
	"@odata.type" : "#Microsoft.OutlookServices.FileAttachment",
	name : "name-value",
	contentType : "contentType-value",
	isInline : false,
	additionalData : {
		"contentLocation" : "contentLocation-value",
		"contentBytes" : "contentBytes-value",
	},
};

const result = async () => {
	await graphServiceClient.me.messagesById("message-id").attachments.post(requestBody);
}


```