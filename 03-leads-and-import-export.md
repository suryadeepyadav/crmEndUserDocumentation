# Leads and CSV Import/Export

## What a lead is

A **Lead** is an early sales enquiry from a person or organization that may need an HHCIL service. It is not yet a confirmed customer opportunity. A lead stores the enquiry, interested services, source, responsible branch, owner, response deadline, activities, and follow-ups.

Leads may be entered manually, imported from a spreadsheet, or received from a connected website form. Website job enquiries are routed separately and are not created as B2B sales leads.

## Why and when to use Leads

Use Lead inbox whenever an enquiry still needs initial review, contact, qualification, or conversion. The lead stage helps the team respond promptly without creating a full customer and opportunity record too early.

Do not create a second lead merely because you cannot find the first one. Search by organization, contact, email, or phone, and check duplicate suggestions first.

## Lead inbox

The Lead inbox shows the leads you are allowed to see. The table includes:

- lead company and contact details;
- current status;
- lead source;
- owner; and
- response target.

An overdue response time is highlighted so it can be handled first.

### Search and filters

- The **Search and filter leads** section starts closed so the lead list has more room. Select its header to open it. If filters are already applied, the header shows how many are active even while closed.
- Enter text in **Search leads** and press Enter or select **Search leads**. Use the clear icon in the search field to remove the text search.
- Select a **Status** to limit the list.
- Filter by **Source**, requested **Service**, **Branch**, or **Owner** (when your role can see user choices).
- Use **Created from** and **Created to** for a received-date range.
- Select **Response overdue** to show leads whose first-response target has passed.
- Select **Not yet contacted** to find New or Assigned leads without a recorded first customer contact.
- Select **Possible duplicates** to review leads that match another lead you are allowed to see by company, email, or phone. Review both records before merging.
- Select **Clear filters** to return to the full visible list.
- Select **Refresh** to reload the latest results.
- Select the section header again to close the controls without removing your applied filters.

Lead inbox displays 25 records per page. Use the page controls to move through the result set. The current table does not provide clickable column sorting.

## Creating a lead manually

Select **Create lead** and complete the form.

| Field         | What to enter                                                             | Required? |
| ------------- | ------------------------------------------------------------------------- | --------: |
| Company name  | The organization making the enquiry, using its recognizable business name |       Yes |
| Contact name  | The name of the person making or representing the enquiry                 |       Yes |
| Email         | A verified business email, when provided                                  |        No |
| Phone         | A verified contact number, including useful area/country code             |        No |
| Services      | One or more services the prospect is asking about                         |       Yes |
| Lead source   | How the enquiry reached HHCIL, such as Manual Entry or Referral           |       Yes |
| Branch        | The HHCIL branch responsible for the enquiry                              |       Yes |
| City          | The city connected to the requested service or prospect                   |        No |
| Enquiry notes | The customer's need, scale, timing, and other useful context              |        No |

Select **Create and assign** to save. The signed-in user becomes the owner of a manually created lead. The response target is calculated from the selected source or assignment rule.

### Real-world example

An operations manager from “Northstar Textiles Pvt Ltd” calls the Pune branch about housekeeping for two facilities. Create a lead with:

- Company name: Northstar Textiles Pvt Ltd
- Contact name: Kavita Rao
- Service: Housekeeping
- Source: Manual Entry
- Branch: Pune
- City: Pune
- Enquiry notes: “Housekeeping for two plants; approximately 60 workers; requested a site discussion this week.”

Avoid entering only “interested” as the note. Useful context reduces repeated questions and helps later requirement collection.

## Lead sources and response targets

The initial configuration includes these sources:

| Source                   | Typical meaning                            | Default response target |
| ------------------------ | ------------------------------------------ | ----------------------: |
| Manual Entry             | Entered by an HHCIL user                   |             240 minutes |
| Website Service Enquiry  | Service request from the website           |              60 minutes |
| Website Consultation     | Website request for consultation           |              60 minutes |
| Website Brochure Request | Website request for information            |             240 minutes |
| Referral                 | Referred by another person or organization |             240 minutes |
| Imported                 | Created through CSV import                 |             480 minutes |

An administrator can add sources or assignment rules, so your organization’s live values may differ. The response deadline shown on the lead is the value that applies to that record.

## Lead statuses

| Status       | Meaning                                                                         |
| ------------ | ------------------------------------------------------------------------------- |
| New          | The enquiry has been received and still needs initial handling.                 |
| Assigned     | An owner has responsibility for responding and progressing the lead.            |
| Contacted    | A first customer contact has been recorded as a Call, Email, or Meeting.        |
| Qualified    | The enquiry has enough fit and intent to become an opportunity.                 |
| Converted    | The CRM has created the connected account, contact, opportunity, and follow-up. |
| Disqualified | The enquiry will not proceed as a sales lead, for a recorded business reason.   |
| Duplicate    | The record has been identified as another copy of an existing lead.             |

Manual creation normally assigns the lead immediately. Website assignment is determined by trusted assignment rules. After a Call, Email, or Meeting changes the lead to **Contacted**, an authorized user can select **Mark as qualified** on the lead detail page. Authorized users can also disqualify an unsuitable lead or merge a confirmed duplicate from its detail page.

## Lead detail page

Open a row in Lead inbox to see:

- organization and contact details;
- phone and city;
- current owner and responsible branch;
- response due time and first-contact time;
- interested services;
- original enquiry notes;
- activity timeline;
- follow-up tasks; and
- possible duplicate leads; and
- attached documents when your role has file access.

Converted, disqualified, and duplicate leads are retained as history and cannot be converted again.

## Editing a lead

Users with lead-update permission can select **Edit** on the lead detail page. Use this action to correct or update the same enquiry.

| Field                | Guidance                                                                    |
| -------------------- | --------------------------------------------------------------------------- |
| Company name         | Correct or current organization name for this enquiry                       |
| Contact name         | Correct name of the person representing the enquiry                         |
| Email and phone      | Verified contact details; either value may be cleared if it is not reliable |
| City                 | City connected to the prospect or requested service                         |
| Preferred start date | Customer's requested service start date, when known                         |
| Lead source          | Correct origin of the enquiry                                               |
| Services             | One or more services currently requested                                    |
| Enquiry notes        | Useful updated context about need, scale, timing, or constraints            |

Editing does not change the lead's branch or owner. Assignment is a separate controlled action described below. Saving uses the latest version of the lead; if another user changed it first, refresh and review the newer information before trying again.

## Assigning or reassigning a lead

Users with lead-assignment permission can select **Assign lead** or **Reassign lead** on the lead detail page. Standard Branch Manager, Regional Manager, Sales Head, and System Administrator roles have this permission; a Sales Executive does not normally have it.

1. Open the lead and select **Reassign lead**.
2. Select the responsible **Branch**. Only branches within your permitted scope are available.
3. Select **Assign to**. The list contains active users whose primary branch matches the selected branch and shows their role and email for identification.
4. Set the **Response deadline** in your configured local timezone.
5. Enter an **Assignment reason** explaining why ownership is changing.
6. Select **Reassign lead** to save.

The CRM updates the owner, branch, and response deadline together. It records assignment history and an audit event, and creates an in-app notification for the new owner. The previous owner may immediately lose access when they are no longer the owner and do not otherwise have branch-level visibility.

Example: a Branch Manager reassigns an Ahmedabad security-services enquiry from one Sales Executive to another because the original owner is on leave. The manager keeps the Ahmedabad branch, chooses the replacement executive, sets a new response deadline, and records “Covering Ahmedabad enquiries during approved leave.”

If the required user is not listed, confirm that the user is active and that their **Primary branch** matches the selected branch. Do not change a user's branch merely to bypass record-visibility rules.

## Archiving a lead

Users with lead-update permission can select **Archive** when a lead should leave active CRM views, for example when it was created only for testing or entered in error and no normal lead status correctly represents it.

1. Open the lead and select **Archive**.
2. Read the confirmation message.
3. Enter a clear reason of at least three characters.
4. Select **Archive lead**.

The lead and its related task records leave normal active views, while audit history is retained. There is currently no Restore button. Do not archive a genuine lost or unsuitable enquiry merely to avoid using the proper disqualification or duplicate process.

## Recording an activity

### What an activity is

An **Activity** is a dated record of something that happened, such as a call, email, meeting, site survey, internal note, follow-up, or account review. It answers “what happened?” A task answers “what still needs to happen?”

### How to log one

1. Open the lead.
2. Select **Log activity**.
3. Choose an **Activity type**.
4. Set **Occurred at** to the actual date and time.
5. Enter a clear **Subject**.
6. Add **Notes** and an **Outcome** when useful.
7. Save the activity.

| Field         | Guidance                                                                          |
| ------------- | --------------------------------------------------------------------------------- |
| Activity type | Choose the closest business action. Do not use Internal Note for a customer call. |
| Occurred at   | Use when the activity actually occurred, not merely when you entered it.          |
| Subject       | Write a short summary such as “Initial requirement call”.                         |
| Notes         | Record relevant facts, requirements, objections, or agreed actions.               |
| Outcome       | State the result, such as “Site discussion agreed for Friday”.                    |

The first saved Call, Email, or Meeting records the first-contact time and moves an eligible lead to **Contacted**. An internal note does not satisfy the first-response requirement.

### Example

- Activity type: Call
- Subject: Initial requirement call
- Notes: “Customer needs housekeeping at two plants and will share current staffing details.”
- Outcome: “Requirement meeting agreed for 3 October at 11:00.”

## Marking a lead as qualified

### What it means

**Qualified** means the initial customer conversation shows that the enquiry is genuine and worth managing as a sales opportunity. It is the required step between **Contacted** and **Converted**.

### When to use it

Use **Mark as qualified** after recording a Call, Email, or Meeting and confirming the basic fit, such as the requested service, location or timing, relevant decision-maker/contact, and a realistic next step. Do not qualify a lead simply because it has an email address or because the first response deadline is close.

### How to mark it qualified

1. Open the contacted lead.
2. Review the activity timeline and any possible duplicates.
3. Select **Mark as qualified**.
4. Read the confirmation message and select **Mark as qualified** again.
5. Confirm that the status chip now shows **Qualified**. The **Convert lead** action becomes available if your role has conversion permission.

Example: after Kavita confirms that Northstar Textiles needs housekeeping at two plants and agrees to provide site details, the salesperson records the call and marks the lead qualified. The salesperson can now create the account and opportunity without treating the deal as won.

If **Mark as qualified** is missing, first record a Call, Email, or Meeting. The action is also hidden if your role does not have permission to update leads or you cannot access that lead.

## Possible duplicates

The detail page can show other records that resemble the lead. Suggestions may be based on identifying information such as company, email, or phone.

Before continuing:

1. Open the suggested record.
2. Compare organization and contact details.
3. Confirm whether it is the same enquiry, a related contact, or a different organization.
4. Avoid converting both copies.

If the two records describe the same enquiry, select **Merge duplicate** on the record that should be closed. Choose the surviving lead, enter a reason, and confirm. The CRM marks the current record **Duplicate** and moves its activities, tasks, and requested services to the surviving lead. Review the chosen survivor carefully: a merge changes linked history and should not be used for different enquiries from the same company.

## Disqualifying a lead

Use **Disqualify** when the enquiry should not continue as a sales lead, such as a request outside HHCIL's services or a prospect that is not qualified. Select a configured reason, add helpful notes, and confirm. The lead remains in history with **Disqualified** status. Use **Merge duplicate** for a confirmed duplicate instead of disqualifying it. A converted, disqualified, or duplicate lead cannot be disqualified again.

## Converting a lead

### What conversion does

Conversion turns a qualified enquiry into the records needed to manage a real deal. The CRM creates all of the following together:

- an Account for the customer organization;
- a Contact for the lead person;
- an Opportunity for the potential business;
- the initial opportunity stage; and
- a follow-up task based on the next action.

If any part cannot be created, the whole conversion is cancelled so that partial or disconnected records are not left behind.

### When to convert

Convert only after the lead status is **Qualified** and after confirming that:

- the organization and contact are genuine;
- the requested service is relevant to HHCIL;
- there is a realistic business need or next step; and
- the basic account and opportunity information is known.

### How to convert

1. Open an eligible lead.
2. Review duplicate suggestions.
3. Record the customer contact and qualification notes.
4. Select **Mark as qualified** and confirm the action.
5. Select **Convert lead**.
6. Complete the conversion fields.
7. Confirm conversion.
8. The CRM opens the new opportunity.

| Field               | What to enter                                                                                 | Required? |
| ------------------- | --------------------------------------------------------------------------------------------- | --------: |
| Legal account name  | Customer’s legal organization name; prefilled from the lead but should be corrected if needed |       Yes |
| Trade name          | Common or brand name if different                                                             |        No |
| Industry            | Closest available industry classification                                                     |        No |
| Billing address     | Known billing or registered address                                                           |        No |
| Opportunity title   | A clear deal name such as “Pune plants housekeeping FY27”                                     |       Yes |
| Expected close date | The best realistic date for a commercial decision                                             |       Yes |
| Indicative amount   | Estimated opportunity value, if known                                                         |        No |
| Next action         | The specific next step, such as “Collect staffing matrix”                                     |       Yes |
| Next action due     | Date and time by which that action should be completed                                        |       Yes |

### Important notes

- Conversion is not the same as winning a deal.
- The initial amount may be updated as requirements and pricing become clearer.
- The next action creates a task and due-time reminder that can appear in Tasks and notifications.
- A new opportunity for an existing customer can also be created from that customer's Account page.

## Importing leads from CSV

### What it is and when to use it

CSV import is for a controlled batch of leads from a spreadsheet or source list. Use manual creation for one or two leads. Clean and validate the spreadsheet before importing; import is not a substitute for data preparation.

### File limits

- File type: CSV
- Maximum file size: 5 MB
- Maximum rows: 1,000 per import

### Supported columns

Use this header row:

```text
company_name,contact_name,email,phone,city,service_keys,source_key,branch_key,message
```

| Column         | Guidance                                                                    |
| -------------- | --------------------------------------------------------------------------- |
| `company_name` | Required organization name                                                  |
| `contact_name` | Required contact person                                                     |
| `email`        | Optional valid email                                                        |
| `phone`        | Optional contact number                                                     |
| `city`         | Optional city                                                               |
| `service_keys` | Required stable service key or keys; separate multiple keys with semicolons |
| `source_key`   | Existing lead-source key; blank uses the Imported source                    |
| `branch_key`   | Required existing branch key                                                |
| `message`      | Enquiry details or source notes                                             |

The stable keys are administration values, not necessarily the displayed names. Ask the CRM administrator for the current service, source, and branch keys before preparing a file.

### Import workflow

1. In Lead inbox, select **Import CSV**.
2. Download the template if you need the current column names and sample master keys, then choose the prepared file.
3. Review the preview summary:
   - total rows;
   - valid rows;
   - possible duplicates; and
   - invalid rows.
4. Review the displayed preview rows and error messages.
5. Select **Download issue report** to keep the invalid-row and possible-duplicate details, then correct the source file if required and preview it again.
6. Import the valid rows.

The preview shows the first 20 rows for review. The current screen imports only rows classified as **valid**. Possible duplicates and invalid rows are not imported. Imported leads are assigned to the signed-in user, and the user must be allowed to work with the selected branch.

### Example row

```csv
Northstar Textiles Pvt Ltd,Kavita Rao,kavita@example.com,9876543210,Pune,housekeeping;security,import,pune,Two plants requiring initial consultation
```

Do not guess stable keys. An unknown service or branch key causes row validation to fail.

## Exporting leads

Users with the restricted export permission can select **Export** from Lead inbox. The CRM downloads a CSV of leads the user is allowed to see, up to the export limit of 10,000 records. The action is recorded for audit purposes.

Export applies the current Lead inbox filters within your permitted record scope. Review the filters before downloading and treat the file as confidential. The export has a 10,000-record limit.

## Related features

- [Dashboard](02-dashboard.md)
- [Accounts, contacts, and locations](04-accounts-contacts-and-locations.md)
- [Opportunities, activities, and tasks](05-opportunities-activities-and-tasks.md)
- [Complete business scenarios](12-complete-business-scenarios.md)

## Common problems

**I cannot see Create lead.**  
Your role may not have lead-creation permission.

**A branch is missing from the form.**  
It may be outside your assigned scope or inactive. Ask the administrator to check your visible branches.

**The lead is still response-overdue after I saved notes.**  
Record a Call, Email, or Meeting activity.

**Convert lead is missing.**  
First confirm that the lead status is **Qualified**. If it is still Assigned or Contacted, record the customer contact when needed and select **Mark as qualified**. The action is also hidden for converted, disqualified, or duplicate leads and for users without conversion permission.

**Mark as qualified is missing.**  
Record a Call, Email, or Meeting first so that the status becomes **Contacted**. If the lead is already qualified or is no longer active, the action is not shown. Your role also needs lead-update permission.

**Edit or Archive is missing.**  
Your role may not have lead-update permission, or the record may be outside your ownership, branch, or regional scope.

**Some CSV rows did not import.**  
Review whether they were marked invalid or possible duplicates. Correct required values and stable keys before trying those rows again.
