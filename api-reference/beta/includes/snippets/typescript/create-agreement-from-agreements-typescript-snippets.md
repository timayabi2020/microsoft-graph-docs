---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : Agreement = {
	displayName : "Contoso ToU for guest users",
	isViewingBeforeAcceptanceRequired : true,
	files : [
		{
			fileName : "TOU.pdf",
			language : "en",
			isDefault : true,
			fileData : {
				data : "sGVsbG8gd29ybGQ=//truncated-binary",
			},
		},
	],
};

const result = async () => {
	await graphServiceClient.identityGovernance.termsOfUse.agreements.post(requestBody);
}


```