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
| Archive              | Remove an eligible record from normal active views without permanently deleting its stored audit history            |

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
| Superseded        | Historical pending version was replaced by newer current work |
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

### Can I permanently delete a lead, account, contact, location, opportunity, quote, or contract?

The screens do not permanently delete these business records. Authorized users can archive an eligible lead, account, contact, location, or opportunity after entering a reason. Dependency checks prevent archiving records that must be retained for contracts, surveys, requirements, or quotes. Quotes and contracts do not have an Archive action on the current screens.

Use the correct business status whenever one applies, such as Lost, Cancelled, Disabled, or Deactivated. There is currently no archived-record list or Restore button.

### How do I create a new opportunity?

For a new prospect, record a Call, Email, or Meeting against the lead, mark it qualified, then select **Convert lead**. For an existing customer, open the Account page and select **New opportunity**. Both paths create an opportunity linked to an account.

### Why canâ€™t I mark a lead as qualified?

Only a Contacted lead can be qualified. Record a customer Call, Email, or Meeting first, then
return to the lead detail page. The button is also hidden if you do not have lead-update permission
or cannot access the lead.

### How do I create a task?

Select **New task** on Tasks, or on a permitted lead, account, or opportunity. Enter the title, assignee, priority, and due time; optionally add details and a linked record. Lead conversion also creates an initial follow-up task automatically.

### Where can I see a completed or cancelled task?

Open **Tasks** and select **Completed** or **Cancelled** under Task status. Completed tasks show the recorded completion time and outcome. Select **All** to view every status together.

### Why is a lead still response-overdue after I added a note?

Only an appropriate customer-contact activity, such as Call, Email, or Meeting, records the first response. Log the activity using the actual occurred time.

### How do I merge duplicate leads?

Open the duplicate lead that should be closed, select **Merge duplicate**, choose the surviving lead, enter a reason, and confirm. Review the two records first; activities, tasks, and services from the closed lead move to the survivor.

### How do I reassign a lead?

If your role has lead-assignment permission, open the lead and select **Reassign lead**. Choose an allowed branch, an active user belonging to that branch, a response deadline, and a clear reason. If the button is missing, ask a Branch Manager, Regional Manager, Sales Head, or System Administrator to perform the reassignment.

### How do I disqualify a lead?

Open the lead, select **Disqualify**, choose the appropriate reason, add notes if helpful, and confirm. The lead stays in history with Disqualified status. Use **Merge duplicate** instead for a confirmed duplicate.

### Why can’t I create a quote?

Every requirement already attached to the opportunity must be Approved. Also confirm that your role permits quote creation. Use a requirement whenever the service scope or price needs controlled sign-off.

### Why can’t I move an opportunity to Won?

It needs an approved or sent quote. Confirm the quote status first.

### How do I revise a rejected quote?

Read the approval comments, then open the current quote. Select **New version** when commercial details must change, save the new Draft, and submit it for approval. If the exact same current version should be reviewed again, the original submitter (or a System Administrator) can select **Resubmit** in **Approval history** and enter a reason. Never send the rejected version.

### What is the difference between Approved and Sent?

Approved means the internal approval process is complete. Sent means that approved version was actually issued to the customer.

### Can I print or download a quote?

Use **PDF** on Quote detail only when your role has both quote-PDF download and protected commercial-rate access. Historical versions have separate PDFs for authorized users. Users with sensitive-export permission can download the selected Reports tab as CSV; the page does not have a print action.

### Why can’t I create a contract?

The opportunity must be Won, and the commercial evidence, contact, locations, and permissions must meet the contract rules. Contract creation is available from the won opportunity.

### Why is my contract still Draft?

Upload the final signed PDF/JPEG/PNG agreement using **Upload and activate**. The file must be accepted and within the 10 MB limit.

### How do I retry a failed handover?

Users with handover-management access can open **Handovers** and select **Retry** for an eligible
Failed or Rejected package. The same package is retried with its existing reference. If the button
is unavailable, contact the CRM/integration administrator. Do not create repeated handovers as a
workaround.

### Where are my notifications?

Select the bell in the top bar. It shows recent notifications and an unread count. Select an item to mark it read and open its related page when available. Also monitor Dashboard, Tasks, contract details, and Renewals report.

### Why do my Dashboard or Report totals differ from another user’s?

You may have different ownership, branch, region, or organization scope. The totals are calculated from records each user is allowed to see.

### Does Lead export use my current filters?

Yes. It applies your current Lead inbox filters within your permitted record scope, up to the export limit. Review those filters before downloading and handle the file as confidential.

### Can I edit a contact or service location after saving?

Yes, if your role has account-management permission and the account is within your scope. Open the account and use the pencil icon beside the contact or location. Use the Archive icon only when the record should leave active views; contacts and locations still used by contracts, surveys, or active site relationships cannot be archived.

### Why was Archive rejected?

Read the message in the confirmation dialog. The record may have been changed by another user, may be outside your permitted scope, or may still be required by another record. Common examples are an account with an opportunity or contract, a contact used by a contract/location, a location used by a contract/survey, or an opportunity with requirements, surveys, quotes, or a contract. Refresh before retrying and preserve the dependent history.

### How do I finish a site survey?

Open the opportunity and find the survey under **Site surveys**. Select **Complete**, record a result for each checklist item and the visit findings, then save. Use **Documents** on the survey card for supporting files when permitted. Select **Follow-up** to create a task for any action that must happen after the visit.

### Why is a pending quote missing from my Approvals inbox?

The inbox shows only work for a branch you are allowed to access when your role is the role required by the current approval step. Another approver may be responsible for an earlier or later serial step. Ask the commercial process owner to confirm the policy and your branch scope; do not use another person's account.

### Why can I see a quote but not its amount or PDF?

Quote status and approval history can be visible without protected commercial-rate access. Rates, discounts, taxes, totals, and the PDF are intentionally hidden unless the role includes the required commercial permissions. Ask the administrator or commercial access owner to review your access if your work genuinely requires it.

### I forgot my password. What should I do?

Contact your administrator or reporting manager. The Forgot password link is intentionally hidden from the sign-in screen.

## Troubleshooting by symptom

### Sign-in problems

1. Re-enter the email carefully.
2. Check Caps Lock.
3. Confirm the correct CRM address.
4. Ask whether the account is active.
5. Contact the administrator if attempts are being rate-limited or you need password help.

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

- editing an already approved requirement;
- self-service password recovery;
- report print/date filters; or
- an organization-wide attachment center.

These are documented so users do not spend time looking for controls that are not present. Follow the approved interim process or contact the appropriate administrator/process owner.

## Where to continue

- Start with [Getting started, login, and navigation](01-getting-started-login-and-navigation.md).
- Follow the whole journey in [Complete business scenarios](12-complete-business-scenarios.md).
- Return to the [documentation home page](README.md) for the full index.
