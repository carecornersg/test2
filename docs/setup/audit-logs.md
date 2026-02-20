# Audit Logs

This guide explains how to use Audit Logs in CAS.

## Overview

Audit Logs provide a complete record of all actions performed in the CAS system. This helps with:

- **Accountability**: Track who did what and when
- **Troubleshooting**: Investigate issues by reviewing action history
- **Compliance**: Maintain records for audit purposes
- **Security**: Monitor for unauthorized or unusual activity

---

## Quick Start

1. Open **Audit Logs**
2. Filter by date range, user, or action type
3. Click any entry to review details
4. Export if needed (CSV)

---

## What Audit Trail Includes

Audit logs capture **who did what, when, and what changed**. Based on the functional specification, audit trail typically includes:

- **Case lifecycle & case actions**
  - Create/edit case, status transitions, start/stop broadcast, manual assignment, re-broadcast/escalation
  - **Case cancellation details**: cancelled by (user), reason, timestamp

- **User & authentication activities**
  - Login/logout
  - User created/updated/deactivated (accounts are preserved; deletion is not permanent)

- **System configuration changes**
  - System rules/config updates with before/after values (e.g., setting changed from old value to new value)

**Note:** Audit logs are used for accountability and compliance, and support troubleshooting by showing a full timeline of actions.

## View Audit Logs

### Step 1: Navigate to Audit Logs

In the left-hand side menu, navigate to **Audit Logs**

### Step 2: View Log Entries

The audit log displays:

- **Timestamp** – Date and time of action
- **User** – Who performed the action
- **Action** – What action was performed
- **Details** – Specific details of the change
- **IP Address** – Source IP (for security tracking)

### Filter and Export (Optional)

- **Filter by date range**: Select start and end dates to narrow down the log entries
- **Export**: Apply your filters, then click **Download** to export (CSV)

![Audit Log](../images/Audit%20log.png){: style="max-width:800px" }

## Logged Actions

The following actions are recorded in Audit Logs:

### User Actions
- User login / logout
- User created / edited / deactivated
- Password reset

### Case Actions
- Case created / edited / cancelled
- Broadcast started / stopped
- AA assigned / unassigned
- Case status changes

### System Actions
- System rules changed
- Configuration updates
- Sync events (VPRMS)

## Troubleshooting

**Can't find specific log**: Expand date range, check spelling of search terms

