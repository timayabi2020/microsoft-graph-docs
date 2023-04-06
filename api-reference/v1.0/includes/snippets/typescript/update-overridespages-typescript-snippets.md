---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : $valuePutRequestBody = {
	additionalData : {
		LocalizedStrings : [
			{
				elementType : "UxElement",
				elementId : null,
				stringId : "alert_message",
				override : true,
				value : "Are you sure that you want to cancel entering your information?",
			},
		],
	},
};

const result = async () => {
	await graphServiceClient.identity.b2xUserFlowsById("b2xIdentityUserFlow-id").languagesById("userFlowLanguageConfiguration-id").overridesPagesById("userFlowLanguagePage-id").$value.put(requestBody);
}


```