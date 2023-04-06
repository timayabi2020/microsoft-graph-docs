---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : Application = {
	identifierUris : [
		"https://contosoiwaapp-contoso.msappproxy.net",
	],
	web : {
		redirectUris : [
			"https://contosoiwaapp-contoso.msappproxy.net",
		],
		homePageUrl : "https://contosoiwaapp-contoso.msappproxy.net",
	},
};

const result = async () => {
	await graphServiceClient.applicationsById("application-id").patch(requestBody);
}


```