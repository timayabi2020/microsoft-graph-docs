---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : EducationUser = {
	displayName : "Rogelio Cazares",
	givenName : "Rogelio",
	middleName : "Fernando",
	surname : "Cazares",
};

const result = async () => {
	await graphServiceClient.education.usersById("educationUser-id").patch(requestBody);
}


```