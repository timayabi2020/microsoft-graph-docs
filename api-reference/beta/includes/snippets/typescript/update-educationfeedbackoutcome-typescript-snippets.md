---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : EducationOutcome = {
	"@odata.type" : "#microsoft.graph.educationFeedbackOutcome",
	additionalData : {
		feedback : {
			text : {
				content : "This is feedback for the assignment as a whole.",
				contentType : "text",
			},
		},
	},
};

const result = async () => {
	await graphServiceClient.education.classesById("educationClass-id").assignmentsById("educationAssignment-id").submissionsById("educationSubmission-id").outcomesById("educationOutcome-id").patch(requestBody);
}


```