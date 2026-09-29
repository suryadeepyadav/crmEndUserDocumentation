# Glossary, Status Reference, FAQs, and Troubleshooting

## CRM and business glossary

| Term                 | Plain-language meaning                                                                                              |
| -------------------- | ------------------------------------------------------------------------------------------------------------------- |
| CRM                  | Customer Relationship Management application used to manage enquiries, customers, sales work, and post-sale records |
| Lead                 | Early enquiry that still needs contact, qualification, or conversion                                                |
| Lead source          | Where the enquiry came from, such as website, referral, or manual entry                                             |
| Response target      | Deadline for the first customer response                                                                            |
| First contact        | First recorded Call, Email, or Meeting with the lead                                                                |
| Assignment           | Giving responsibility for a lead or task to a user                                                                  |
| Owner                | Person responsible for progressing a record                                                                         |
| Account              | Customer or prospective customer organization                                                                       |
| Trade name           | Familiar brand name, when different from the legal name                                                             |
| GSTIN                | Goods and Services Tax Identification Number                                                                        |
| Contact              | Person connected to an account                                                                                      |
| Influence            | Contact’s role in a buying or service decision                                                                      |
| Location             | Physical customer site where service may be surveyed or delivered                                                   |
| Opportunity          | Specific potential sale being actively pursued                                                                      |
| Pipeline             | Collection of opportunities grouped by progress stage                                                               |
| Stage                | Current step in the sales process                                                                                   |
| Probability          | Estimated percentage chance of winning an opportunity                                                               |
| Weighted pipeline    | Opportunity value multiplied by probability                                                                         |
| Expected close       | Forecast date for the customer’s commercial decision                                                                |
| Activity             | Historical record of something that happened                                                                        |
| Task / follow-up     | Work that still needs to be completed                                                                               |
| Requirement          | Structured record of what the customer needs for one service                                                        |
| Requirement template | Versioned set of service-specific questions                                                                         |
| Snapshot             | Frozen copy of information at an approval or handover point                                                         |
| Site survey          | Planned visit to inspect and understand a service location                                                          |
| Quote                | Versioned commercial offer containing price, tax, terms, and scope references                                       |
| Recurring charge     | Charge expected to repeat, such as a monthly service fee                                                            |
| One-time charge      | Charge applied once, such as mobilization                                                                           |
| Approval policy      | Rule deciding which roles must approve a quote                                                                      |
| Contract             | Record of agreed service dates, sites, contact, signed agreement, and renewal information                           |
| Amendment            | Approved change that preserves the previous contract history                                                        |
| Renewal notice days  | Number of days before expiry to begin renewal work                                                                  |
| Handover             | Controlled transfer of approved sales/contract information to operations                                            |
| Branch               | HHCIL business unit responsible for records                                                                         |
| Region               | Group of branches                                                                                                   |
| Scope                | Record boundary a user is allowed to see or change                                                                  |
| Permission           | Specific action a role is allowed to perform                                                                        |
| Stable key           | Permanent administrator identifier used by imports, rules, or integrations                                          |
| Audit history        | Read-only record of important user and system actions                                                               |

## Status quick reference

### Lead statuses

| Status       | Meaning                                                   |
| ------------ | --------------------------------------------------------- |
| New          | Received and awaiting initial handling                    |
| Assigned     | Responsibility has been given to an owner                 |
| Contacted    | First Call, Email, or Meeting has been recorded           |
| Qualified    | Suitable to progress as a real opportunity                |
| Converted    | Account, contact, opportunity, and follow-up were created |
| Disqualified | Will not proceed as a sales lead                          |
| Duplicate    | Another record represents the same enquiry                |

### Opportunity stages

| Stage                  | Meaning                                                 |
| ---------------------- | ------------------------------------------------------- |
| Qualification          | Confirming need, fit, authority, and timing             |
| Requirement Collection | Capturing the service scope                             |
| Site Survey            | Inspecting or planning the customer site                |
| Proposal Preparation   | Preparing the commercial solution                       |
| Internal Approval      | Quote is being reviewed inside HHCIL                    |
| Proposal Sent          | Approved offer was sent to the customer                 |
| Negotiation            | Scope or commercial terms are being discussed           |
| Won                    | Customer agreed and required commercial evidence exists |
| Lost                   | Opportunity will not proceed                            |
| On Hold                | Temporarily paused, not closed                          |

### Requirement statuses

| Status   | Meaning                           |
| -------- | --------------------------------- |
| Draft    | Saved for review                  |
| Approved | Frozen as approved scope evidence |

### Quote statuses

| Status            | Meaning                                     |
| ----------------- | ------------------------------------------- |
| Draft             | Being prepared                              |
| Pending approval  | Waiting for one or more approver decisions  |
| Approved          | Internal approvals are complete             |
| Rejected          | Version was declined                        |
| Changes requested | Revision is required                        |
| Withdrawn         | Removed from the active approval process    |
| Sent              | Approved version was issued to the customer |

### Task statuses

| Status    | Meaning                               |
| --------- | ------------------------------------- |
| Open      | Work remains to be done               |
| Completed | Work was done and an outcome recorded |
| Cancelled | Work is no longer required            |

### Contract statuses

| Status | Meaning                                          |
| ------ | ------------------------------------------------ |
| Draft  | Signed agreement not yet uploaded/activated      |
| Active | Signed agreement uploaded and contract activated |

### Handover statuses

| Status   | Meaning                                                 |
| -------- | ------------------------------------------------------- |
| Pending  | Awaiting delivery or processing                         |
| Sent     | Delivered to the operational integration                |
| Accepted | Receiving side accepted it                              |
| Rejected | Receiving side declined it with a reason when available |
| Failed   | Delivery failed and needs controlled recovery           |

## Frequently asked questions

### Why can’t I see a menu item or button mentioned in this guide?

Your role may not include that permission, or the record may be outside your branch/region/ownership scope. Ask the administrator to review your assigned access. Some actions are also hidden when a record’s status makes them invalid.

### Why does a direct link say the record is not found?

The CRM does not reveal records outside your scope. Confirm ownership and branch with your manager or administrator.

### Can I delete a lead, account, opportunity, quote, or contract?

The current screens do not provide permanent delete actions for these business records. Use the correct business status, such as Lost, Cancelled, Disabled, or Deactivated. This keeps audit and reporting history.

### How do I create a new opportunity?

Convert a qualified lead. The current application does not have a standalone New Opportunity form.

### How do I create a task?

Tasks are currently created through workflows such as lead conversion and system reminders. The Tasks page can edit, complete, and cancel open tasks but has no general New Task button.

### Where can I see a completed or cancelled task?

Open **Tasks** and select **Completed** or **Cancelled** under Task status. Completed tasks show the recorded completion time and outcome. Select **All** to view every status together.

### Why is a lead still response-overdue after I added a note?

Only an appropriate customer-contact activity, such as Call, Email, or Meeting, records the first response. Log the activity using the actual occurred time.

### How do I merge duplicate leads?

The detail page shows suggestions, but the current screen has no Merge button. Do not convert both copies. Contact the authorized process owner.

### How do I reassign or disqualify a lead?

These actions are not exposed on the current screens. Contact an authorized administrator or workflow owner.

### Why can’t I create a quote?

The opportunity must have at least one requirement, and every attached requirement must be Approved. Also confirm that your role permits quote creation.

### Why can’t I move an opportunity to Won?

It needs an approved or sent quote. Confirm the quote status first.

### How do I revise a rejected quote?

Read the approval comments. The current screen does not provide New Version or Resubmit controls, so contact the authorized commercial process owner. Never send the rejected version.

### What is the difference between Approved and Sent?

Approved means the internal approval process is complete. Sent means that approved version was actually issued to the customer.

### Can I print or download a quote?

Use **PDF** on Quote detail if your role has access. Historical versions have separate PDFs. The Reports page itself does not have a download or print action.

### Why can’t I create a contract?

The opportunity must be Won, and the commercial evidence, contact, locations, and permissions must meet the contract rules. Contract creation is available from the won opportunity.

### Why is my contract still Draft?

Upload the final signed PDF/JPEG/PNG agreement using **Upload and activate**. The file must be accepted and within the 10 MB limit.

### How do I retry a failed handover?

The current screen has no Retry button. Contact the CRM/integration administrator. Do not create repeated handovers as a workaround.

### Where are my notifications?

There is no separate notification-inbox page yet. The bell opens Tasks. Also monitor Dashboard, contract details, and Renewals report.

### Why do my Dashboard or Report totals differ from another user’s?

You may have different ownership, branch, region, or organization scope. The totals are calculated from records each user is allowed to see.

### Does Lead export use my current filters?

No. The current export downloads leads visible to your access scope rather than only the current on-screen search/status filter, up to the export limit. Handle the file as confidential.

### Can I edit a contact or service location after saving?

The current account screen does not provide edit or delete controls for contacts or locations. Verify before saving and contact the process owner for corrections.

### How do I finish a site survey?

The current screen schedules the survey only. It does not yet provide completion, findings, checklist, or photo controls. Follow the approved interim process.

### I requested a password reset. What happens next?

Follow administrator-provided instructions. The application accepts reset requests, but a normal end-user new-password page is not currently available.

## Troubleshooting by symptom

### Sign-in problems

1. Re-enter the email carefully.
2. Check Caps Lock.
3. Confirm the correct CRM address.
4. Use Forgot your password? once if appropriate.
5. Ask whether the account is active.
6. Contact the administrator if attempts are being rate-limited.

Never send your password in email or chat.

### A page is blank or stale

1. Select Refresh when available.
2. Reload the browser page.
3. Confirm your network connection.
4. Sign out and back in if the session has expired.
5. Note the page, time, and action before contacting support.

Avoid repeatedly pressing Save while the result is unknown.

### A form will not save

1. Look for highlighted required fields.
2. Check dates: expiry must follow effective date, and required due times cannot be blank.
3. Check number ranges such as probability 0–100 and renewal notice 1–730.
4. Check that currency uses a three-letter code.
5. Confirm selected services, branches, contacts, and locations are valid.
6. Read the error message before changing data.

### CSV import has invalid rows

1. Confirm required headers and values.
2. Check `company_name`, `contact_name`, `branch_key`, and `service_keys`.
3. Use current stable keys supplied by the administrator.
4. Separate multiple service keys with semicolons.
5. Correct malformed email values.
6. Keep the file under 5 MB and 1,000 rows.
7. Preview again before importing.

### File upload fails

1. Use PDF, JPEG/JPG, or PNG for the signed agreement.
2. Keep it below 10 MB.
3. Confirm the file opens normally on your computer.
4. Do not rename an unsupported file extension.
5. If production security scanning rejects it, ask the administrator for the recorded reason.

### Data looks wrong after another user changed it

Refresh the page. If it remains wrong, compare the record’s audit or stage/version history where available. Do not overwrite correct newer information with an old browser form.

### What to include in a support request

Provide:

- your name and work email;
- page/module;
- record name or reference, without including sensitive data unnecessarily;
- date and time of the issue;
- exact action attempted;
- exact error message;
- whether Refresh or sign-in again changed the result; and
- a screenshot if company policy allows it.

Do not include your password, session information, full exported files, or customer documents unless support explicitly requests them through an approved secure channel.

## Current user-interface limitations summary

The current application does not yet provide user-facing controls for:

- lead reassignment, disqualification, or merge;
- standalone opportunity creation;
- general task creation;
- contact or location editing/deletion;
- requirement editing after creation;
- site-survey completion, findings, or photo upload;
- quote revision, withdrawal, or resubmission;
- handover accept/reject or manual retry;
- a separate notification inbox;
- normal password-reset completion;
- report export/print/date filters; or
- general attachment management.

These are documented so users do not spend time looking for controls that are not present. Follow the approved interim process or contact the appropriate administrator/process owner.

## Where to continue

- Start with [Getting started, login, and navigation](01-getting-started-login-and-navigation.md).
- Follow the whole journey in [Complete business scenarios](12-complete-business-scenarios.md).
- Return to the [documentation home page](README.md) for the full index.
