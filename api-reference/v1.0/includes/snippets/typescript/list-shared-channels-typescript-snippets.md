---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const configuration = {
	queryParameters : {
		filter: "membershipType eq 'shared'",
	}
};

const result = async () => {
	await graphServiceClient.teamsById("team-id").channels.get(configuration);
}


```