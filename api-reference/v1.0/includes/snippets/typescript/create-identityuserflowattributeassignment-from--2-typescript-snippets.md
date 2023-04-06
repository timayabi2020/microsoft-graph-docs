---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : IdentityUserFlowAttributeAssignment = {
	isOptional : false,
	requiresVerification : false,
	userInputType : IdentityUserFlowAttributeInputType.TextBox,
	displayName : "Shoe size",
	userAttributeValues : [
	],
	userAttribute : {
		id : "extension_guid_shoeSize",
	},
};

const result = async () => {
	await graphServiceClient.identity.b2xUserFlowsById("b2xIdentityUserFlow-id").userAttributeAssignments.post(requestBody);
}


```