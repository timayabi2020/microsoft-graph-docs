---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : ChangeDeploymentStatusPostRequestBody = {
	tenantGroupId : "String",
	tenantId : "String",
	managementActionId : "String",
	managementTemplateId : "String",
	status : "String",
};

const result = async () => {
	await graphServiceClient.tenantRelationships.managedTenants.managementActionTenantDeploymentStatuses.managedTenantsChangeDeploymentStatus.post(requestBody);
}


```