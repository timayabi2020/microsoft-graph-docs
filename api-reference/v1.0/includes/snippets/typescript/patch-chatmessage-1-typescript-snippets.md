---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : ChatMessage = {
	messageType : ChatMessageType.Message,
	subject : null,
	summary : null,
	importance : ChatMessageImportance.Normal,
	locale : "en-us",
	from : {
		application : null,
		device : null,
		user : {
			id : "3b102402-813e-4e17-a6b2-f841aef1fdfc",
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
		contentType : BodyType.Text,
		content : "Edit text only",
	},
	attachments : [
	],
	mentions : [
	],
	reactions : [
	],
};

const result = async () => {
	await graphServiceClient.teamsById("team-id").channelsById("channel-id").messagesById("chatMessage-id").patch(requestBody);
}


```