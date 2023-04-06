---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : Team = {
	isMembershipLimitedToOwners : true,
	memberSettings : {
		allowCreateUpdateChannels : true,
	},
	messagingSettings : {
		allowUserEditMessages : true,
		allowUserDeleteMessages : true,
	},
	funSettings : {
		allowGiphy : true,
		giphyContentRating : GiphyRatingType.Strict,
	},
	discoverySettings : {
		showInTeamsSearchAndSuggestions : true,
	},
};

const result = async () => {
	await graphServiceClient.teamsById("team-id").patch(requestBody);
}


```