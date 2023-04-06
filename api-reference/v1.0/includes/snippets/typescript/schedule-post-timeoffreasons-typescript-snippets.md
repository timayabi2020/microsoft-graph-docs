---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : TimeOffReason = {
	displayName : "Vacation",
	iconType : TimeOffReasonIconType.Plane,
	isActive : true,
};

const result = async () => {
	await graphServiceClient.teamsById("team-id").schedule.timeOffReasons.post(requestBody);
}


```