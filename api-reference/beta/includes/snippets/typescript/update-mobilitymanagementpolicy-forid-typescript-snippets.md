---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : MobilityManagementPolicy = {
	"@odata.type" : "#microsoft.graph.mobilityManagementPolicy",
	complianceUrl : "https://portal.uem.contoso.com/?portalAction=Compliance",
	discoveryUrl : "https://enrollment.uem.contoso.com/enrollmentserver/discovery.svc",
	termsOfUseUrl : "https://portal.uem.contoso.com/TermsofUse.aspx",
};

const result = async () => {
	await graphServiceClient.policies.mobileDeviceManagementPoliciesById("mobilityManagementPolicy-id").patch(requestBody);
}


```