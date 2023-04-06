---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : Group = {
	description : "Marketing department folks",
	displayName : "Marketing department",
	groupTypes : [
		"Unified",
		"DynamicMembership",
	],
	mailEnabled : true,
	mailNickname : "marketing",
	securityEnabled : false,
	membershipRule : "user.department -eq \"Marketing\"",
	membershipRuleProcessingState : "on",
};

const result = async () => {
	await graphServiceClient.groups.post(requestBody);
}


```