---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : EducationSchool = {
	displayName : "Fabrikam Arts High School",
	description : "Magnate school for the arts. Los Angeles School District",
};

const result = async () => {
	await graphServiceClient.education.schoolsById("educationSchool-id").patch(requestBody);
}


```