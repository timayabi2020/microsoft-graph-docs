---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : CustomTaskExtension = {
	displayName : "Grant manager access to mailbox and OneDrive",
	description : "Grant manager access to mailbox and OneDrive",
	endpointConfiguration : {
		"@odata.type" : "#microsoft.graph.logicAppTriggerEndpointConfiguration",
		additionalData : {
			"subscriptionId" : "c500b67c-e9b7-4ad2-a90d-77d41385ae55",
			"resourceGroupName" : "RG-LCM",
			"logicAppWorkflowName" : "ManagerAccess",
		},
	},
	authenticationConfiguration : {
		"@odata.type" : "#microsoft.graph.azureAdTokenAuthentication",
		additionalData : {
			"resourceId" : "542dc01a-0b5d-4edc-b3f9-5cfe6393f557",
		},
	},
	clientConfiguration : {
		"@odata.type" : "#microsoft.graph.customExtensionClientConfiguration",
		timeoutInMilliseconds : 1000,
		additionalData : {
			maximumRetries : 1,
		},
	},
	callbackConfiguration : {
		"@odata.type" : "#microsoft.graph.identityGovernance.customTaskExtensionCallbackConfiguration",
		timeoutDuration : pT20M,
	},
};

const result = async () => {
	await graphServiceClient.identityGovernance.lifecycleWorkflows.customTaskExtensionsById("customTaskExtension-id").patch(requestBody);
}


```