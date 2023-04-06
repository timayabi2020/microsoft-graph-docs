---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : EducationAssignmentResource = {
	distributeForStudentWork : false,
	resource : {
		displayName : "Where the Wonders of Learning Never Cease | Wonderopolis",
		"@odata.type" : "#microsoft.graph.educationLinkResource",
		additionalData : {
			"link" : "https://wonderopolis.org/",
			thumbnailPreviewUrl : null,
		},
	},
};

const result = async () => {
	await graphServiceClient.education.classesById("educationClass-id").assignmentsById("educationAssignment-id").resources.post(requestBody);
}


```