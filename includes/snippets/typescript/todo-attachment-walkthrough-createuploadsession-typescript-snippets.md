---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : CreateUploadSessionPostRequestBody = {
	attachmentInfo : {
		attachmentType : AttachmentType.File,
		name : "flower",
		size : 3483322,
	},
};

const result = async () => {
	await graphServiceClient.me.todo.listsById("todoTaskList-id").tasksById("todoTask-id").attachments.createUploadSession.post(requestBody);
}


```