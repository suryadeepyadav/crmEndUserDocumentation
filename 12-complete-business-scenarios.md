# Complete Business Scenarios

These scenarios show how the modules connect. The names and values are fictional; follow your organization’s approved process and live CRM configuration.

## Scenario 1 — Manual enquiry to active contract

### Situation

Kavita Rao from Northstar Textiles contacts the Pune branch about housekeeping at two plants.

### Step 1: Create the lead

The Sales Executive opens Lead inbox and selects **Create lead**.

- Company: Northstar Textiles Pvt Ltd
- Contact: Kavita Rao
- Service: Housekeeping
- Source: Manual Entry
- Branch: Pune
- City: Pune
- Notes: Two plants, approximately 60 workers, desired start in January

The CRM assigns the lead to the creator and calculates its response target.

### Step 2: Record the first response

After speaking with Kavita, the salesperson logs a **Call**:

- Subject: Initial requirement call
- Notes: Need site-wise staffing, shifts, and area details
- Outcome: Requirement discussion scheduled

The first-contact time is recorded and the lead becomes Contacted.

### Step 3: Check duplicates and convert

The salesperson reviews possible duplicates. Finding none, they select **Convert lead** and enter:

- Legal account name: Northstar Textiles Private Limited
- Trade name: Northstar Textiles
- Industry: Manufacturing
- Opportunity title: Pune plants housekeeping FY27
- Expected close: 30 November
- Indicative amount: ₹18,00,000
- Next action: Collect site-wise staffing and shift details
- Next action due: 3 October, 4:00 PM

The CRM creates the Account, Contact, Opportunity, and follow-up task together.

### Step 4: Complete the account

On the Account page, the salesperson:

- confirms Kavita’s contact role and marks her as Sales and Operations;
- adds Pune Plant 1 and Pune Plant 2 as separate locations; and
- records any account review discussion.

### Step 5: Collect requirements

On the Opportunity page, the salesperson adds a Housekeeping requirement, selects the current template, and enters:

- anticipated start date;
- service scale;
- shift details;
- customer responsibilities;
- special access or safety instructions.

After checking every value, they select **Freeze & approve**.

### Step 6: Schedule the site survey

The salesperson adds a Site survey for Pune Plant 1 with visit time and preparation notes. The current application records the schedule; the team follows the interim approved process for survey findings because completion/photo screens are not yet available.

### Step 7: Create and approve the quote

With every requirement approved, the salesperson adds a quote:

- recurring monthly service line;
- one-time mobilization line;
- tax and any authorized discount;
- payment terms;
- assumptions and exclusions;
- validity date.

They review the PDF and submit it. The commercial approver reviews the exact version and approves with comments. The salesperson sends that approved PDF to the customer and selects **Mark sent**.

### Step 8: Close as won

After customer acceptance, the salesperson uses **Change stage** and selects Won. This is allowed because approved/sent commercial evidence exists.

### Step 9: Create and activate the contract

From the won opportunity, the account manager adds a contract with:

- unique reference;
- effective and expiry dates;
- Kavita as operational contact;
- both Pune locations; and
- a 90-day renewal notice.

The record starts as Draft. The account manager uploads the final signed PDF, and the contract becomes Active.

### Step 10: Handover and renewal

The account manager verifies the commercial basis, scope, sites, contact, and approved requirement snapshots, then creates the handover. The status is monitored for Sent, Accepted, Rejected, or Failed.

Before the calculated renewal reminder date, the account manager opens the Renewals report and begins the account review.

## Scenario 2 — Website enquiry and response deadline

### Situation

A visitor submits a service enquiry through the connected HHCIL website.

### Workflow

1. The CRM validates the trusted website request.
2. Spam and repeated submissions are checked.
3. The matching assignment rule selects the branch, optional owner, and response target.
4. The lead appears in the appropriate Lead inbox.
5. The owner checks Dashboard and Response overdue.
6. The owner contacts the customer and logs a Call, Email, or Meeting.
7. The lead continues through qualification and conversion.

Repeated website submissions using the same request identity are designed to create one business result rather than duplicate leads.

Website job enquiries are routed outside the B2B sales-lead workflow. A user should not recreate a job enquiry as a sales lead unless an authorized business review confirms it is actually a service enquiry.

## Scenario 3 — Controlled CSV lead import

### Situation

A branch has 250 validated leads from an approved event spreadsheet.

### Workflow

1. The branch user obtains current service and branch stable keys from the administrator.
2. They prepare the required CSV columns and remove exact duplicates.
3. They select **Import CSV** and preview the file.
4. The preview reports valid, possible duplicate, and invalid rows.
5. They correct invalid branch keys and malformed emails in the source file.
6. They preview again and import valid rows.
7. Possible duplicates are reviewed individually and not automatically imported.
8. Imported records are assigned to the signed-in user.

The user does not repeatedly import the same file to “see what happens,” because that creates avoidable review work even when duplicate controls exist.

## Scenario 4 — Opportunity is lost

### Situation

The customer selects an incumbent national vendor.

### Workflow

1. The owner completes or cancels outstanding follow-up tasks appropriately.
2. They open the opportunity and select **Change stage**.
3. They select Lost.
4. They choose the configured loss reason, such as Competitor selected.
5. They enter context: decision date, known reason, and possible future revisit.
6. The CRM adds the change to stage history and the deal appears in lost performance.

The user does not delete the account or opportunity. The history is useful for reporting and future relationship work.

## Scenario 5 — Approver requests quote changes

### Situation

The quote includes mobilization inside a recurring line, but policy requires it to be shown separately.

### Workflow

1. The approver opens Approvals and reviews the quote PDF.
2. They select **Changes**.
3. They enter: “Separate mobilization as a one-time line and confirm 30-day validity.”
4. The decision is retained in approval history.
5. The salesperson does not send the current version.
6. Because the current user interface does not provide New version or Resubmit controls, the salesperson contacts the authorized commercial process owner to arrange the controlled revision.
7. The corrected version must complete required approval before it is sent.

## Scenario 6 — Contract amendment and renewal planning

### Situation

An active contract is formally extended by six months.

### Workflow

1. The account manager obtains the approved amendment evidence.
2. They open the contract and add an Amendment.
3. Reason: Six-month extension approved.
4. They enter the new expiry date and agreed renewal-notice days.
5. They record approved change notes.
6. The CRM preserves the previous snapshot and recalculates renewal timing.
7. The manager later monitors the new reminder in Renewals report.

Saving the CRM amendment does not replace signed legal documentation.

## Scenario 7 — Failed handover

### Situation

An Active contract handover shows Failed.

### Workflow

1. The user opens the contract and checks the handover status and available error information.
2. They verify the contract, service locations, operational contact, and approved requirement data.
3. They contact the CRM/integration administrator with the contract reference and handover status.
4. The administrator uses the controlled retry or reconciliation process.
5. The user refreshes the contract later and confirms the updated status.

The user does not create several new handovers as a retry. This protects the receiving system from duplicate operational sites.

## Scenario 8 — New employee access setup

### Situation

A new Sales Executive joins the Pune branch.

### Workflow

1. The administrator creates a user with work email and a secure temporary password.
2. Primary branch is set to Pune.
3. Sales Executive role is assigned.
4. Only required visible branches or regions are selected.
5. The reporting manager is assigned.
6. The employee signs in and confirms Lead inbox, Accounts, Pipeline, Tasks, and Reports access expected for the role.
7. The employee cannot see unrelated branch records.

If the employee later leaves, the administrator deactivates the user. Existing sessions are revoked immediately, while historical actions remain available for audit.

## Scenario 9 — Daily salesperson routine

1. Open Dashboard.
2. Handle Response overdue.
3. Review New leads.
4. Complete or reschedule Overdue tasks with accurate outcomes.
5. Plan Today tasks.
6. Update opportunity next actions and stages after customer events.
7. Check pending requirement, quote, or approval work.
8. Review high-value or stalled Kanban cards.
9. Sign out when finished on a shared device.

## Scenario 10 — Weekly manager review

1. Review overdue lead response by branch/team.
2. Review Pipeline by stage and owner.
3. Inspect opportunities with old stages or unrealistic close dates.
4. Review Lead cohorts for response and conversion trends.
5. Review Won/Lost performance and loss context.
6. Review Renewals and assign account actions.
7. Check account expansion opportunities.
8. Resolve access, assignment, and data-quality problems through the correct administrative process.
