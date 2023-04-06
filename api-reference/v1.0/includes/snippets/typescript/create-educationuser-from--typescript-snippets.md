---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : EducationUser = {
	"@odata.type" : "#microsoft.graph.educationUser",
	primaryRole : EducationUserRole.String,
	middleName : "String",
	externalSource : EducationExternalSource.String,
	externalSourceDetail : "String",
	residenceAddress : {
		"@odata.type" : "microsoft.graph.physicalAddress",
	},
	mailingAddress : {
		"@odata.type" : "microsoft.graph.physicalAddress",
	},
	student : {
		"@odata.type" : "microsoft.graph.educationStudent",
	},
	teacher : {
		"@odata.type" : "microsoft.graph.educationTeacher",
	},
	createdBy : {
		"@odata.type" : "microsoft.graph.identitySet",
	},
	accountEnabled : boolean,
	assignedLicenses : [
		{
			"@odata.type" : "microsoft.graph.assignedLicense",
		},
	],
	assignedPlans : [
		{
			"@odata.type" : "microsoft.graph.assignedPlan",
		},
	],
	businessPhones : [
		"String",
	],
	department : "String",
	displayName : "String",
	givenName : "String",
	mail : "String",
	mailNickname : "String",
	mobilePhone : "String",
	passwordPolicies : "String",
	passwordProfile : {
		"@odata.type" : "microsoft.graph.passwordProfile",
	},
	officeLocation : "String",
	preferredLanguage : "String",
	provisionedPlans : [
		{
			"@odata.type" : "microsoft.graph.provisionedPlan",
		},
	],
	refreshTokensValidFromDateTime : new Date("String (timestamp)"),
	showInAddressList : boolean,
	surname : "String",
	usageLocation : "String",
	userPrincipalName : "String",
	userType : "String",
	onPremisesInfo : {
		"@odata.type" : "microsoft.graph.educationOnPremisesInfo",
	},
};

const result = async () => {
	await graphServiceClient.education.users.post(requestBody);
}


```