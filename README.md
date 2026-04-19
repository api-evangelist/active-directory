# Microsoft Active Directory (active-directory)
Microsoft Active Directory and Microsoft Entra ID provide identity and access management for organizations of all sizes. Microsoft Graph API is the unified REST API gateway for accessing and managing Microsoft Entra ID (formerly Azure Active Directory), including users, groups, applications, devices, conditional access policies, identity governance, and directory administration. The Microsoft Graph API enables IT administrators, identity engineers, and security teams to automate user lifecycle management, enforce zero trust policies, and integrate identity data into security operations.

**URL:** [Visit APIs.json](https://raw.githubusercontent.com/api-evangelist/active-directory/refs/heads/main/apis.yml)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags:

 - Active Directory, Authentication, Authorization, Directory Services, Identity Management, Microsoft Entra, Zero Trust

## Timestamps

- **Created:** 2024-01-01
- **Modified:** 2026-04-19

## APIs

### Microsoft Graph Users API
Manage the entire lifecycle of users in Microsoft Entra ID, including creating, reading, updating, and deleting user accounts, managing licenses, group memberships, authentication methods, and profile photos. Supports both v1.0 and beta endpoints.

**Human URL:** [https://learn.microsoft.com/en-us/graph/api/resources/users](https://learn.microsoft.com/en-us/graph/api/resources/users)

#### Tags:

 - Directory Services, Identity Management, Users

#### Properties

- [Documentation](https://learn.microsoft.com/en-us/graph/api/resources/users)
- [OpenAPI](openapi/active-directory-users-openapi.yaml)
- [JSONSchema](json-schema/users-user-schema.json)
- [JSONSchema](json-schema/users-password-profile-schema.json)
- [JSONStructure](json-structure/users-user-structure.json)
- [Example](examples/users-user-example.json)
- [NaftikoCapability](capabilities/shared/active-directory-users.yaml)

---

### Microsoft Graph Groups API
Create and manage Microsoft Entra security groups, Microsoft 365 groups, and distribution lists. Manage group memberships, owners, and settings. Groups enable efficient entitlement management for users, licensing, and resource access.

**Human URL:** [https://learn.microsoft.com/en-us/graph/api/resources/groups-overview](https://learn.microsoft.com/en-us/graph/api/resources/groups-overview)

#### Tags:

 - Directory Services, Groups, Identity Management

#### Properties

- [Documentation](https://learn.microsoft.com/en-us/graph/api/resources/groups-overview)
- [OpenAPI](openapi/active-directory-groups-openapi.yaml)
- [JSONSchema](json-schema/groups-group-schema.json)
- [JSONStructure](json-structure/groups-group-structure.json)
- [Example](examples/groups-group-example.json)
- [NaftikoCapability](capabilities/shared/active-directory-groups.yaml)

---

### Microsoft Graph Applications and Service Principals API
Register and manage Microsoft Entra applications and their associated service principals programmatically. Configure app permissions, OAuth2 permission grants, app role assignments, certificates, federated identity credentials, and app consent policies.

**Human URL:** [https://learn.microsoft.com/en-us/graph/api/resources/applications-api-overview](https://learn.microsoft.com/en-us/graph/api/resources/applications-api-overview)

#### Tags:

 - Applications, Identity Management, OAuth2, Service Principals

#### Properties

- [Documentation](https://learn.microsoft.com/en-us/graph/api/resources/applications-api-overview)
- [OpenAPI](openapi/active-directory-applications-openapi.yaml)
- [JSONSchema](json-schema/applications-application-schema.json)
- [JSONSchema](json-schema/applications-service-principal-schema.json)
- [JSONStructure](json-structure/applications-application-structure.json)
- [Example](examples/applications-application-example.json)
- [NaftikoCapability](capabilities/shared/active-directory-applications.yaml)

---

### Microsoft Graph Devices API
Manage devices registered or joined to Microsoft Entra ID, including Entra joined, Entra registered, and hybrid Azure AD joined devices. Retrieve BitLocker recovery keys and Local Admin Password Solution (LAPS) credentials for managed devices.

**Human URL:** [https://learn.microsoft.com/en-us/graph/api/resources/device](https://learn.microsoft.com/en-us/graph/api/resources/device)

#### Tags:

 - Devices, Endpoint Management, Identity Management

#### Properties

- [Documentation](https://learn.microsoft.com/en-us/graph/api/resources/device)

---

### Microsoft Graph Directory Roles and Administrative Units API
Manage Microsoft Entra built-in and custom directory roles, role assignments, and role-scoped administrative units. Assign administrator roles to users, groups, or service principals, and create scoped role assignments via administrative units.

**Human URL:** [https://learn.microsoft.com/en-us/graph/api/resources/directoryrole](https://learn.microsoft.com/en-us/graph/api/resources/directoryrole)

#### Tags:

 - Authorization, Directory Services, Role Management

#### Properties

- [Documentation](https://learn.microsoft.com/en-us/graph/api/resources/directoryrole)

---

### Microsoft Graph Conditional Access API
Create and manage Microsoft Entra Conditional Access policies that enforce access controls based on user, location, device, and risk signals. Configure named locations, authentication context class references, and evaluate policy impact using what-if analysis.

**Human URL:** [https://learn.microsoft.com/en-us/graph/api/resources/conditionalaccesspolicy](https://learn.microsoft.com/en-us/graph/api/resources/conditionalaccesspolicy)

#### Tags:

 - Authorization, Conditional Access, Security, Zero Trust

#### Properties

- [Documentation](https://learn.microsoft.com/en-us/graph/api/resources/conditionalaccesspolicy)

---

### Microsoft Graph Identity Governance API
Manage Microsoft Entra ID Governance features including access reviews, entitlement management (access packages, catalogs, and policies), Privileged Identity Management (PIM) for just-in-time role activation, and lifecycle workflows for joiner/mover/leaver employee identity lifecycle automation.

**Human URL:** [https://learn.microsoft.com/en-us/graph/api/resources/identitygovernance-overview](https://learn.microsoft.com/en-us/graph/api/resources/identitygovernance-overview)

#### Tags:

 - Governance, Identity Management, Lifecycle Management, Privileged Identity Management

#### Properties

- [Documentation](https://learn.microsoft.com/en-us/graph/api/resources/identitygovernance-overview)

---

### Microsoft Graph Identity Protection API
Detect, investigate, and remediate identity-based risks using Microsoft Entra ID Protection. Access risk detections, risky users, risky service principals, and risk events, and feed data into SIEM tools for security correlation and incident response.

**Human URL:** [https://learn.microsoft.com/en-us/graph/api/resources/identityprotection-overview](https://learn.microsoft.com/en-us/graph/api/resources/identityprotection-overview)

#### Tags:

 - Identity Protection, Risk Management, Security

#### Properties

- [Documentation](https://learn.microsoft.com/en-us/graph/api/resources/identityprotection-overview)

---

### Microsoft Graph Authentication Methods API
Manage authentication methods registered for users in Microsoft Entra ID, including FIDO2 security keys, Microsoft Authenticator, phone (SMS/voice call), email OTP, Windows Hello for Business, and temporary access passes. Configure authentication method policies and authentication strength requirements.

**Human URL:** [https://learn.microsoft.com/en-us/graph/api/resources/authenticationmethods-overview](https://learn.microsoft.com/en-us/graph/api/resources/authenticationmethods-overview)

#### Tags:

 - Authentication, MFA, Passwordless, Security

#### Properties

- [Documentation](https://learn.microsoft.com/en-us/graph/api/resources/authenticationmethods-overview)

---

### Microsoft Graph Identity and Access Reports API
Access audit logs, sign-in logs, provisioning logs, and identity-related reports for monitoring, compliance, and troubleshooting. Stream logs to Azure Monitor and Log Analytics or to third-party SIEM tools for security operations.

**Human URL:** [https://learn.microsoft.com/en-us/graph/api/resources/report-identity-access](https://learn.microsoft.com/en-us/graph/api/resources/report-identity-access)

#### Tags:

 - Audit Logs, Compliance, Monitoring, Reports

#### Properties

- [Documentation](https://learn.microsoft.com/en-us/graph/api/resources/report-identity-access)

## Common Properties

- [Portal](https://developer.microsoft.com/en-us/graph)
- [GettingStarted](https://learn.microsoft.com/en-us/graph/get-started)
- [Documentation](https://learn.microsoft.com/en-us/graph/overview)
- [Authentication](https://learn.microsoft.com/en-us/graph/auth/auth-concepts)
- [APIReference](https://learn.microsoft.com/en-us/graph/api/overview)
- [RateLimits](https://learn.microsoft.com/en-us/graph/throttling)
- [SDK](https://learn.microsoft.com/en-us/graph/sdks/sdks-overview)
- [CLI](https://learn.microsoft.com/en-us/cli/azure/ad)
- [Blog](https://devblogs.microsoft.com/microsoft365dev/)
- [StatusPage](https://azure.status.microsoft.com/)
- [Support](https://developer.microsoft.com/en-us/graph/support)
- [TermsOfService](https://learn.microsoft.com/en-us/legal/microsoft-apis/terms-of-use)
- [PrivacyPolicy](https://privacy.microsoft.com/privacystatement)
- [Pricing](https://www.microsoft.com/en-us/security/business/microsoft-entra-pricing)
- [ChangeLog](https://learn.microsoft.com/en-us/graph/changelog)
- [GitHubOrganization](https://github.com/microsoftgraph)
- [GitHubRepository](https://github.com/microsoftgraph/microsoft-graph-openapi)
- [StackOverflow](https://stackoverflow.com/questions/tagged/microsoft-graph)
- [Training](https://learn.microsoft.com/en-us/training/paths/m365-msgraph-associate/)
- [SpectralRules](rules/active-directory-spectral-rules.yml)
- [NaftikoCapability](capabilities/identity-management-operations.yaml)
- [Vocabulary](vocabulary/active-directory-vocabulary.yaml)
- [JSON-LD](json-ld/active-directory-context.jsonld)

## Features

| Name | Description |
|------|-------------|
| Unified Identity API | Single REST endpoint (graph.microsoft.com) for all Microsoft Entra identity and directory operations. |
| User Lifecycle Management | Full CRUD operations for user accounts including bulk operations, license assignment, and guest management. |
| Group Management | Create and manage security groups, Microsoft 365 groups, and dynamic membership groups. |
| Application Registration | Programmatic app registration, permission configuration, and service principal management. |
| Conditional Access Automation | Create, update, and evaluate Conditional Access policies via API for Zero Trust enforcement. |
| Privileged Identity Management | Just-in-time role activation, time-bound access, and PIM policy management via API. |
| Identity Protection | Access risk signals, risky users, and risk detections for automated threat response. |
| Authentication Method Management | Manage MFA and passwordless authentication methods registered for users. |
| Audit and Sign-in Logs | Programmatic access to audit logs, sign-in logs, and provisioning logs for SIEM integration. |
| Identity Governance | Access reviews, entitlement management, and lifecycle workflows for automated IAM. |

## Use Cases

| Name | Description |
|------|-------------|
| User Provisioning Automation | Automate user account creation, attribute updates, and deprovisioning for HR-driven identity lifecycle. |
| Zero Trust Policy Enforcement | Programmatically deploy and manage Conditional Access policies across the organization. |
| SIEM Integration | Stream audit logs and sign-in events to security information and event management systems. |
| Application Access Management | Automate app registration, permission grants, and app role assignments for developer self-service. |
| Identity Risk Remediation | Detect and respond to risky sign-ins and compromised accounts via Identity Protection APIs. |
| Compliance Reporting | Generate access reviews, entitlement reports, and audit logs for regulatory compliance. |
| Privileged Access Governance | Enforce just-in-time privileged access and audit role assignments via PIM APIs. |

## Integrations

| Name | Description |
|------|-------------|
| Azure Active Directory | Microsoft Entra ID (formerly Azure AD) is the cloud identity backbone accessed via Microsoft Graph. |
| Microsoft 365 | Microsoft Graph provides unified access to Microsoft 365 user data alongside identity operations. |
| Azure Monitor | Stream Microsoft Entra sign-in and audit logs to Azure Monitor Log Analytics for analysis. |
| Microsoft Sentinel | Feed identity risk signals and audit logs into Microsoft Sentinel SIEM for threat hunting. |
| Intune | Microsoft Graph Intune APIs integrate device management with identity policies. |
| SCIM Providers | Automate user provisioning to SaaS applications using Microsoft Entra SCIM provisioning. |
| SAML and OIDC Applications | Register and manage federated applications using SAML 2.0 and OpenID Connect via Microsoft Graph. |

## Artifacts

Machine-readable API specifications organized by format.

### OpenAPI

- [Microsoft Graph Users API](openapi/active-directory-users-openapi.yaml)
- [Microsoft Graph Groups API](openapi/active-directory-groups-openapi.yaml)
- [Microsoft Graph Applications and Service Principals API](openapi/active-directory-applications-openapi.yaml)

### JSON Schema

- [User Schema](json-schema/users-user-schema.json)
- [Password Profile Schema](json-schema/users-password-profile-schema.json)
- [Group Schema](json-schema/groups-group-schema.json)
- [Application Schema](json-schema/applications-application-schema.json)
- [Service Principal Schema](json-schema/applications-service-principal-schema.json)

### JSON Structure

- [User Structure](json-structure/users-user-structure.json)
- [Group Structure](json-structure/groups-group-structure.json)
- [Application Structure](json-structure/applications-application-structure.json)

### JSON-LD

- [Active Directory Context](json-ld/active-directory-context.jsonld)

### Examples

- [User Example](examples/users-user-example.json)
- [Group Example](examples/groups-group-example.json)
- [Application Example](examples/applications-application-example.json)

## Capabilities

Naftiko capabilities organized as shared per-API definitions composed into customer-facing workflows.

### Shared Per-API Definitions

- [Active Directory Users](capabilities/shared/active-directory-users.yaml) — 5 operations for user lifecycle management
- [Active Directory Groups](capabilities/shared/active-directory-groups.yaml) — 3 operations for group management
- [Active Directory Applications](capabilities/shared/active-directory-applications.yaml) — 4 operations for application and service principal management

### Workflow Capabilities

| Workflow | APIs Combined | Tools | Persona |
|----------|--------------|-------|---------|
| [Identity Management Operations](capabilities/identity-management-operations.yaml) | Users, Groups, Applications | 10 | IT Administrator, Identity Engineer, Security Analyst |

## Vocabulary

- [Active Directory Vocabulary](vocabulary/active-directory-vocabulary.yaml) — Unified taxonomy mapping 12 resources, 9 actions, 1 workflow, and 3 personas across operational (OpenAPI) and capability (Naftiko) dimensions

## Rules

- [Active Directory Spectral Rules](rules/active-directory-spectral-rules.yml) — 30+ rules across 10 categories enforcing Microsoft Graph API conventions

## Maintainers

**FN:** Kin Lane

**Email:** kin@apievangelist.com
