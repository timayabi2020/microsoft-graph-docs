---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const configuration = {
	queryParameters : {
		top: 3,
	}
};

const result = async () => {
	await graphServiceClient.education.classesById("educationClass-id").assignmentCategories.delta().get(configuration);
}


```