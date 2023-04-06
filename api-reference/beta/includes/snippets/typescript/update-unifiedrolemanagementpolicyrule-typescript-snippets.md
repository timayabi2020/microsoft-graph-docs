---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : UnifiedRoleManagementPolicyRule = {
	"@odata.type" : "#microsoft.graph.unifiedRoleManagementPolicyExpirationRule",
	id : "Expiration_EndUser_Assignment",
	target : {
		"@odata.type" : "microsoft.graph.unifiedRoleManagementPolicyRuleTarget",
		caller : "EndUser",
		operations : [
			"All",
		],
		level : "Assignment",
		inheritableSettings : [
		],
		enforcedSettings : [
		],
	},
	additionalData : {
		isExpirationRequired : true,
		"maximumDuration" : "PT1H45M",
	},
};

const result = async () => {
	await graphServiceClient.policies.roleManagementPoliciesById("unifiedRoleManagementPolicy-id").rulesById("unifiedRoleManagementPolicyRule-id").patch(requestBody);
}


```