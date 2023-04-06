---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : ReferenceCreate = {
	"@odata.id" : "https://graph.microsoft.com/beta/education/classes/11006",
};

const result = async () => {
	await graphServiceClient.education.schoolsById("educationSchool-id").classes.$ref.post(requestBody);
}


```