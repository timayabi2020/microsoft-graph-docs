---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : Group = {
	description : "Building security",
	displayName : "Building security",
	groupTypes : [
	],
	mailEnabled : false,
	mailNickname : "buildingsecurity",
	securityEnabled : true,
	additionalData : {
		"owners@odata.bind" : [
			"https://graph.microsoft.com/beta/users/d3bcdff4-4f80-4418-a65e-7bf3778c5dca",
		],
		"members@odata.bind" : [
			"https://graph.microsoft.com/beta/users/3b8ceebc-49e6-4e0c-9e14-c906374a7ef6",
			"https://graph.microsoft.com/beta/users/bf59c5ba-5304-4c9b-9192-e5a4cb8444e7",
		],
	},
};

const result = async () => {
	await graphServiceClient.groups.post(requestBody);
}


```