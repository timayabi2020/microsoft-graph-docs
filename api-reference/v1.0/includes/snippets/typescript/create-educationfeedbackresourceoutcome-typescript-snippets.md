---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : EducationOutcome = {
	"@odata.type" : "#microsoft.graph.educationFeedbackResourceOutcome",
	additionalData : {
		feedbackResource : {
			"@odata.type" : "#microsoft.graph.educationWordResource",
			displayName : "Document1.docx",
		},
	},
};

const result = async () => {
	await graphServiceClient.education.classesById("educationClass-id").assignmentsById("educationAssignment-id").submissionsById("educationSubmission-id").outcomes.post(requestBody);
}


```