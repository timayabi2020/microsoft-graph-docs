---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : Extension = {
	additionalData : {
		"@odata.context" : "https://graph.microsoft.com/beta/$metadata#users('3fbd929d-8c56-4462-851e-0eb9a7b3a2a5')/extensions/$entity",
		"@odata.type" : "#microsoft.graph.openTypeExtension",
		"xboxGamerTag" : "FierceAdele",
		"linkedInProfile" : "www.linkedin.com/in/testlinkedinprofile",
		"id" : "com.contoso.socialSettings",
	},
};

const result = async () => {
	await graphServiceClient.usersById("user-id").extensionsById("extension-id").get(requestBody);
}


```