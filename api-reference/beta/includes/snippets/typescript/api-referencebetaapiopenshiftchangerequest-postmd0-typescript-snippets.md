---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const configuration = {
	headers : {
		"Authorization": "Bearer {token}",
	}
};
const requestBody : OpenShiftChangeRequest = {
	senderMessage : "Can I take this shift?",
	openShiftId : "577b75d2-a927-48c0-a5d1-dc984894e7b8",
};

const result = async () => {
	await graphServiceClient.teamsById("team-id").schedule.openShiftChangeRequests.post(requestBody, configuration);
}


```