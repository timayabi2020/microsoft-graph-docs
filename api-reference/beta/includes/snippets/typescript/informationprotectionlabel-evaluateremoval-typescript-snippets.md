---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const configuration = {
	headers : {
		"User-Agent": "ContosoLOBApp/1.0",
	}
};
const requestBody : EvaluateRemovalPostRequestBody = {
	contentInfo : {
		"@odata.type" : "#microsoft.graph.contentInfo",
		format : ContentFormat.Default,
		identifier : null,
		state : ContentState.Rest,
		metadata : [
			{
				"@odata.type" : "#microsoft.graph.keyValuePair",
				name : "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_Enabled",
				value : "True",
			},
			{
				"@odata.type" : "#microsoft.graph.keyValuePair",
				name : "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_Method",
				value : "Standard",
			},
			{
				"@odata.type" : "#microsoft.graph.keyValuePair",
				name : "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_SetDate",
				value : "1/1/0001 12:00:00 AM",
			},
			{
				"@odata.type" : "#microsoft.graph.keyValuePair",
				name : "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_SiteId",
				value : "cfa4cf1d-a337-4481-aa99-19d8f3d63f7c",
			},
			{
				"@odata.type" : "#microsoft.graph.keyValuePair",
				name : "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_Name",
				value : "General",
			},
			{
				"@odata.type" : "#microsoft.graph.keyValuePair",
				name : "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_ContentBits",
				value : "0",
			},
			{
				"@odata.type" : "#microsoft.graph.keyValuePair",
				name : "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_ActionId",
				value : "00000000-0000-0000-0000-000000000000",
			},
		],
		additionalData : {
			"format@odata.type" : "#microsoft.graph.contentFormat",
			"state@odata.type" : "#microsoft.graph.contentState",
			"metadata@odata.type" : "#Collection(microsoft.graph.keyValuePair)",
		},
	},
	downgradeJustification : {
		justificationMessage : "The information has been declassified.",
		isDowngradeJustified : true,
	},
};

const result = async () => {
	await graphServiceClient.informationProtection.policy.labels.evaluateRemoval.post(requestBody, configuration);
}


```