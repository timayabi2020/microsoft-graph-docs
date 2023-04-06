---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : ReferenceCreate = {
	"@odata.id" : "https://graph.microsoft.com/v1.0/users/{userId}",
};

const result = async () => {
	await graphServiceClient.print.sharesById("printerShare-id").allowedUsers.$ref.post(requestBody);
}


```