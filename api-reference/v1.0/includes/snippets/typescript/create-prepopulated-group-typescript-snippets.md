---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : Group = {
	description : "Group with designated owner and members",
	displayName : "Operations group",
	groupTypes : [
	],
	mailEnabled : false,
	mailNickname : "operations2019",
	securityEnabled : true,
	additionalData : {
		"owners@odata.bind" : [
			"https://graph.microsoft.com/v1.0/users/26be1845-4119-4801-a799-aea79d09f1a2",
		],
		"members@odata.bind" : [
			"https://graph.microsoft.com/v1.0/users/ff7cb387-6688-423c-8188-3da9532a73cc",
			"https://graph.microsoft.com/v1.0/users/69456242-0067-49d3-ba96-9de6f2728e14",
		],
	},
};

const result = async () => {
	await graphServiceClient.groups.post(requestBody);
}


```