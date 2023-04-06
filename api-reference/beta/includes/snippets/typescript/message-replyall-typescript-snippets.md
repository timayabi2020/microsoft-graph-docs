---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : ReplyAllPostRequestBody = {
	message : {
		attachments : [
			{
				"@odata.type" : "#microsoft.graph.fileAttachment",
				name : "guidelines.txt",
				additionalData : {
					"contentBytes" : "bWFjIGFuZCBjaGVlc2UgdG9kYXk=",
				},
			},
		],
	},
	comment : "Please take a look at the attached guidelines before you decide on the name.",
};

const result = async () => {
	await graphServiceClient.me.messagesById("message-id").replyAll.post(requestBody);
}


```