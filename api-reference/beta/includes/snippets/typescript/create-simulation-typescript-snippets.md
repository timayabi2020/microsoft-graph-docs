---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : Simulation = {
	displayName : "Graph Simulation",
	payloadDeliveryPlatform : PayloadDeliveryPlatform.Email,
	durationInDays : 7,
	attackTechnique : SimulationAttackTechnique.CredentialHarvesting,
	attackType : SimulationAttackType.Social,
	status : SimulationStatus.Scheduled,
	completionDateTime : new Date("2022-09-16T06:13:08.4297612Z"),
	launchDateTime : new Date("2022-09-05T06:13:08.4297612Z"),
	includedAccountTarget : {
		"@odata.type" : "#microsoft.graph.addressBookAccountTargetContent",
		type : AccountTargetContentType.AddressBook,
		additionalData : {
			accountTargetEmails : [
				"john@contoso.com",
			],
		},
	},
	additionalData : {
		"payload@odata.bind" : "https://graph.microsoft.com/beta/security/attacksimulation/payloads/12345678-9abc-def0-123456789a",
	},
};

const result = async () => {
	await graphServiceClient.security.attackSimulation.simulations.post(requestBody);
}


```