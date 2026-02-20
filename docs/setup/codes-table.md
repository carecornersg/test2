# Codes Table

This guide explains the Codes Table and how it syncs with VPRMS.

## Overview

The Codes Table contains reference (master) data used throughout CAS as **picklist/dropdown values** (e.g., gender, race, qualifications, regions).

This data is **maintained in VPRMS** and **synced from VPRMS to CAS** automatically.

In addition to standard code sets (Gender/Race/Qualification, etc.), CAS can also be configured with **additional code types** to support CAS picklists (for example **Police Division**, **Cancellation Reason** or **Offense Type**).

---

## View Codes Table

### Step 1: Navigate to Codes Table

In the left-hand side menu, navigate to **Codes Table**

### Step 2: View Synced Data

The following information is synced from VPRMS to CAS:

- **Qualifications** – AA certifications (e.g., YS Under 10, House Visit)
- **Race** – Ethnicity options
- **Gender** – Gender options
- **Region** – Police regions (North, South, East, West, Central)
- **Language** – Spoken languages
- **Timing Preference** – Preferred time windows for AA availability (used for scheduling and broadcast eligibility)

You can also quickly find and review codes using the page controls:

- **Search**: Search by **code name**
- **Filter by Type**: Narrow down to a specific code type
- **Filter by Status**: View Active/Inactive codes
- **Filter by Access**: Show **Read-only** (synced) vs **Editable** (admin-created) codes

⚠️ **Important (Edit icon):** If the **edit pen icon is greyed out**, it means the code is **synced from Salesforce (VPRMS)** and is **read-only in CAS**. To update it, make the change in **Salesforce** and wait for the next sync (or run **Sync with VPRMS**).

![Codes Table](../images/Codes%20table%201.png){: style="max-width:800px" }

### Sync Schedule

- **Automatic** – Every 30 minutes (polling for updates)
- **Daily Full Sync** – 2:00 AM (complete data reconciliation)
- **Manual Sync** – On-demand (triggered by System Administrator)

### Manual Sync (Optional)

If you need to sync immediately (e.g., after adding new values in VPRMS), click **Sync with VPRMS** and wait for completion. New values will appear in the table.

## Create a New Code

If you need to add a new picklist value to a code type (e.g., **Police Division**, **Offense Type**, **Cancellation Reason**) and your role has access.

### Step 1: Go to **Codes Table** and click **Create Code**

Click **Create Code** to open the form.

![Codes Table Filters](../images/Codes%20table%202.png){: style="max-width:800px" }

### Step 2: Fill in Details

- **Label**
- **Code**
- **Type** (select from the dropdown)
- **Description**

![Create Code](../images/Create%20code.png){: style="max-width:500px" }

### Step 3: Save Changes

Click **Create** to save changes.

## Edit an Existing Code (Admin-created)

If the code was created in CAS (not synced), you can edit it:

### Step 1: Click Edit

Click the **blue edit pen** icon.

![Edit Codes Table Step 1](../images/Edit%20codes%20table%201.png){: style="max-width:800px" }

### Step 2: Update Details

Update fields as needed:

- Edit **Label** and/or **Description**
- Toggle **Active** off to inactivate the code

![Edit Codes Table Step 2](../images/Edit%20codes%20table%202.png){: style="max-width:500px" }

### Step 3: Save Changes

Click **Update** to save changes.

## Troubleshooting

**New value not appearing**: Wait for next sync cycle or trigger manual sync

**Sync failed**: Check VPRMS connection, contact System Administrator

