---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : AttachmentBase = {
	"@odata.type" : "#microsoft.graph.taskFileAttachment",
	name : "smile",
	contentType : "image/gif",
	additionalData : {
		"contentBytes" : "a0b1c76de9f7=",
	},
};

const result = async () => {
	await graphServiceClient.me.todo.listsById("todoTaskList-id").tasksById("todoTask-id").attachments.post(requestBody);
}


```