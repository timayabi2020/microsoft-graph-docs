---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : Group = {
	description : "Feelgood Marketing Campaign with external partners and vendors.",
	displayName : "Feelgood Marketing Campaign",
	groupTypes : [
		"Unified",
	],
	mailEnabled : true,
	mailNickname : "FeelGoodCampaign",
	securityEnabled : true,
	additionalData : {
		"owners@odata.bind" : [
			"https://graph.microsoft.com/v1.0/users/cdb555e3-b33e-4fd5-a427-17fadacbdfa7",
		],
		"members@odata.bind" : [
			"https://graph.microsoft.com/v1.0/users/baf1b0a0-1f9a-4a56-9884-6a30824f8d20",
		],
	},
};

const result = async () => {
	await graphServiceClient.groups.post(requestBody);
}


```