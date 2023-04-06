---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : ProfileCardProperty = {
	directoryPropertyName : "CustomAttribute1",
	annotations : [
		{
			displayName : "Cost Center",
			localizations : [
				{
					languageTag : "ru-RU",
					displayName : "центр затрат",
				},
			],
		},
	],
};

const result = async () => {
	await graphServiceClient.organizationById("organization-id").settings.profileCardProperties.post(requestBody);
}


```