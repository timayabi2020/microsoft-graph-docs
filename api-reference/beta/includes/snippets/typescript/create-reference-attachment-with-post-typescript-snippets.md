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
			content : "I attached a reference to a file on OneDrive.",
		},
		attachments : [
			{
				"@odata.type" : "#microsoft.graph.referenceAttachment",
				name : "Personal pictures",
				additionalData : {
					"sourceUrl" : "https://contoso.com/personal/mario_contoso_net/Documents/Pics",
					"providerType" : "oneDriveConsumer",
					"permission" : "Edit",
					"isFolder" : "True",
				},
			},
		],
	},
};

const result = async () => {
	await graphServiceClient.groupsById("group-id").threadsById("conversationThread-id").reply.post(requestBody);
}


```