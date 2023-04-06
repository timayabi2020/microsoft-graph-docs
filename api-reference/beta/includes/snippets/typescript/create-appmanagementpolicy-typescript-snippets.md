---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : AppManagementPolicy = {
	displayName : "Credential management policy",
	description : "Cred policy sample",
	isEnabled : true,
	restrictions : {
		passwordCredentials : [
			{
				restrictionType : AppCredentialRestrictionType.PasswordAddition,
				maxLifetime : null,
				restrictForAppsCreatedAfterDateTime : new Date("2019-10-19T10:37:00Z"),
			},
			{
				restrictionType : AppCredentialRestrictionType.PasswordLifetime,
				maxLifetime : p4DT12H30M5S,
				restrictForAppsCreatedAfterDateTime : new Date("2014-10-19T10:37:00Z"),
			},
			{
				restrictionType : AppCredentialRestrictionType.SymmetricKeyAddition,
				maxLifetime : null,
				restrictForAppsCreatedAfterDateTime : new Date("2019-10-19T10:37:00Z"),
			},
			{
				restrictionType : AppCredentialRestrictionType.SymmetricKeyLifetime,
				maxLifetime : p4D,
				restrictForAppsCreatedAfterDateTime : new Date("2014-10-19T10:37:00Z"),
			},
		],
		keyCredentials : [
			{
				restrictionType : AppKeyCredentialRestrictionType.AsymmetricKeyLifetime,
				maxLifetime : p90D,
				restrictForAppsCreatedAfterDateTime : new Date("2014-10-19T10:37:00Z"),
			},
		],
	},
};

const result = async () => {
	await graphServiceClient.policies.appManagementPolicies.post(requestBody);
}


```