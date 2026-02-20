# 📝 Create Case

This guide will walk you through creating a new case in CAS.

## Overview

When an Investigation Officer (IO) calls to request an Appropriate Adult, you will create a new case in CAS. The system will then broadcast to eligible AAs based on the case requirements.

---

## Quick Start (Most common flow)

1. Go to **Cases** → **Create New Case**
2. Add youth information and number of AAs required
3. Set interview schedule and location
4. Add IO contact details
5. Add special requirements (optional)
6. Choose **Assignment Method** (Broadcast, manual assignment or data entry)
7. Click **Start Broadcast**

---

### How Case Broadcast Works

**Broadcast Types:**

| Type | Name | AA Pool | When Used |
|------|------|---------|-----------|
| **B1** | Standard Broadcast | Primary region AAs | First broadcast |
| **B2** | Secondary Region | Primary + Secondary region AAs | Re-broadcasts |
| **B3** | Staff-Only | AA Staff only (ignores preferences) | Urgent final attempt |

**Broadcast Flow:**

1. **Broadcast 1 (B1)** → Case sent to AAs in primary region
2. **Holding Period** (5 mins) → System collects multiple responses
3. **Weighted Selection** → If multiple responses, system selects based on workload:
   - Bucket A (0-2 cases/month): 60% chance
   - Bucket B (3-6 cases/month): 30% chance
   - Bucket C (7+ cases/month): 10% chance
4. **Waiting Period** (10 mins) → FCFS if no response during holding
5. **Confirmation** (5 mins) → Selected AA must confirm assignment
6. **Broadcast 2 (B2)** → Expands to secondary regions if no confirmation
7. **Broadcast 3 (B3)** → Staff-only broadcast for urgent cases

**Urgency Classification:**

| Classification | Condition | Broadcast Sequence |
|----------------|-----------|-------------------|
| **Standard** | Interview > 4 hours away | B1 → B2 → B2... |
| **Urgent** | Interview ≤ 4 hours away | B1 → B2 → B3 |
| **Last Minute** | Interview ≤ 90 mins (AA cancels) | Force B3 immediately |

**8-Stage Filtering:** Before broadcast, system filters AAs by: Qualifications → Region → Timing → Gender → Language → Race → Cooldown → Quiet Hours

---

## Create New Case

### Step 1: Navigate to Cases

Login to CAS Web Portal. In the left-hand side menu, navigate to **Cases**

### Step 2: Click Create New Case

Click **Create New Case** button

![Create New Case 1](../images/Create%20new%20case%201%20replace.png){: style="max-width:800px"}

### Step 3: Fill Youth Information

Fill in the youth details:

- **Youth Name** – Full name of young suspect (required)
- **Youth Age** – Age of youth (6-17 years)
- **Youth Gender** – Male / Female / Other (required)

If more than one youth, click **Add New Youth** to add additional youth (maximum 7).

Then input the **Number of AAs Required** for this case.

![Create New Case 2](../images/create new case 2.png){: style="max-width:800px"}

### Step 4: Fill Offense Details

Select the **Specific Offense** from the offense list dropdown.

![Offense Details](../images/offense details.png){: style="max-width:800px"}

### Step 5: Specify Interview Schedule

- **Interview Date** – Date of interview
- **Interview Time** – Time of interview
- **Location** – Police station or other location
- **House Visit** – Check if interview requires house visit

![Interview Schedule 1](../images/interview schedule 1.png){: style="max-width:800px"}

If **House Visit** is checked, the House Visit qualification requirement will be automatically added.

![Interview Schedule 2](../images/interview schedule 2.png){: style="max-width:800px"}

### Step 6: Fill IO Information

- **IO Name** – Investigation Officer's full name (required)
- **Contact Number** – Primary phone (8 digits, starts with 6/8/9)
- **Alt Contact Number** – Alternative phone, optional (8 digits, starts with 6/8/9)

![IO Info](../images/IO%20Details.png){: style="max-width:800px"}

### Step 7: Select Special Requirements (Optional)

If the case requires specific AA characteristics:

- **Gender** – Male or Female AA preferred
- **Race** – Preferred ethnicity
- **Language** – Required spoken language
- **Qualifications** – Additional qualifications needed

![Special Requirements](../images/Special%20require.png){: style="max-width:800px"}

### Step 8: Choose Assignment Method

- **Broadcast** – Notify all eligible AAs via automated selection.
- **Manual Assignment** – Select a specific AA directly.
- **Data Entry Only** – Record completed case without notification. Use for cases completed offline, for records only.

**Broadcast:**

If you choose **Broadcast**, CAS will show:

- The **number of eligible AAs** for this case (based on the criteria you entered)
- Case-level **assignment timing parameters** that you can adjust for this specific case before starting:
  - **Holding Period**
  - **Waiting Period**
  - **Confirmation Period**

![Broadcast](../images/Broadcast%20replace.png){: style="max-width:800px"}

**Manual Assignment:**

If you choose **Manual Assignment**, you can view the list of **eligible AAs**, pick an AA by name and select manual assignment reason droplist.

**Urgent manual assignment:** If the manual assignment reason is **Urgent**, the AA must respond within **3 minutes**.

![Manual Assignment](../images/Manual assignment.png){: style="max-width:800px"}

**Data Entry Only:**

This method is used to **record cases that were completed offline** — no notification will be sent to AA, and the case goes directly to **Completed** status.

- **AA Name** – Shows all AAs for selection (search by name available)
- **Youth Name** – Auto-filled from youth info entered above

![Data Entry](../images/Data Entry.png){: style="max-width:800px"}

### Step 9: Start Broadcast/ Assignement or Save

- **Start Broadcast or Start Assignment** – Save and start broadcast/ assignment immediately
- **Save as Draft** – Save case to broadcast/ assignment later

---

## 🎥 Video Tutorial

Follow this short video to see how each case assignment method is created and how it appears on the AA mobile app!

### Broadcast and Pending Confirmation Case

<iframe width="560" height="315" src="https://www.youtube.com/embed/O1c6Lhqo1pI" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>


<iframe width="560" height="315" src="https://www.youtube.com/embed/gaimzN6Z20U" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

### Manual Assignment Case

<iframe width="560" height="315" src="https://www.youtube.com/embed/9XBtOPPteRM" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

### Data Entry

<iframe width="560" height="315" src="https://www.youtube.com/embed/T0orTEvNfPQ" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

---

## Next Steps

After creating a case: [Monitor Broadcast](monitor-broadcast.md) - Track AA responses and to **edit** or **cancel** a case, follow the steps in this page

## Troubleshooting

**Phone validation error**: Ensure phone is 8 digits starting with 6, 8, or 9

**Can't start broadcast**: Check all required fields are filled
