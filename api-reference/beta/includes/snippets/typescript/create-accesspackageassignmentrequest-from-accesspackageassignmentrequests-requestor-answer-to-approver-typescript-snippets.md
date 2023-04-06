---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : AccessPackageAssignmentRequest = {
	requestType : "UserAdd",
	accessPackageAssignment : {
		targetId : "46184453-e63b-4f20-86c2-c557ed5d5df9",
		assignmentPolicyId : "2264bf65-76ba-417b-a27d-54d291f0cbc8",
		accessPackageId : "a914b616-e04e-476b-aa37-91038f0b165b",
	},
	answers : [
		{
			"@odata.type" : "#microsoft.graph.accessPackageAnswerString",
			answeredQuestion : {
				"@odata.type" : "#microsoft.graph.accessPackageMultipleChoiceQuestion",
				id : "A714EC6F-4EE0-4614-BD81-37E0C5ECBBFF",
			},
			additionalData : {
				"value" : "Arizona",
			},
		},
		{
			"@odata.type" : "#microsoft.graph.accessPackageAnswerString",
			answeredQuestion : {
				"@odata.type" : "#microsoft.graph.accessPackageTextInputQuestion",
				id : "AA615EE9-D9D8-4C03-BE91-BEE37106DEDA",
			},
			additionalData : {
				"value" : "Need access to marketing campaign material",
			},
		},
	],
};

const result = async () => {
	await graphServiceClient.identityGovernance.entitlementManagement.accessPackageAssignmentRequests.post(requestBody);
}


```