---
title: "Manage an Azure AD application using Microsoft Graph"
description: "Learn how to use the applications and service principals APIs in Microsoft Graph to manage your applications."
author: "FaithOmbongi"
ms.author: ombongifaith
ms.reviewer: sureshja
ms.localizationpriority: medium
ms.topic: how-to
ms.prod: "applications"
ms.date: 12/08/2022
---

# Manage an Azure AD application using Microsoft Graph

Your app must be registered in Azure AD before the Microsoft identity platform can authorize it to access data stored in Azure Active Directory (Azure AD) or Microsoft 365 tenants. This condition applies to apps that you develop yourself, that are owned by your organization, or that you access through an active subscription.

Many settings for apps are recorded as objects that can be accessed, updated, or deleted using Microsoft Graph. In this article, you'll learn how to use Microsoft Graph to manage app and service principal objects including the properties, permissions, and role assignments.

## Prerequisites

To complete this tutorial, you need the following resources and privileges:

+ A working Azure AD tenant.
+ Sign in to [Graph Explorer](https://aka.ms/ge) as a user in an _Application Administrator_ role or a user allowed to create and manage applications in the tenant.

## Register an application with Azure AD

### Request

Least privilege delegated permission: `Application.ReadWrite.All`

# [HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "tutorial-application-basics-create-app"
}-->
```msgraph-interactive
POST https://graph.microsoft.com/v1.0/applications
Content-type: application/json

{
  "displayName": "My application"
}
```

# [PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/tutorial-application-basics-create-app-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [TypeScript](#tab/typescript)
[!INCLUDE [sample-code](../includes/snippets/typescript/tutorial-application-basics-create-app-typescript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [Cli](#tab/cli)
[!INCLUDE [sample-code](../includes/snippets/cli/tutorial-application-basics-create-app-cli-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### Response

The following code is an example of the default response that includes all the properties returned by default. The application is assigned an ID that's globally unique in the Azure AD ecosystem.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#applications/$entity",
    "id": "0d0021e2-eaab-4b9f-a5ad-38c55337d63e",
    "deletedDateTime": null,
    "appId": "5f0f8757-988d-474c-9f85-74a6bc70dfd0",
    "applicationTemplateId": null,
    "disabledByMicrosoftStatus": null,
    "createdDateTime": "2022-02-08T08:58:36.7669085Z",
    "displayName": "My application",
    "description": null,
    "groupMembershipClaims": null,
    "identifierUris": [],
    "isDeviceOnlyAuthSupported": null,
    "isFallbackPublicClient": null,
    "notes": null,
    "publisherDomain": "M365x010717.onmicrosoft.com",
    "serviceManagementReference": null,
    "signInAudience": "AzureADandPersonalMicrosoftAccount",
    "tags": [],
    "tokenEncryptionKeyId": null,
    "defaultRedirectUri": null,
    "certification": null,
    "optionalClaims": null,
    "addIns": [],
    "api": {
        "acceptMappedClaims": null,
        "knownClientApplications": [],
        "requestedAccessTokenVersion": 2,
        "oauth2PermissionScopes": [],
        "preAuthorizedApplications": []
    },
    "appRoles": [],
    "info": {
        "logoUrl": null,
        "marketingUrl": null,
        "privacyStatementUrl": null,
        "supportUrl": null,
        "termsOfServiceUrl": null
    },
    "keyCredentials": [],
    "parentalControlSettings": {
        "countriesBlockedForMinors": [],
        "legalAgeGroupRule": "Allow"
    },
    "passwordCredentials": [],
    "publicClient": {
        "redirectUris": []
    },
    "requiredResourceAccess": [],
    "verifiedPublisher": {
        "displayName": null,
        "verifiedPublisherId": null,
        "addedDateTime": null
    },
    "web": {
        "homePageUrl": null,
        "logoutUrl": null,
        "redirectUris": [],
        "implicitGrantSettings": {
            "enableAccessTokenIssuance": false,
            "enableIdTokenIssuance": false
        }
    },
    "spa": {
        "redirectUris": []
    }
}
```

The **signInAudience** property is assigned a default value of `AzureADandPersonalMicrosoftAccount`. This configuration allows any user who is signed in with any account type, including Azure AD accounts, personal Microsoft accounts, and social media credentials, can use your app. You can change the **signInAudience** to a different scope.

If you created the application as a user with administrator privileges, you were automatically assigned ownership to the application. You can confirm ownership by retrieving the owners navigation property through `GET https://graph.microsoft.com/v1.0/applications/0d0021e2-eaab-4b9f-a5ad-38c55337d63e/owners`. You can also assign another user or app ownership of the application.

## Configure other basic properties for your app

Least privilege delegated permission: `Application.ReadWrite.All`

You'll configure the following basic properties for the app.

+ Add tags for categorization in the organization. Also, use the `HideApp` tag to hide the app from My Apps and the Microsoft 365 Launcher.
+ Add basic information including the logo, terms of service, and privacy statement.
+ Store contact information about the application

# [HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "tutorial-application-basics-update-app"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/applications/0d0021e2-eaab-4b9f-a5ad-38c55337d63e/
Content-type: application/json

{
    "tags": [
        "HR",
        "Payroll",
        "HideApp"
    ],
    "info": {
        "logoUrl": "https://cdn.pixabay.com/photo/2016/03/21/23/25/link-1271843_1280.png",
        "marketingUrl": "https://www.contoso.com/app/marketing",
        "privacyStatementUrl": "https://www.contoso.com/app/privacy",
        "supportUrl": "https://www.contoso.com/app/support",
        "termsOfServiceUrl": "https://www.contoso.com/app/termsofservice"
    },
    "web": {
        "homePageUrl": "https://www.contoso.com/",
        "logoutUrl": "https://www.contoso.com/frontchannel_logout",
        "redirectUris": [
            "https://localhost"
        ]
    },
    "serviceManagementReference": "Owners aliases: Finance @ contosofinance@contoso.com; The Phone Company HR consulting @ hronsite@thephone-company.com;"
}
```

# [PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/tutorial-application-basics-update-app-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [TypeScript](#tab/typescript)
[!INCLUDE [sample-code](../includes/snippets/typescript/tutorial-application-basics-update-app-typescript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [Cli](#tab/cli)
[!INCLUDE [sample-code](../includes/snippets/cli/tutorial-application-basics-update-app-cli-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

## Limit app sign-in to only assigned identities

Least privilege delegated permission: `Application.ReadWrite.All`

<!-- {
  "blockType": "request",
  "name": "tutorial-application-basics-grant-approleassignmentrequired"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/servicePrincipals/89473e09-0737-41a1-a0c3-1418d6908bcd
{
    "appRoleAssignmentRequired": true
}
```



### Assign an owner to an app

Least privilege delegated permission: `Application.ReadWrite.All`

In the following request, `8afc02cb-4d62-4dba-b536-9f6d73e9be26` is the object ID for a user or service principal.


# [HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "tutorial-application-basics-assign-app-owner"
}-->
```http
POST https://graph.microsoft.com/v1.0/applications/7b45cf6d-9083-4eb2-92c4-a7e090f1fc40/owners/$ref
Content-Type: application/json

{
    "@odata.id": "https://graph.microsoft.com/v1.0/directoryObjects/8afc02cb-4d62-4dba-b536-9f6d73e9be26"
}
```

# [PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/tutorial-application-basics-assign-app-owner-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [TypeScript](#tab/typescript)
[!INCLUDE [sample-code](../includes/snippets/typescript/tutorial-application-basics-assign-app-owner-typescript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [Cli](#tab/cli)
[!INCLUDE [sample-code](../includes/snippets/cli/tutorial-application-basics-assign-app-owner-cli-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### Assign an owner to a service principal

Least privilege delegated permission: `Application.ReadWrite.All`

The following request references the service principal using its **appId**. `8afc02cb-4d62-4dba-b536-9f6d73e9be26` is the object ID for a user or service principal.


<!-- {
  "blockType": "request",
  "name": "tutorial-application-basics-assign-serviceprincipal-owner"
}-->
```http
POST https://graph.microsoft.com/v1.0/servicePrincipals(appId='46e6adf4-a9cf-4b60-9390-0ba6fb00bf6b')/owners/$ref
Content-Type: application/json

{
    "@odata.id": "https://graph.microsoft.com/v1.0/directoryObjects/8afc02cb-4d62-4dba-b536-9f6d73e9be26"
}
```

## See also

+ [Properties of an enterprise application (service principal)](/azure/active-directory/manage-apps/application-properties)
+ [Add a certificate to an app using Microsoft Graph](/graph/applications-how-to-add-certificate)
