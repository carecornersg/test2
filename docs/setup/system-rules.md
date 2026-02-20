# System Rules

This guide will walk you through configuring system rules in CAS.

## Overview

System Rules allow you to customize the behavior of the assignment workflow, weighted selection logic, and other system configurations. These settings are optional and can be adjusted by **AAYS Managers** and **System Administrators**.

---

## Quick Start

Most updates follow this flow:

1. Open the relevant section (Weighted Selection Logic / Assignment Workflow / Configurations)
2. Update values as needed
3. Click **Save Changes**

**Tip:** Changes apply to **new broadcasts only** (existing in-progress broadcasts are unaffected).

---

## Weighted Selection Logic

Configure how AAs are selected for case assignments.

### Step 1: Navigate to Weighted Selection Logic

In the left-hand side menu, navigate to **System Rules** → **Weighted Selection Logic**

![Weighted Selection](../images/Weighted%20Selection.png){: style="max-width:860px"}

### Step 2: Configure Settings

| Setting | Description | Default |
|---------|-------------|---------|
| **Weighted Balance Period** | Rolling window for case count calculation (days) | 30 days |
| **Low Priority Reset** | Duration before low priority flag is cleared (days) | 14 days |
| **Bucket A Range** | Monthly cases for 60% probability | 0-2 cases |
| **Bucket B Range** | Monthly cases for 30% probability | 3-6 cases |
| **Bucket C Range** | Monthly cases for 10% probability | 7+ cases |

### Step 3: Click Save Changes

Click **Save Changes** to apply the new settings.

---

## Assignment Workflow

Configure timing parameters for the broadcast and assignment process.

### Step 1: Navigate to Assignment Workflow

In the left-hand side menu, navigate to **System Rules** → **Assignment Workflow**

![Assignment Workflow](../images/Assignment%20workflow.png){: style="max-width:800px"}

### Step 2: Configure Settings

| Setting | Description | Default |
|---------|-------------|---------|
| **Holding Period** | Collection time for Broadcast 1 (minutes) | 5 mins |
| **Waiting Period** | FCFS window after holding, applies to all broadcasts (minutes) | 10 mins |
| **Confirmation Period** | Time for AA to confirm after selection (minutes) | 5 mins |
| **Interview Reminder Period** | Reminder sent before interview time (hours) | 2 hours |
| **Documentation Reminder** | Reminder sent after interview time if documentation is still pending (hours) | 4 hours |
| **Urgency Threshold** | Time threshold to mark case as Urgent (hours) | 4 hours |
| **Cooldown Period** | Rest period for AA after assignment (hours) | 3 hours |

### Step 3: Click Save Changes

Click **Save Changes** to apply the new settings.

---

## Configurations

Configure general system settings.

### Step 1: Navigate to Configurations

In the left-hand side menu, navigate to **System Rules** → **Configurations**

![Configuration](../images/Configuration%201.png){: style="max-width:800px"}

### Step 2: Configure Settings

| Setting | Description | Default |
|---------|-------------|---------|
| **Call Centre Inactivity Timeout** | Auto-logout for web portal (hours) | 2 hours |
| **Mobile App Inactivity Timeout** | Auto-logout for mobile app (hours) | 0.5 hours |
| **Transport Allowance** | Reimbursement amount per case (dollars) | $50 |

### Step 3: Click Save Changes

Click **Save Changes** to apply the new settings.

---

## Important Notes

- Changes apply to **new broadcasts only** (existing in-progress broadcasts are unaffected)
- All configuration changes are logged in Audit Logs
- Only AAYS Manager and System Administrator can modify these settings

## Troubleshooting

**Settings not saving**: Check you have the correct permissions (AAYS Manager or System Administrator)

**Changes not taking effect**: Changes only apply to new broadcasts, not existing ones

