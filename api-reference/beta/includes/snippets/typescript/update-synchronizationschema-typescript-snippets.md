---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : SchemaPutRequestBody = {
	additionalData : {
		directories : [
			{
				name : "Azure Active Directory",
				objects : [
					{
						name : "User",
						attributes : [
							{
								name : "userPrincipalName",
								type : "string",
							},
						],
					},
				],
			},
			{
				name : "Salesforce",
			},
		],
		synchronizationRules : [
			{
				name : "USER_TO_USER",
				sourceDirectoryName : "Azure Active Directory",
				targetDirectoryName : "Salesforce",
				objectMappings : [
					{
						sourceObjectName : "User",
						targetObjectName : "User",
						attributeMappings : [
							{
								source : {
								},
								targetAttributeName : "userName",
							},
						],
					},
				],
			},
		],
	},
};

async () => {
	await graphServiceClient.servicePrincipalsById("servicePrincipal-id").synchronization.jobsById("synchronizationJob-id").schema.put(requestBody);
}


```