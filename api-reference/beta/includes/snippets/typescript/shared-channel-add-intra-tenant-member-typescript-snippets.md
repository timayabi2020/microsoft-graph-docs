---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : ConversationMember = {
	"@odata.type" : "#microsoft.graph.aadUserConversationMember",
	roles : [
	],
	additionalData : {
		"user@odata.bind" : "https://graph.microsoft.com/beta/users/24b3819b-4e1d-4f3e-86bd-e42b54d0b2b4",
	},
};

const result = async () => {
	await graphServiceClient.teamsById("team-id").channelsById("channel-id").members.post(requestBody);
}


```