---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : Application = {
	additionalData : {
		onPremisesPublishing : {
			singleSignOnSettings : {
				kerberosSignOnSettings : {
					kerberosServicePrincipalName : "HTTP/iwademo.contoso.com",
					kerberosSignOnMappingAttributeType : "userPrincipalName",
				},
				singleSignOnMode : "onPremisesKerberos",
			},
		},
	},
};

async () => {
	await graphServiceClient.applicationsById("application-id").patch(requestBody);
}


```