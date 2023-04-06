---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : MakePermanentPostRequestBody = {
	reason : "reason-value",
	ticketNumber : "ticketNumber-value",
	ticketSystem : "ticketSystem-value",
};

const result = async () => {
	await graphServiceClient.privilegedRoleAssignmentsById("privilegedRoleAssignment-id").makePermanent.post(requestBody);
}


```