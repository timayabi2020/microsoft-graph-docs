---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : AgreementFileLocalization = {
	fileName : "Contoso ToU for guest users (French)",
	language : "fr-FR",
	isDefault : false,
	isMajorVersion : false,
	displayName : "Contoso ToU for guest users (French)",
	fileData : {
		data : "base64JVBERi0xLjUKJb/3ov4KNCAwIG9iago8PCAvTGluZWFyaX//truncated-binary-data",
	},
};

const result = async () => {
	await graphServiceClient.identityGovernance.termsOfUse.agreementsById("agreement-id").files.post(requestBody);
}


```