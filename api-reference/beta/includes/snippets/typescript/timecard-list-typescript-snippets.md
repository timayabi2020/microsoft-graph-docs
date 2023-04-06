---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const configuration = {
	queryParameters : {
		top: 2,
		filter: "state eq 'clockedOut'",
	}
};

const result = async () => {
	await graphServiceClient.teamsById("team-id").schedule.timeCards.get(configuration);
}


```