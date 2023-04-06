---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : Extension = {
	"@odata.type" : "#microsoft.graph.openTypeExtension",
	id : "com.contoso.socialSettings",
	additionalData : {
		"extensionName" : "com.contoso.socialSettings",
		"skypeId" : "skypeId.AdeleV",
		"linkedInProfile" : "www.linkedin.com/in/testlinkedinprofile",
		"xboxGamerTag" : "AwesomeAdele",
	},
};

const result = async () => {
	await graphServiceClient.usersById("user-id").extensions.post(requestBody);
}


```