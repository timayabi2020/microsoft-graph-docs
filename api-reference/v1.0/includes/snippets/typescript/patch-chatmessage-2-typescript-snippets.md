---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : ChatMessage = {
	messageType : ChatMessageType.Message,
	deletedDateTime : null,
	subject : null,
	summary : null,
	importance : ChatMessageImportance.Normal,
	locale : "en-us",
	from : {
		application : null,
		device : null,
		user : {
			id : "6b3f3c54-d09c-4fdd-b146-9b514a8a4f40",
			displayName : "Lam Cong",
			additionalData : {
				"userIdentityType" : "aadUser",
			},
		},
		additionalData : {
			conversation : null,
		},
	},
	body : {
		contentType : BodyType.Html,
		content : "<div><div>\n<div>\n<div>\n<div>\n<div><at id=\"0\">Raghav</at><at id=\"1\">TestGlobalBot</at> YEAH",
	},
	attachments : [
	],
	mentions : [
		{
			id : 0,
			mentionText : "Raghav",
			mentioned : {
				application : null,
				device : null,
				conversation : null,
				user : {
					id : "f1b66449-b46d-49b0-9c3c-53c10234c818e",
					displayName : "Lam Cong",
					additionalData : {
						"userIdentityType" : "aadUser",
					},
				},
			},
		},
		{
			id : 1,
			mentionText : "TestGlobalBot",
			mentioned : {
				application : {
					id : "03a02232-d8f5-4970-a77e-6e8c76ce7a4e",
					displayName : "TestGlobalBot",
					additionalData : {
						"applicationIdentityType" : "bot",
					},
				},
				device : null,
				conversation : null,
				user : null,
			},
		},
	],
	reactions : [
	],
};

const result = async () => {
	await graphServiceClient.teamsById("team-id").channelsById("channel-id").messagesById("chatMessage-id").patch(requestBody);
}


```