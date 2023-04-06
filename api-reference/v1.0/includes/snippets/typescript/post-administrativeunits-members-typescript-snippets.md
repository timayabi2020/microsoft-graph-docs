---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : MembersPostRequestBody = {
	additionalData : {
		"@odata.type" : "#microsoft.graph.group",
		"description" : "Self help community for golf",
		"displayName" : "Golf Assist",
		groupTypes : [
			"Unified",
		],
		mailEnabled : true,
		"mailNickname" : "golfassist",
		securityEnabled : false,
	},
};

async () => {
	await graphServiceClient.directory.administrativeUnitsById("administrativeUnit-id").members.post(requestBody);
}


```