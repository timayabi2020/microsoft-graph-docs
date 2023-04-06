---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : NamedLocation = {
	"@odata.type" : "#microsoft.graph.countryNamedLocation",
	displayName : "Updated named location without unknown countries and regions",
	additionalData : {
		countriesAndRegions : [
			"CA",
			"IN",
		],
		includeUnknownCountriesAndRegions : false,
	},
};

const result = async () => {
	await graphServiceClient.identity.conditionalAccess.namedLocationsById("namedLocation-id").patch(requestBody);
}


```