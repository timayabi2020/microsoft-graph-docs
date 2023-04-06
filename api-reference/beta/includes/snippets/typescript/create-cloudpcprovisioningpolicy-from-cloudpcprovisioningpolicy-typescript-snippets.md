---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : CloudPcProvisioningPolicy = {
	"@odata.type" : "#microsoft.graph.cloudPcProvisioningPolicy",
	description : "Description value",
	displayName : "Display Name value",
	domainJoinConfiguration : {
		onPremisesConnectionId : "16ee6c71-fc10-438b-88ac-daa1ccafffff",
		additionalData : {
			"domainJoinType" : "hybridAzureADJoin",
		},
	},
	id : "1d164206-bf41-4fd2-8424-a3192d39ffff",
	imageDisplayName : "Windows-10 19h1-evd",
	imageId : "MicrosoftWindowsDesktop_Windows-10_19h1-evd",
	imageType : CloudPcProvisioningPolicyImageType.Gallery,
	onPremisesConnectionId : "4e47d0f6-6f77-44f0-8893-c0fe1701ffff",
	windowsSettings : {
		language : "en-US",
	},
};

const result = async () => {
	await graphServiceClient.deviceManagement.virtualEndpoint.provisioningPolicies.post(requestBody);
}


```