---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : Application = {
	tags : [
		"HR",
		"Payroll",
		"HideApp",
	],
	info : {
		logoUrl : "https://cdn.pixabay.com/photo/2016/03/21/23/25/link-1271843_1280.png",
		marketingUrl : "https://www.contoso.com/app/marketing",
		privacyStatementUrl : "https://www.contoso.com/app/privacy",
		supportUrl : "https://www.contoso.com/app/support",
		termsOfServiceUrl : "https://www.contoso.com/app/termsofservice",
	},
	web : {
		homePageUrl : "https://www.contoso.com/",
		logoutUrl : "https://www.contoso.com/frontchannel_logout",
		redirectUris : [
			"https://localhost",
		],
	},
	serviceManagementReference : "Owners aliases: Finance @ contosofinance@contoso.com; The Phone Company HR consulting @ hronsite@thephone-company.com;",
};

const result = async () => {
	await graphServiceClient.applicationsById("application-id").patch(requestBody);
}


```