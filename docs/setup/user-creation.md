# User Creation

This guide will walk you through creating and managing user accounts.

## Overview

User management is available to **System Administrators** only. This section covers how to create, edit, and manage user accounts for the CAS Web Portal.

---

## Role Permissions

Different roles have different capabilities in CAS:

### Call Centre Staff

- ✅ View case dashboard (real-time status)
- ✅ Create and edit cases
- ✅ Start/Stop broadcast
- ✅ Manual AA assignment
- ✅ Cancel cases
- ✅ View AA profiles (read-only)
- ❌ Cannot create completed cases (Data Entry)
- ❌ Cannot access advanced reports
- ❌ Cannot configure system settings

### AAYS Manager

- ✅ All Call Centre Staff functions
- ✅ Full reporting access (all dashboards)
- ✅ AA management (override availability, view qualifications)
- ✅ Data export (CSV)
- ✅ Configure assignment logic
- ✅ View case-related audit logs only
- ❌ Cannot perform user management

### System Administrator

- ✅ All AAYS Manager functions
- ✅ User management (create/edit/deactivate users)
- ✅ System configuration (notifications, integrations)
- ✅ Full Audit Logs access

## Create User

### Step 1: Navigate to Users

In the left-hand side menu, navigate to **Users**

### Step 2: Click Create User

Click the **Create User** button

![Create User Step 2](../images/Create%20user%201.png){: style="max-width:800px"}

### Step 3: Fill In User Details

Fill in the following information:

- **Name** – User's full name
- **Email** – Login email address
- **Role** – Select: AAYS Manager, System Administrator, or Call Centre Staff

![Create User Step 3](../images/Create%20user.png){: style="max-width:350px"}

### Step 4: Click Create

Click **Create** to save the new user.

The user will receive email with a link to create password.

## Edit User

### Step 1: Select User

- Click on the user name in the Users list
- Click **Edit** button

![Edit User Step 1](../images/Edit%20user%201%20replace.png){: style="max-width:800px"}

### Step 2: Update Details

- Modify the user information as needed
- Toggle off **Active** if you want to deactivate user

![Edit User Step 2](../images/Edit%20user%202%20replace.png){: style="max-width:350px"}

**What happens when a user is deactivated:**

- ❌ User cannot login to CAS
- ❌ If user is an AA, they will not receive any broadcasts
- ✅ User records and history are preserved
- ✅ User can be reactivated anytime

### Step 3: Save Changes

Click **Update** to apply changes

---

## ⚠️ Important: Users Cannot Be Deleted

CAS does **not allow permanent deletion** of user accounts. Users can only be **deactivated**.

**Reasons:**

- 📋 **Audit Trail** – All user actions must be traceable for compliance
- 🔗 **Data Integrity** – Cases and logs reference user accounts
- 📁 **Record Keeping** – Historical data must be preserved

If you need to remove a user, simply **deactivate** them. Their account will remain in the system but they will not be able to access CAS.

---

## Troubleshooting

**User can't login**: Check if user status is Active, try resetting password

**Wrong permissions**: Verify the correct role is assigned

**Not receiving emails**: Check email address is correct, check spam folder

