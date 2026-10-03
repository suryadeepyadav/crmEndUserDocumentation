# Roles, Permissions, Notifications, and Files

## Why access differs between users

The CRM protects customer and commercial information using roles and record visibility.

- A **role** controls which types of action a user may perform.
- **Ownership and scope** control which records the user may see or change.

These checks apply even when someone opens a direct link. Hiding a menu item is not the only protection.

## Standard roles

The descriptions below explain the intended end-user purpose of the current standard roles. Administrators may assign more than one role, so actual access can be a combination.

### System Administrator

**Purpose:** Manage the CRM configuration and access across the organization.

**Typical access:** All modules, users, master data, roles, audit history, and organization-wide records.

**Use with care:** This role can make changes affecting every user. It should be limited to designated administrators.

### Sales Executive

**Purpose:** Manage personal leads and the sales process.

**Typical work:**

- create, update, contact, and convert owned leads;
- edit or archive eligible leads, accounts, contacts, locations, and opportunities within scope;
- record activities and manage tasks;
- create requirements and surveys;
- create quotes and review permitted quote status and approval history; and
- review permitted reports.

**Typical restrictions:** No organization-wide lead assignment, sensitive lead export, commercial approval, contract administration, CRM administration, or protected quote-rate access unless an additional role grants it. Quote PDF download also requires protected-rate access.

### Branch Manager

**Purpose:** Supervise sales and customer work for assigned branches.

**Typical work:** Sales Executive activities plus branch team visibility, lead assignment authority, contracts, and branch-level oversight.

### Regional Manager

**Purpose:** Supervise work across the assigned region.

**Typical work:** Similar management activities across branches in the visible region.

### Sales Head

**Purpose:** Lead the organization-wide sales process.

**Typical work:** Broad sales visibility, sensitive exports, commercial-rate visibility, contracts, handovers, reports, and audit review.

**Typical restrictions:** User/master administration and formal quote approval are separate permissions unless another role is also assigned.

### Commercial Approver

**Purpose:** Review controlled quote versions and commercial terms.

**Typical work:** Open approval work for the approver's assigned branch and current policy step, inspect permitted quotes and rates, download PDFs when permitted, approve, request changes, or reject with comments.

This role should make decisions only within approved authority and policy.

### Account Manager

**Purpose:** Manage customer relationships after or alongside the sale.

**Typical work:** Accounts, opportunities, tasks, reports, contracts, renewals, and handovers within assigned scope.

### Operations Liaison

**Purpose:** Support post-sale handover and operational receipt.

**Typical work:** Open **Handovers**, review the permitted operations queue, accept a Pending or Sent package, optionally add its external reference, or reject it with a clear reason. Contract links require the separate account-read permission; the handover list itself is available with handover acknowledgement access.

## Multiple roles

A person can hold more than one role. For example, a Branch Manager may also be a Commercial Approver. Their allowed actions combine, but record scope still applies.

Do not assign a powerful role merely to expose one unrelated menu item. Administrators should choose the least access necessary for the person’s responsibilities.

## Ownership and visibility scope

### Owner

The owner is the person currently responsible for a lead, opportunity, account, task, contract, or related record.

### Primary branch

The user’s home branch. It often supplies the normal context for manually created work.

### Visible branches

Additional branches whose records the user may access according to their role.

### Visible regions

Regions whose branch records the user may access according to their role.

### Organization-wide scope

Certain senior or administrative roles can access all relevant organization records.

### Example

A salesperson in Pune may create and manage their own Pune leads. A Pune Branch Manager may see team records for Pune. A Regional Manager may see several branches in the West region. None should see an unrelated branch merely because they know a record link.

Commercial approval has an additional boundary: an approver sees a pending quote only when the quote is in an allowed branch and the approver's role is the role currently required by that quote's approval policy. A direct quote link does not bypass this boundary.

## What to do when access looks wrong

If a page, button, or record is missing:

1. Confirm you are signed into the correct account.
2. Check whether the item is normally part of your role.
3. Ask the record owner or manager to confirm its branch and ownership.
4. Ask the administrator to review your roles and visible branch/region scope.

Do not ask a colleague to export or download restricted information as a workaround.

Edit and Archive controls are permission-aware. Lead maintenance requires lead-update permission; account, contact, and location maintenance requires account-management permission; and opportunity maintenance requires opportunity-management permission. The API repeats these checks and also verifies ownership/branch/region scope.

## Notifications and reminders

The CRM can create internal notifications for events such as:

- lead assignment;
- task assignment or due time; and
- contract renewal timing.

Select the top-bar bell to see recent notifications and the unread count. Select a notification to mark it read and open its related page when a link is available. Users should also monitor:

- Dashboard statistics;
- Tasks filters;
- lead and account detail pages;
- contract details; and
- Renewals report.

Notifications support work management but do not replace agreed customer commitments or manager escalation procedures.

## File uploads

### Documents on lead, account, and opportunity pages

Open the **Documents** panel on a permitted lead, account, or opportunity. Choose a file, select its document category (Internal, Commercial, or Contract), then select **Upload**. Users with download access see existing files, upload time, scan status, and a download icon for cleared files. A user who is allowed to upload but not download can add a file but is not shown the existing-file list. The category describes the file; it does not itself grant access.

Accepted in the Documents panel:

- PDF, JPEG/JPG, PNG, DOCX, or XLSX;
- maximum 10 MB.

### Signed contract agreement

The contract page also accepts a signed agreement to activate a Draft contract. Accepted there:

- PDF
- JPEG/JPG
- PNG
- maximum 10 MB

Before uploading:

- confirm the document is the final signed version;
- ensure all pages are present and legible;
- remove unrelated personal information;
- use a sensible local file name; and
- follow HHCIL document-retention and confidentiality policy.

The production system may apply further file-security scanning. If a file is rejected, verify its type and size; do not disguise an unsupported file by changing its extension.

### Survey files

On an opportunity, open **Documents** on a site-survey card to add or review the survey's supporting files, including photographs, when your role has the required file permissions. Keep evidence with the survey it belongs to rather than uploading it to an unrelated account or opportunity document list.

### Current file limitations

There is no organization-wide file center. Documents remain attached to the individual lead, account, opportunity, survey, or contract context where they were added.

## Downloads and exports

### Quote PDF

Available from Quote detail only when the user has both quote-PDF download and protected commercial-rate access. Historical quote versions can have their own PDFs. Treat every PDF as commercially confidential.

### Lead CSV export

Available only with the sensitive export permission. It downloads leads matching the on-screen Lead inbox filters within your visible record scope, up to the export limit, and records the export for audit.

### Report export and printing

Users with sensitive-export permission can download the selected Reports tab as CSV using **Export current report**. The export is audited. The Reports page has no print control.

## Data handling responsibilities

- Download only when needed for an approved business purpose.
- Store files only in approved company locations.
- Do not email customer or commercial data to personal accounts.
- Do not upload executable files or unrelated archives.
- Do not share quote PDFs with users who lack commercial access.
- Report accidental disclosure using the organization’s incident process.

## Session security

- Sign out on shared computers.
- Do not share browser sessions.
- Use **Manage signed-in sessions** in the profile area to review or revoke a session you no longer trust. Revoking the current session signs you out immediately.
- An administrator can deactivate a user and immediately revoke access.
- If you believe your account is being used by someone else, sign out and contact the administrator immediately.

## Related guides

- [Getting started, login, and navigation](01-getting-started-login-and-navigation.md)
- [Quotes and approvals](07-quotes-and-approvals.md)
- [Contracts, renewals, and handovers](08-contracts-renewals-and-handovers.md)
- [Administration and settings](10-administration-and-settings.md)
