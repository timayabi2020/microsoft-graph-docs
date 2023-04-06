---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : Channel = {
	displayName : "Architecture Discussion",
	description : "This channel is where we debate all future architecture plans",
	membershipType : ChannelMembershipType.Standard,
};

const result = async () => {
	await graphServiceClient.teamsById("team-id").channels.post(requestBody);
}


```