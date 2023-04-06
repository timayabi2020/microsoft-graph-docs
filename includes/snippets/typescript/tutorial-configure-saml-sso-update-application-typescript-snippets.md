---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : Application = {
	web : {
		redirectUris : [
			"https://signin.aws.amazon.com/saml",
		],
	},
	identifierUris : [
		"https://signin.aws.amazon.com/saml",
	],
};

const result = async () => {
	await graphServiceClient.applicationsById("application-id").patch(requestBody);
}


```