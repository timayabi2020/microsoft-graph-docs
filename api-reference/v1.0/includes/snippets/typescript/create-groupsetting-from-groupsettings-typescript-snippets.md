---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : GroupSetting = {
	templateId : "62375ab9-6b52-47ed-826b-58e47e0e304b",
	values : [
		{
			name : "GuestUsageGuidelinesUrl",
			value : "https://privacy.contoso.com/privacystatement",
		},
		{
			name : "EnableMSStandardBlockedWords",
			value : "true",
		},
		{
			name : "EnableMIPLabels",
			value : "true",
		},
		{
			name : "PrefixSuffixNamingRequirement",
			value : "[Contoso-][GroupName]",
		},
	],
};

const result = async () => {
	await graphServiceClient.groupSettings.post(requestBody);
}


```