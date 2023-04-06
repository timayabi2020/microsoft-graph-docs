---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : TenantAppManagementPolicy = {
	isEnabled : true,
	applicationRestrictions : {
		passwordCredentials : [
			{
				restrictionType : AppCredentialRestrictionType.PasswordAddition,
				maxLifetime : null,
				restrictForAppsCreatedAfterDateTime : new Date("2021-01-01T10:37:00Z"),
			},
			{
				restrictionType : AppCredentialRestrictionType.PasswordLifetime,
				maxLifetime : p4DT12H30M5S,
				restrictForAppsCreatedAfterDateTime : new Date("2017-01-01T10:37:00Z"),
			},
			{
				restrictionType : AppCredentialRestrictionType.SymmetricKeyAddition,
				maxLifetime : null,
				restrictForAppsCreatedAfterDateTime : new Date("2021-01-01T10:37:00Z"),
			},
			{
				restrictionType : AppCredentialRestrictionType.CustomPasswordAddition,
				maxLifetime : null,
				restrictForAppsCreatedAfterDateTime : new Date("2015-01-01T10:37:00Z"),
			},
			{
				restrictionType : AppCredentialRestrictionType.SymmetricKeyLifetime,
				maxLifetime : p40D,
				restrictForAppsCreatedAfterDateTime : new Date("2015-01-01T10:37:00Z"),
			},
		],
		keyCredentials : [
			{
				restrictionType : AppKeyCredentialRestrictionType.AsymmetricKeyLifetime,
				maxLifetime : p30D,
				restrictForAppsCreatedAfterDateTime : new Date("2015-01-01T10:37:00Z"),
			},
		],
	},
};

const result = async () => {
	await graphServiceClient.policies.defaultAppManagementPolicy.patch(requestBody);
}


```