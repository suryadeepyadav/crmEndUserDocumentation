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
- work with accounts and opportunities within scope;
- record activities and manage tasks;
- create requirements and surveys;
- create quotes and access permitted PDFs;
- review permitted reports.

**Typical restrictions:** No organization-wide lead assignment, sensitive lead export, commercial approval, contract administration, or CRM administration.

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

**Typical work:** Open Approvals, inspect quotes and rates, download PDFs, approve, request changes, or reject with comments.

This role should make decisions only within approved authority and policy.

### Account Manager

**Purpose:** Manage customer relationships after or alongside the sale.

**Typical work:** Accounts, opportunities, tasks, reports, contracts, renewals, and handovers within assigned scope.

### Operations Liaison

**Purpose:** Support post-sale handover and operational receipt.

**Typical work:** Handover acknowledgement and relevant attachments where a user-facing workflow is available.

**Current interface note:** The present application does not yet expose handover accept/reject controls, and the standard navigation prerequisites may not show Contracts to an Operations Liaison alone. The administrator may need to provide an additional appropriate role or use the interim operational process.

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

## What to do when access looks wrong

If a page, button, or record is missing:

1. Confirm you are signed into the correct account.
2. Check whether the item is normally part of your role.
3. Ask the record owner or manager to confirm its branch and ownership.
4. Ask the administrator to review your roles and visible branch/region scope.

Do not ask a colleague to export or download restricted information as a workaround.

## Notifications and reminders

The CRM can create internal notifications for events such as:

- lead assignment;
- task assignment or due time; and
- contract renewal timing.

The current application does not have a separate notification-inbox page. The top-bar bell opens **Tasks**. Users should monitor:

- Dashboard statistics;
- Tasks filters;
- lead and account detail pages;
- contract details; and
- Renewals report.

Notifications support work management but do not replace agreed customer commitments or manager escalation procedures.

## File uploads

### Signed contract agreement

The current user-facing upload is the signed agreement used to activate a Draft contract.

Accepted on the current screen:

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

### Current file limitations

Although the wider CRM records can reference attachments, the current user interface does not provide a general attachment center or general attachment-download list. Site-survey photo upload is also not currently available on a screen.

## Downloads and exports

### Quote PDF

Available from Quote detail according to permission. Historical quote versions can have their own PDFs. Treat every PDF as commercially confidential.

### Lead CSV export

Available only with the sensitive export permission. It downloads visible leads and records the export for audit. The current export does not use the on-screen Lead inbox filters and can include all records within your access scope, up to the export limit.

### Report export and printing

The Reports page currently has no export or print control.

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
- An administrator can deactivate a user and immediately revoke access.
- If you believe your account is being used by someone else, sign out and contact the administrator immediately.

## Related guides

- [Getting started, login, and navigation](01-getting-started-login-and-navigation.md)
- [Quotes and approvals](07-quotes-and-approvals.md)
- [Contracts, renewals, and handovers](08-contracts-renewals-and-handovers.md)
- [Administration and settings](10-administration-and-settings.md)
