---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : AssignPostRequestBody = {
	assignments : [
		{
			id : "b0c2d35f-3385-46c8-a6f5-6c3dfad7708b_64ff06de-9c00-4a5a-98b5-7f5abe26ffff",
			target : {
				"@odata.type" : "microsoft.graph.cloudPcManagementGroupAssignmentTarget",
				additionalData : {
					"groupId" : "64ff06de-9c00-4a5a-98b5-7f5abe26ffff",
				},
			},
		},
	],
	additionalData : {
		"@odata.type" : "#microsoft.graph.cloudPcProvisioningPolicyAssignment",
	},
};

const result = async () => {
	await graphServiceClient.deviceManagement.virtualEndpoint.provisioningPoliciesById("cloudPcProvisioningPolicy-id").assign.post(requestBody);
}


```