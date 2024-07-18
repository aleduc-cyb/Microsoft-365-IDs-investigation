# Microsoft-365-IDs-investigation
This repo aims to help cybersecurity professionals with numerous IDs found in Microsoft 365 logs.

## Office 365 Audit logs
### Common
- `Id`: unique identifier of an audit record.
- `OrganizationId`: unique identifier of the organization. Also referred to as TenantId.
- `ClientRequestId`: unique identifier of a cmdlet execution. Only used by Microsoft support.
- `SessionId`: unique identifier of the session used for actions in a specific Office 365 service. A session refers to a period of authenticated user activity that begins with authentication and ends with log out, expiration or admin termination.
- `AADSessionId`: unique identifier of an Entra authentication session. Consistent across various services that use the same authentication session. A session refers to a period of authenticated user activity that begins with authentication and ends with log out, expiration or admin termination.
- `UniqueTokenId`: unique identifier of the Entra token generated for access. Case-sensitive.

### Application
- `AppId`: unique identifier of the application or service that performed the action. Referred to as application ID in Entra (not object ID).
- `ClientAppId`: unique identifier of the client application. Referred to as application ID in Entra (not object ID).

### SharePoint/OneDrive
- `CorrelationID`: unique identifier of a request to SharePoint/OneDrive.
- `WebId`: unique identifier of the SharePoint/OneDrive website.

## Entra ID Audit logs


## References
- O365 Management Activity API Schema: https://learn.microsoft.com/en-us/office/office-365-management-api/office-365-management-activity-api-schema
