---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : Application = {
	requiredResourceAccess : [
		{
			resourceAppId : "00000002-0000-0000-c000-000000000000",
			resourceAccess : [
				{
					id : "311a71cc-e848-46a1-bdf8-97ff7156d8e6",
					type : "Scope",
				},
				{
					id : "3afa6a7d-9b1a-42eb-948e-1650a849e176",
					type : "Role",
				},
			],
		},
	],
};

const result = async () => {
	await graphServiceClient.applicationsById("application-id").patch(requestBody);
}


```