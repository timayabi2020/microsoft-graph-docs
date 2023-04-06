---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : LanguageProficiency = {
	displayName : "Norwegian Bokmål",
	tag : "nb-NO",
	spoken : LanguageProficiencyLevel.NativeOrBilingual,
	written : LanguageProficiencyLevel.NativeOrBilingual,
	reading : LanguageProficiencyLevel.NativeOrBilingual,
};

const result = async () => {
	await graphServiceClient.me.profile.languages.post(requestBody);
}


```