---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershell

Import-Module Microsoft.Graph.Beta.WindowsUpdates

$params = @{
	"@odata.type" = "#microsoft.graph.windowsUpdates.deployment"
	content = @{
		"@odata.type" = "microsoft.graph.windowsUpdates.featureUpdateReference"
		version = "20H2"
	}
	settings = @{
		"@odata.type" = "microsoft.graph.windowsUpdates.windowsDeploymentSettings"
		monitoring = @{
			monitoringRules = @(
				@{
					"@odata.type" = "#microsoft.graph.windowsUpdates.monitoringRule"
					signal = "rollback"
					threshold = 5
					action = "pauseDeployment"
				}
			)
		}
	}
}

New-MgBetaWindowsUpdatesDeployment -BodyParameter $params

```