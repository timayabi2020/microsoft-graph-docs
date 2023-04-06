---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : EducationSubmissionResource = {
	resource : {
		displayName : "Wikipedia",
		"@odata.type" : "#microsoft.graph.educationLinkResource",
		additionalData : {
			"link" : "https://en.wikipedia.org/wiki/Main_Page",
		},
	},
};

const result = async () => {
	await graphServiceClient.education.classesById("educationClass-id").assignmentsById("educationAssignment-id").submissionsById("educationSubmission-id").resources.post(requestBody);
}


```