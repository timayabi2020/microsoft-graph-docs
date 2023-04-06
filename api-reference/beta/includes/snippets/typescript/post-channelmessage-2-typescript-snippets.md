---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : ChatMessage = {
	createdDateTime : new Date("2019-02-04T19:58:15.511Z"),
	from : {
		user : {
			id : "id-value",
			displayName : "Joh Doe",
			additionalData : {
				"userIdentityType" : "aadUser",
			},
		},
	},
	body : {
		contentType : BodyType.Html,
		content : "Hello World",
	},
};

const result = async () => {
	await graphServiceClient.teamsById("team-id").channelsById("channel-id").messages.post(requestBody);
}


```