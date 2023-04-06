---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const configuration = {
	headers : {
		"Prefer": "return=representation",
	}
};
const requestBody : TimeOffReason = {
	additionalData : {
		"displayName" : "Vacation",
		"iconType" : "plane",
		isActive : true,
	},
};

async () => {
	await graphServiceClient.teamsById("team-id").schedule.timeOffReasonsById("timeOffReason-id").put(requestBody, configuration);
}


```