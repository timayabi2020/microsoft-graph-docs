---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : GrantPostRequestBody = {
	recipients : [
		{
			email : "john@contoso.com",
		},
		{
			email : "ryan@external.com",
		},
	],
	roles : [
		"read",
	],
};

const result = async () => {
	await graphServiceClient.sharesById("sharedDriveItem-id").permission.grant.post(requestBody);
}


```