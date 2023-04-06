---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const configuration = {
	headers : {
		"Prefer": "return=representation",
	}
};
const requestBody : TiIndicator = {
	additionalInformation : "additionalInformation-after-update",
	confidence : 42,
	description : "description-after-update",
};

const result = async () => {
	await graphServiceClient.security.tiIndicatorsById("tiIndicator-id").patch(requestBody, configuration);
}


```