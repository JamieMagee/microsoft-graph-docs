---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var authenticationMethodConfiguration = await graphClient.Policies.AuthenticationMethodsPolicy.AuthenticationMethodConfigurations["microsoftAuthenticator"]
	.Request()
	.GetAsync();

```