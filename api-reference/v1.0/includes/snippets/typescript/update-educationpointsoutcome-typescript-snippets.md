---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : EducationOutcome = {
	"@odata.type" : "#microsoft.graph.educationPointsOutcome",
	additionalData : {
		points : {
			"@odata.type" : "#microsoft.graph.educationAssignmentPointsGrade",
			points : 85.0,
		},
	},
};

const result = async () => {
	await graphServiceClient.education.classesById("educationClass-id").assignmentsById("educationAssignment-id").submissionsById("educationSubmission-id").outcomesById("educationOutcome-id").patch(requestBody);
}


```