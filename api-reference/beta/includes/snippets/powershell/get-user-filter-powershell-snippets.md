---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershell

Import-Module Microsoft.Graph.Beta.Users

Get-MgBetaUser -CountVariable CountVar -Consistencylevel "eventual" -Filter "endsWith(mail,'@contoso.com')" 

```