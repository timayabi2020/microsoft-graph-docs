---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : ServicePrincipal = {
	customSecurityAttributes : {
		additionalData : {
			engineering : {
				"@odata.type" : "#Microsoft.DirectoryServices.CustomSecurityAttributeValue",
				projectDate : "2022-10-01",
			},
		},
	},
};

const result = async () => {
	await graphServiceClient.servicePrincipalsById("servicePrincipal-id").patch(requestBody);
}


```