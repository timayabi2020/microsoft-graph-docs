---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : OnPremisesDirectorySynchronization = {
	configuration : {
		accidentalDeletionPrevention : {
			synchronizationPreventionType : OnPremisesDirectorySynchronizationDeletionPreventionType.EnabledForCount,
			alertThreshold : 500,
		},
		synchronizationInterval : pT30M,
		customerRequestedSynchronizationInterval : pT1H,
	},
	features : {
		groupWriteBackEnabled : true,
	},
};

const result = async () => {
	await graphServiceClient.directory.onPremisesSynchronizationById("onPremisesDirectorySynchronization-id").patch(requestBody);
}


```