---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : AdministrativeUnit = {
	additionalData : {
		"membershipType" : "Dynamic",
		"membershipRule" : "(user.country -eq \"United States\")",
		"membershipRuleProcessingState" : "On",
	},
};

const result = async () => {
	await graphServiceClient.administrativeUnitsById("administrativeUnit-id").patch(requestBody);
}


```