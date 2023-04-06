---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : CloudPcOnPremisesConnection = {
	"@odata.type" : "#microsoft.graph.cloudPcOnPremisesConnection",
	displayName : "test-canary-02",
	type : CloudPcOnPremisesConnectionType.HybridAzureADJoin,
	subscriptionId : "0ac520ee-14c0-480f-b6c9-0a90c585ffff",
	subscriptionName : "CPC customer 001 test subscription",
	adDomainName : "contoso001.com",
	adDomainUsername : "dcadmin",
	organizationalUnit : "OU=Domain Controllers, DC=contoso001, DC=com",
	resourceGroupId : "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c585ad47/resourceGroups/CustomerRG",
	virtualNetworkId : "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c585ad47/resourceGroups/CustomerRG/providers/Microsoft.Network/virtualNetworks/canary01-MyVNET",
	subnetId : "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c585ad47/resourceGroups/CustomerRG/providers/Microsoft.Network/virtualNetworks/canary01-MyVNET/subnets/canary01-Subnet",
};

const result = async () => {
	await graphServiceClient.deviceManagement.virtualEndpoint.onPremisesConnections.post(requestBody);
}


```