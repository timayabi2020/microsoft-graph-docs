---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : EducationAssignment = {
	displayName : "Reading and review test 09.03 #5",
	instructions : {
		contentType : BodyType.Text,
		content : "Read chapter 5 and write your review",
	},
	dueDateTime : new Date("2021-09-10T00:00:00Z"),
	addedStudentAction : EducationAddedStudentAction.None,
};

const result = async () => {
	await graphServiceClient.education.classesById("educationClass-id").assignmentsById("educationAssignment-id").patch(requestBody);
}


```