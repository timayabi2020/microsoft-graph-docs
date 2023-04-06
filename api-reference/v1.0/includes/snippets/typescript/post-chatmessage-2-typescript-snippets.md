---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : ChatMessage = {
	body : {
		contentType : BodyType.Html,
		content : "Hello World <at id=\"0\">Jane Smith</at>",
	},
	mentions : [
		{
			id : 0,
			mentionText : "Jane Smith",
			mentioned : {
				user : {
					displayName : "Jane Smith",
					id : "ef1c916a-3135-4417-ba27-8eb7bd084193",
					additionalData : {
						"userIdentityType" : "aadUser",
					},
				},
			},
		},
	],
};

const result = async () => {
	await graphServiceClient.teamsById("team-id").channelsById("channel-id").messages.post(requestBody);
}


```