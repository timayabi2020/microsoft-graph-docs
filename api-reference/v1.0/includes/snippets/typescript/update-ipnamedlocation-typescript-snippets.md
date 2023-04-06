---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : NamedLocation = {
	"@odata.type" : "#microsoft.graph.ipNamedLocation",
	displayName : "Untrusted named location with only IPv4 address",
	additionalData : {
		isTrusted : false,
		ipRanges : [
			{
				"@odata.type" : "#microsoft.graph.iPv4CidrRange",
				cidrAddress : "6.5.4.3/18",
			},
		],
	},
};

const result = async () => {
	await graphServiceClient.identity.conditionalAccess.namedLocationsById("namedLocation-id").patch(requestBody);
}


```