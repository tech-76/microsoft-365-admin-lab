# Microsoft 365 Support Workflow

## Purpose

This diagram shows a professional Microsoft 365 support workflow for common help desk issues such as sign-in problems, password resets, Outlook issues, mailbox access, MFA problems, Teams support, and licensing checks.

```mermaid
flowchart TB
    A["Microsoft 365 Support Request"] --> B["Confirm User and Issue Details<br/>User, service affected, error message, impact"]
    B --> C{"What type of issue<br/>is being reported?"}

    C -->|Sign-in / Password| D["Check account status<br/>Verify username, password, and account access"]
    C -->|Outlook / Email| E["Check Outlook and email access<br/>Desktop, web, send/receive, mailbox status"]
    C -->|Mailbox Access| F["Check mailbox permissions<br/>Shared mailbox, full access, send as"]
    C -->|MFA Issue| G["Verify user identity<br/>Review MFA device, method, or reset need"]
    C -->|Teams Issue| H["Check Teams access<br/>Sign-in, app status, audio/video, permissions"]
    C -->|License Issue| I["Check assigned license<br/>Service availability and product access"]

    D --> D1{"Can user sign in?"}
    D1 -->|No| D2["Reset password or unlock account<br/>Confirm sign-in again"]
    D1 -->|Yes| J["Document findings and confirm access"]

    E --> E1{"Does Outlook Web work?"}
    E1 -->|Yes| E2["Troubleshoot Outlook desktop<br/>Profile, cache, updates, connectivity"]
    E1 -->|No| E3["Check mailbox, account, service health,<br/>or broader Microsoft 365 issue"]
    E2 --> J
    E3 --> K["Escalate if needed with clear notes"]

    F --> F1{"Does user have correct access?"}
    F1 -->|No| F2["Review approval and assign mailbox permissions"]
    F1 -->|Yes| F3["Check Outlook refresh or re-login"]
    F2 --> J
    F3 --> J

    G --> G1{"Is MFA reset required?"}
    G1 -->|Yes| G2["Reset MFA after identity verification<br/>Guide user through re-registration"]
    G1 -->|No| G3["Troubleshoot MFA method<br/>Authenticator, SMS, call, prompts"]
    G2 --> J
    G3 --> J

    H --> H1{"Is Teams issue app-specific?"}
    H1 -->|Yes| H2["Check Teams desktop app<br/>Cache, update, sign-out, reinstall"]
    H1 -->|No| H3["Check web access, permissions,<br/>device settings, or service issue"]
    H2 --> J
    H3 --> K

    I --> I1{"Correct license assigned?"}
    I1 -->|No| I2["Assign approved license<br/>Confirm service is enabled"]
    I1 -->|Yes| I3["Check account provisioning<br/>and service availability"]
    I2 --> J
    I3 --> J

    J --> L["Confirm issue resolved with user"]
    L --> M["Document troubleshooting steps,<br/>resolution, and user confirmation"]
    M --> N["Close Ticket"]

    K --> O["Escalate Ticket<br/>Include impact, error, steps taken, screenshots, and results"]
```

## What This Workflow Demonstrates

- Microsoft 365 help desk workflow
- Sign-in and password troubleshooting
- Outlook and email troubleshooting
- Shared mailbox access support
- MFA support and reset process
- Microsoft Teams support
- Licensing checks
- Ticket escalation and documentation

## Common Microsoft 365 Support Scenarios

| Scenario | Example Support Action |
|---|---|
| User cannot sign in | Check account status, reset password, confirm MFA |
| Outlook not working | Test Outlook web, rebuild profile, review mailbox |
| Shared mailbox missing | Check permissions and Outlook refresh |
| MFA prompts not working | Verify identity and reset MFA if needed |
| Teams audio/video issue | Check device settings, Teams app, permissions |
| Missing app access | Check assigned license and enabled services |

## Example Support Notes

When documenting a Microsoft 365 issue, include:

- User impact
- Service affected
- Error message
- Troubleshooting completed
- Whether issue affects one user or multiple users
- Account or license checks completed
- Resolution provided
- User confirmation
- Escalation details if unresolved

## Portfolio Note

This workflow is part of a Microsoft 365 Admin Lab designed to demonstrate practical IT Support, Service Desk, Desktop Support, and Junior Systems Administrator documentation skills.
