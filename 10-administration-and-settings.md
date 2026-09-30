# Administration and Settings

## Purpose of Administration

Administration controls the people, master data, organization structure, and workflow rules used throughout the CRM. Changes here can affect forms, permissions, deadlines, reports, quote approvals, and automatic lead assignment.

Only authorized administrators should use this area. Test or review high-impact changes with the business owner before saving them.

## Administration sections

The current Administration page contains areas for:

- Users
- Services
- Requirement Templates
- Pipeline stages
- Lead controls
- Structure
- Configuration
- Audit

The exact controls visible depend on permission.

## Users

### What user administration does

User records determine who can sign in, which actions they can perform, and which business records they can see.

### Adding a user

Select **Add user** and complete:

| Field                  | Meaning                                                      |
| ---------------------- | ------------------------------------------------------------ |
| First name / Last name | Employee’s correct name                                      |
| Email                  | Unique work email used for sign-in                           |
| Temporary password     | Initial password of at least 12 characters; deliver securely |
| Timezone               | User's working timezone, for example `Asia/Kolkata`          |
| Primary branch         | User’s home/responsible branch                               |
| Reporting manager      | Active manager selected from the user list, if applicable    |
| Roles                  | One or more permission groups                                |
| Visible branches       | Additional branches whose records the user may see           |
| Visible regions        | Regions whose branch records the user may see                |

The temporary password is hidden by default. Select the eye icon in the field to check what you entered, then hide it again before another person can see the screen.

### Primary branch, role, and scope

- **Primary branch** identifies the user’s main branch.
- **Role** controls the type of actions the user can perform.
- **Visible branches/regions** control which records are in the user’s scope.

These are separate. Giving a role does not automatically mean every record is visible, and adding a visible branch does not automatically grant every action.

### Editing a user

Select **Edit** beside a user to update:

- first and last name;
- sign-in email;
- timezone;
- primary branch;
- reporting manager;
- roles; and
- visible branches and regions.

The form opens with the user's current values selected. The Reporting manager field shows **Select a reporting manager** when none is assigned, and its options show each active user's name and email. A user cannot be their own reporting manager. If the current manager has become inactive, the option is identified as inactive so the administrator can replace or clear it.

The temporary password is shown only when creating a user. Use the password-reset process when an existing user's password must change.

If another administrator updated the same user first, refresh the Administration page and review the latest version before saving again.

### Activating and deactivating

The user list shows name, branch, status, and last sign-in. Select **Deactivate**, review the immediate-access warning, and confirm **Deactivate user** to remove access; active sessions end immediately. Select **Activate** to restore sign-in when appropriate.

Do not create a replacement user simply because an employee changes branch, manager, role, or scope. Select **Edit** and maintain the existing user so ownership and audit history remain connected.

## Services

### What services are

Services are the HHCIL offerings users select on leads, opportunities, requirements, quotes, contracts, and assignment rules.

### Adding a service

| Field                    | Guidance                                                               |
| ------------------------ | ---------------------------------------------------------------------- |
| Name                     | User-facing service name                                               |
| Stable key               | Permanent lowercase identifier using letters, numbers, and underscores |
| Description              | Clear explanation of the offering                                      |
| Survey normally required | Select if opportunities for this service normally need a site survey   |

Example stable key: `industrial_housekeeping`.

The stable key may be used by imports and integrations. Do not change its meaning or reuse it for a different service. The current screen can add services but does not provide general edit, archive, or toggle controls.

## Requirement templates

### What they are

A requirement template is a versioned set of service-specific questions. It ensures that users collect consistent information before quotes and handovers.

### Adding a template or version

1. Select **Add template** for a new service template, or **New version** beside an existing template.
2. For a new template, choose the Service and enter a Name.
3. Enter the **Structured definition JSON**.
4. Save and verify the resulting requirement form before live use.

This is an advanced administrator feature. The definition is structured text and must be valid. Supported field types are:

- `text`
- `textarea`
- `number`
- `date`
- `boolean`
- `select`

Example:

```json
{
  "fields": [
    {
      "key": "guard_count",
      "label": "Number of guards",
      "type": "number",
      "required": true,
      "helpText": "Enter the total across all shifts"
    },
    {
      "key": "shift",
      "label": "Primary shift",
      "type": "select",
      "required": true,
      "options": ["Day", "Night", "Both"]
    }
  ]
}
```

### Important notes

- Each new version preserves earlier approved requirement snapshots.
- Use a new version when questions change; do not repurpose an old field key to mean something else.
- Test required fields, labels, help text, and options with service specialists.
- Invalid structured text cannot produce a reliable form.

## Pipeline stages

### What stages control

Stages describe opportunity progress, provide default probabilities, determine open/closed behavior, and drive pipeline reports.

### Adding a stage

| Field       | Guidance                                                |
| ----------- | ------------------------------------------------------- |
| Name        | User-facing stage label                                 |
| Stable key  | Permanent system identifier                             |
| Order       | Position in the pipeline; smaller values appear earlier |
| Probability | Default win likelihood from 0 to 100                    |
| Closed      | Select when the stage closes the opportunity            |
| Won         | Select only for the successful closed stage             |

The configured `won` and `lost` meanings are business-critical. Do not duplicate, rename through a new conflicting key, or change closed/won behavior without technical and business review. Existing opportunity and report logic depends on these meanings.

## Lead controls

### Lead sources

Lead sources identify where enquiries came from and set a default response target.

Fields:

- Name
- Stable key
- Response target in minutes

Use realistic response targets. A website consultation may require faster action than an imported historical list.

### Loss reasons

Loss reasons standardize why a lead or opportunity did not proceed.

Fields:

- Name
- Stable key
- Applies to: Lead, Opportunity, or Both

Create categories that support useful analysis. Avoid near-duplicates such as “Too expensive” and “Price high” unless the business truly distinguishes them.

### Assignment rules

Assignment rules automatically decide how trusted website sales enquiries are routed.

| Field           | Meaning                                                       |
| --------------- | ------------------------------------------------------------- |
| Rule name       | Clear administrator label                                     |
| Priority        | Evaluation order; lower number is checked first               |
| Response target | Deadline in minutes for leads matched by the rule             |
| Service         | Optional service condition; blank means any service           |
| Source          | Optional source condition; blank means any source             |
| Branch          | Branch that receives matched leads                            |
| Specific owner  | Optional named user; blank allows the branch routing behavior |

Put narrow rules before broad fallback rules. For example, a Pune Security website rule should have a lower priority number than an Any Service Pune rule.

After a change, submit an approved test enquiry and confirm branch, owner, and response target. Assignment rules affect website intake, not every manually created record.

### Activity types

Activity types are the choices users see when logging lead interactions. Add a Name and Stable key. Typical initial values include Call, Email, Meeting, Site Survey, Internal Note, Follow-up, and Account Review.

Do not create several labels for the same activity, because inconsistent selection weakens timeline and response reporting.

## Structure: regions and branches

### Regions

Regions group branches for responsibility and visibility. Add:

- Name
- Stable key

### Branches

Branches connect users and CRM records to an HHCIL business unit. Add:

- Name
- Stable key
- Region
- Timezone

The timezone affects how business dates and deadlines are interpreted. Use the official timezone for the branch.

Stable region and branch keys can be used in CSV imports. Coordinate key changes carefully.

## Organization settings

The Configuration area includes:

| Setting           | Purpose                                                  |
| ----------------- | -------------------------------------------------------- |
| Organization name | Name displayed or used for organization identity         |
| Timezone          | Default organization timezone                            |
| Currency          | Three-letter default currency code, such as INR          |
| Number format     | Display convention such as `en-IN`, `en-US`, or `en-GB`  |
| Logo URL          | Approved image location used where branding is supported |

Use a valid three-letter currency. Number format affects how grouped numbers appear; for example, Indian grouping differs from international grouping.

## Approval policies

### What they are

Approval policies determine which roles must approve a quote, based on business conditions.

The list shows policy name, threshold, and status. Policies can be enabled or disabled.

### Adding a policy

| Field            | Guidance                                           |
| ---------------- | -------------------------------------------------- |
| Name             | Descriptive policy name                            |
| Branch           | Optional branch restriction; blank makes it global |
| Minimum amount   | Optional quote-value threshold                     |
| Maximum discount | Optional discount condition                        |
| Ordered roles    | Approver roles in serial decision order            |

Order matters. The first selected role reviews before the next. Test the policy using representative amounts and discounts before relying on it.

Disabling a policy affects future matching. The CRM asks for confirmation before disabling it. Do not use enable/disable casually while quotes are under review.

## Industries

Industry is available on account/lead-conversion forms. The initial values include Manufacturing, Healthcare, Education, Retail, Hospitality, and Other. The current Administration page does not provide an industry-management control.

## Audit history

### What it is

Audit history is a read-only record of important actions. It can show:

- time;
- actor;
- action;
- record type/reference; and
- summary.

It supports accountability and investigation. It is not a place for editing business records.

The current Audit view has no search or filter controls. Access is restricted because it can contain sensitive operational information.

## Safe administration checklist

Before saving a configuration change:

1. Identify which live forms, imports, rules, or reports use it.
2. Confirm the business owner approved the change.
3. Use a unique and stable key.
4. Avoid creating a duplicate value with different spelling.
5. Check role and scope impact.
6. Test the affected workflow with a representative record.
7. Record the decision outside the CRM if formal change approval is required.

## Related guides

- [Roles, permissions, notifications, and files](11-roles-permissions-notifications-and-files.md)
- [Complete business scenarios](12-complete-business-scenarios.md)
- [Glossary, status reference, FAQs, and troubleshooting](13-glossary-statuses-faq-and-troubleshooting.md)
