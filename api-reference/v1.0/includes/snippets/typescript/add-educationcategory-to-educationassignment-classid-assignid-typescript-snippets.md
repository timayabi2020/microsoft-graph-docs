---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});


const result = async () => {
	await graphServiceClient.education.classesById("educationClass-id").assignmentsById("educationAssignment-id").categoriesById("educationCategory-id").$ref.delete();
}


```