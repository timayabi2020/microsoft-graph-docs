---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : ConversationMember = {
	"@odata.type" : "#microsoft.graph.aadUserConversationMember",
	roles : [
		"owner",
	],
	additionalData : {
		"user@odata.bind" : "https://graph.microsoft.com/v1.0/users('jacob@contoso.com')",
	},
};

const result = async () => {
	await graphServiceClient.teamsById("team-id").members.post(requestBody);
}


```