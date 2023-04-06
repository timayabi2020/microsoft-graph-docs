---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : Organization = {
	marketingNotificationEmails : [
		"marketing@contoso.com",
	],
	privacyProfile : {
		contactEmail : "alice@contoso.com",
		statementUrl : "https://contoso.com/privacyStatement",
	},
	securityComplianceNotificationMails : [
		"security@contoso.com",
	],
	securityComplianceNotificationPhones : [
		"(123) 456-7890",
	],
	technicalNotificationMails : [
		"tech@contoso.com",
	],
};

const result = async () => {
	await graphServiceClient.organizationById("organization-id").patch(requestBody);
}


```