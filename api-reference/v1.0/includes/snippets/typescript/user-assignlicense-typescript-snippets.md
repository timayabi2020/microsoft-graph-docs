---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : AssignLicensePostRequestBody = {
	addLicenses : [
		{
			disabledPlans : [
				"11b0131d-43c8-4bbb-b2c8-e80f9a50834a",
			],
			skuId : "45715bb8-13f9-4bf6-927f-ef96c102d394",
		},
	],
	removeLicenses : [
		"bea13e0c-3828-4daa-a392-28af7ff61a0f",
	],
};

const result = async () => {
	await graphServiceClient.me.assignLicense.post(requestBody);
}


```