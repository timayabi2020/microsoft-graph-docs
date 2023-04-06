---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : ReplyPostRequestBody = {
	post : {
		body : {
			contentType : BodyType.Text,
			content : "Which quarter does that file cover? See my attachment.",
		},
		attachments : [
			{
				"@odata.type" : "#microsoft.graph.fileAttachment",
				name : "Another file as attachment",
				additionalData : {
					"contentBytes" : "VGhpcyBpcyBhIGZpbGUgdG8gYmUgYXR0YWNoZWQu",
				},
			},
		],
	},
};

const result = async () => {
	await graphServiceClient.groupsById("group-id").threadsById("conversationThread-id").reply.post(requestBody);
}


```