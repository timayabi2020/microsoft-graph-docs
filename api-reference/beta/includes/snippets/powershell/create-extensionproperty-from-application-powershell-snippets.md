---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershell

Import-Module Microsoft.Graph.Beta.Applications

$params = @{
	name = "jobGroup"
	dataType = "String"
	targetObjects = @(
		"User"
	)
}

New-MgBetaApplicationExtensionProperty -ApplicationId $applicationId -BodyParameter $params

```