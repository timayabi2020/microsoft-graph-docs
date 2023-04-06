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
const requestBody : SwapShiftsChangeRequest = {
	senderShiftId : "5ad10161-6524-4c7c-9beb-4e8677ba2f6d",
	senderMessage : "I can't make my shift, any chance we can swap?",
	recipientUserId : "567c8ea5-9e32-422a-a663-8270201699cd",
	recipientShiftId : "e73408ca-3ea5-4bbf-96a8-2e06c95f7a2c",
};

const result = async () => {
	await graphServiceClient.teamsById("team-id").schedule.swapShiftsChangeRequests.post(requestBody, configuration);
}


```