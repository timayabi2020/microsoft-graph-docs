---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : CloudPcProvisioningPolicy = {
	"@odata.type" : "#microsoft.graph.cloudPcProvisioningPolicy",
	displayName : "HR provisioning policy",
	description : "Provisioning policy for India HR employees",
	onPremisesConnectionId : "4e47d0f6-6f77-44f0-8893-c0fe1701ffff",
	imageId : "Image ID value",
	imageDisplayName : "Image Display Name value",
	imageType : CloudPcProvisioningPolicyImageType.Custom,
	windowsSettings : {
		language : "en-US",
	},
};

const result = async () => {
	await graphServiceClient.deviceManagement.virtualEndpoint.provisioningPoliciesById("cloudPcProvisioningPolicy-id").patch(requestBody);
}


```