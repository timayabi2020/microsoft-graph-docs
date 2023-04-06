---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : Place = {
	"@odata.type" : "microsoft.graph.roomList",
	displayName : "Building 1",
	phone : "555-555-0100",
	address : {
		street : "4567 Main Street",
		city : "Buffalo",
		state : "NY",
		postalCode : "98052",
		countryOrRegion : "USA",
	},
	geoCoordinates : {
		altitude : null,
		latitude : 47,
		longitude : -122,
		accuracy : null,
		altitudeAccuracy : null,
	},
};

const result = async () => {
	await graphServiceClient.placesById("place-id").patch(requestBody);
}


```