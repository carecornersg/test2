# System Monitoring

This guide explains how to view system health and integration status.

---

## Overview

The **System Monitoring** dashboard provides real-time visibility into:

- VPRMS sync status
- Authentication/login activity
- SMS delivery health

![System Monitoring](../images/System%20monitoring.png){: style="max-width:850px" }

---

## Integration Status

### VPRMS Sync Status

Displays the status of data synchronisation between CAS and VPRMS (Salesforce).

- **Records Pushed**: Number of records synced to VPRMS
- **AAs Synced**: Number of AA profiles synced
- **Errors (24h)**: Sync errors in the last 24 hours
- **Last Sync**: Timestamp of the most recent sync

A green checkmark (✓) indicates sync is healthy.

---

### Authentication Status

Displays login and session activity for Web Portal users.

- **Active Sessions**: Number of users currently logged in
- **Logins Today**: Total login attempts today
- **Failed Logins**: Number of failed login attempts today
- **Azure AD Operational**: Indicates Azure AD SSO is working

---

### SMS Delivery Status

Displays SMS notification delivery metrics.

- **Sent Today**: Total SMS sent today
- **Last Sent**: Time of the most recent SMS
- **Delivered**: Number of SMS successfully delivered
- **Failed**: Number of SMS that failed to deliver
- **Message Delivered**: Delivery success rate (%)

A "Healthy" badge indicates SMS delivery is operating normally.

---

## Login Activity

The **Login Activity** table shows recent login attempts to the Web Portal.

| Column | Description |
|--------|-------------|
| Time | Timestamp of the login attempt |
| User Name | Name of the user |
| Status | Success or Failed |
| Failure Reason | Reason for failure (e.g., Invalid OTP) |
| IP Address | IP address of the login attempt |

This helps administrators monitor for:

- Unusual login patterns
- Failed login attempts (security monitoring)
- User activity auditing


