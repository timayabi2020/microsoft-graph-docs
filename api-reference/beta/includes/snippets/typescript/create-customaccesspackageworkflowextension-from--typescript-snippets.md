---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : CustomAccessPackageWorkflowExtension = {
	displayName : "test_action_0124",
	description : "this is for graph testing only",
	endpointConfiguration : {
		"@odata.type" : "#microsoft.graph.logicAppTriggerEndpointConfiguration",
		additionalData : {
			"subscriptionId" : "38ab2ccc-3747-4567-b36b-9478f5602f0d",
			"resourceGroupName" : "EMLogicApp",
			"logicAppWorkflowName" : "customextension_test",
		},
	},
	authenticationConfiguration : {
		"@odata.type" : "#microsoft.graph.azureAdTokenAuthentication",
		additionalData : {
			"resourceId" : "f604bd15-f785-4309-ad7c-6fad18ddb6cb",
		},
	},
};

const result = async () => {
	await graphServiceClient.identityGovernance.entitlementManagement.accessPackageCatalogsById("accessPackageCatalog-id").customAccessPackageWorkflowExtensions.post(requestBody);
}


```