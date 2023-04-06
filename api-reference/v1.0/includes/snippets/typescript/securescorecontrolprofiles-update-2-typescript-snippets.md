---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : SecureScoreControlProfile = {
	vendorInformation : {
		provider : "SecureScore",
		providerVersion : null,
		subProvider : null,
		vendor : "Microsoft",
	},
	additionalData : {
		"assignedTo" : "",
		"comment" : "control is reviewed",
		"state" : "Reviewed",
	},
};

const result = async () => {
	await graphServiceClient.security.secureScoreControlProfilesById("secureScoreControlProfile-id").patch(requestBody);
}


```