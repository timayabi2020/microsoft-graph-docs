---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : ReferenceCreate = {
	"@odata.id" : "https://graph.microsoft.com/v1.0/education/users/13015",
};

const result = async () => {
	await graphServiceClient.education.classesById("educationClass-id").members.$ref.post(requestBody);
}


```