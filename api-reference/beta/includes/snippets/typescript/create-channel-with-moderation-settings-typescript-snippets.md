---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : Channel = {
	displayName : "TestChannelModeration",
	description : "Test channel moderation.",
	membershipType : ChannelMembershipType.Standard,
	moderationSettings : {
		userNewMessageRestriction : UserNewMessageRestriction.EveryoneExceptGuests,
		replyRestriction : ReplyRestriction.Everyone,
		allowNewMessageFromBots : true,
		allowNewMessageFromConnectors : true,
	},
};

const result = async () => {
	await graphServiceClient.teamsById("team-id").channels.post(requestBody);
}


```