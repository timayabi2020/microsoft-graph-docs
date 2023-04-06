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
			content : "content-value",
		},
		receivedDateTime : new Date("datetime-value"),
		hasAttachments : true,
		from : {
			emailAddress : {
				name : "name-value",
				address : "address-value",
			},
		},
		sender : {
			emailAddress : {
				name : "name-value",
				address : "address-value",
			},
		},
		conversationThreadId : "conversationThreadId-value",
		newParticipants : [
			{
				emailAddress : {
					name : "name-value",
					address : "address-value",
				},
			},
		],
		conversationId : "conversationId-value",
		createdDateTime : new Date("datetime-value"),
		lastModifiedDateTime : new Date("datetime-value"),
		changeKey : "changeKey-value",
		categories : [
			"categories-value",
		],
		id : "id-value",
		inReplyTo : {
		},
		attachments : [
			{
				"@odata.type" : "#microsoft.graph.fileAttachment",
				lastModifiedDateTime : new Date("datetime-value"),
				name : "name-value",
				contentType : "contentType-value",
				size : 99,
				isInline : true,
				id : "id-value",
			},
		],
	},
};

const result = async () => {
	await graphServiceClient.groupsById("group-id").threadsById("conversationThread-id").postsById("post-id").reply.post(requestBody);
}


```