---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workforceIntegrations = new WorkforceIntegration
{
	DisplayName = "displayName-value",
	ApiVersion = 99,
	Encryption = new WorkforceIntegrationEncryption
	{
		Protocol = WorkforceIntegrationEncryptionProtocol.SharedSecret,
		Secret = "secret-value"
	},
	IsActive = true,
	Url = "url-value",
	SupportedEntities = WorkforceIntegrationSupportedEntities.None
};

await graphClient.Teamwork.WorkforceIntegrations
	.Request()
	.UpdateAsync(workforceIntegrations);

```