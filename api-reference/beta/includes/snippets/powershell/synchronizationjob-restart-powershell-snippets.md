---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershell

Import-Module Microsoft.Graph.Beta.Applications

$params = @{
	criteria = @{
		resetScope = "Watermark, Escrows, QuarantineState"
	}
}

Restart-MgBetaServicePrincipalsSynchronizationJob -ServicePrincipalId $servicePrincipalId -SynchronizationJobId $synchronizationJobId -BodyParameter $params

```