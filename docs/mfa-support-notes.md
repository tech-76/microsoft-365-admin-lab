# MFA Support Notes

## Purpose

Multi-factor authentication adds an extra layer of protection to user accounts. Help desk teams often support users who lose access to their MFA device, change phones, delete the Authenticator app, or cannot complete sign-in approval.

## Common MFA Issues

- User changed phone
- User lost phone
- Authenticator app was deleted
- Push notification not appearing
- User cannot receive SMS code
- User is stuck in an MFA registration loop
- User gets repeated MFA prompts
- User cannot access email after MFA reset

## Basic MFA Troubleshooting Questions

- Did the user recently change phones?
- Is the user's device connected to the internet?
- Is the Authenticator app installed?
- Is the correct account added to the app?
- Is the device time and date correct?
- Is SMS or phone call verification available?
- Is the user traveling or signing in from a new location?

## MFA Reset Workflow

1. Verify the user's identity.
2. Confirm the issue and affected device.
3. Review the user's MFA methods if access is available.
4. Remove or reset the outdated method if approved.
5. Ask the user to register a new MFA method.
6. Confirm successful sign-in.
7. Document the change in the ticket.

## Security Considerations

- MFA resets are sensitive.
- Always verify the user before changing MFA methods.
- Escalate suspicious requests.
- Watch for signs of social engineering.
- Do not approve MFA changes based only on email requests.
- Document all actions clearly.

## Example Ticket Note

User reported new phone and could not access Microsoft Authenticator prompts. Verified identity according to procedure. Reset MFA registration and guided user through adding the new device. User confirmed successful sign-in.
