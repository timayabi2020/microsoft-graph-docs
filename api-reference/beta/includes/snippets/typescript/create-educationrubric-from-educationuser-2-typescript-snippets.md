---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : EducationRubric = {
	displayName : "Example Points Rubric",
	description : {
		content : "This is an example of a rubric with points",
		contentType : BodyType.Text,
	},
	levels : [
		{
			displayName : "Good",
			description : {
				content : "",
				contentType : BodyType.Text,
			},
			grading : {
				"@odata.type" : "#microsoft.graph.educationAssignmentPointsGradeType",
				additionalData : {
					maxPoints : 2,
				},
			},
		},
		{
			displayName : "Poor",
			description : {
				content : "",
				contentType : BodyType.Text,
			},
			grading : {
				"@odata.type" : "#microsoft.graph.educationAssignmentPointsGradeType",
				additionalData : {
					maxPoints : 1,
				},
			},
		},
	],
	qualities : [
		{
			description : {
				content : "Argument",
				contentType : BodyType.Text,
			},
			criteria : [
				{
					description : {
						content : "The essay's argument is persuasive.",
						contentType : BodyType.Text,
					},
				},
				{
					description : {
						content : "The essay's argument does not make sense.",
						contentType : BodyType.Text,
					},
				},
			],
			weight : 50.0,
		},
		{
			description : {
				content : "Spelling and Grammar",
				contentType : BodyType.Text,
			},
			criteria : [
				{
					description : {
						content : "The essay uses proper spelling and grammar with few or no errors.",
						contentType : BodyType.Text,
					},
				},
				{
					description : {
						content : "The essay has numerous errors in spelling and/or grammar.",
						contentType : BodyType.Text,
					},
				},
			],
			weight : 50.0,
		},
	],
	grading : {
		"@odata.type" : "#microsoft.graph.educationAssignmentPointsGradeType",
	},
};

const result = async () => {
	await graphServiceClient.education.me.rubrics.post(requestBody);
}


```