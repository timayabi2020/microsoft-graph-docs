---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const configuration = {
	queryParameters : {
		filter: "graphlearn_courses/courseId eq ‘123’",
		select: ["displayName","id","description","graphlearn_courses"],
	}
};

const result = async () => {
	await graphServiceClient.groups.get(configuration);
}


```