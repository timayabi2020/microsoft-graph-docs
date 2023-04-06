---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : TenantCustomizedInformation = {
	"@odata.type" : "#microsoft.graph.managedTenants.tenantCustomizedInformation",
	tenantId : "String",
	contacts : [
		{
			"@odata.type" : "microsoft.graph.managedTenants.tenantContactInformation",
			name : "String",
			title : "String",
			email : "String",
			phone : "String",
			notes : "String",
		},
	],
	website : "String",
};

const result = async () => {
	await graphServiceClient.tenantRelationships.managedTenants.tenantsCustomizedInformationById("tenantCustomizedInformation-id").patch(requestBody);
}


```