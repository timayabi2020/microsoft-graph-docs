---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : GroupLifecyclePolicy = {
	groupLifetimeInDays : 180,
	managedGroupTypes : "Selected",
	alternateNotificationEmails : "admin@contoso.com",
};

const result = async () => {
	await graphServiceClient.groupLifecyclePoliciesById("groupLifecyclePolicy-id").patch(requestBody);
}


```