---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : User = {
	additionalData : {
		ext55gb1l09_msLearnCourses : {
			courseType : "Admin",
		},
	},
};

const result = async () => {
	await graphServiceClient.usersById("user-id").patch(requestBody);
}


```