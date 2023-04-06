---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : CreateUploadSessionPostRequestBody = {
	attachmentItem : {
		attachmentType : AttachmentType.File,
		name : "flower",
		size : 3483322,
	},
};

const result = async () => {
	await graphServiceClient.me.messagesById("message-id").attachments.createUploadSession.post(requestBody);
}


```