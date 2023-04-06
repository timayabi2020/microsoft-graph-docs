---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : Extension = {
	"@odata.type" : "microsoft.graph.openTypeExtension",
	additionalData : {
		"extensionName" : "com.contoso.roamingSettings",
		"theme" : "dark",
		"color" : "purple",
		"lang" : "Japanese",
	},
};

const result = async () => {
	await graphServiceClient.me.extensions.post(requestBody);
}


```