# Reports and Analytics

## What Reports are for

Reports turn visible CRM records into management views for pipeline, response, performance, renewals, and account growth. They are operational decision tools, not accounting statements.

Every report is permission- and scope-aware. A salesperson, branch manager, regional manager, and sales head may see different totals on the same tab.

## Opening Reports

Select **Reports** from navigation. If the item is missing, your role does not currently have report access.

The current report page provides five tabs:

- Pipeline
- Lead cohorts
- Performance
- Renewals
- Account expansion

The page currently has no date/branch filters, CSV export, print control, pagination, or clickable sorting. The results reflect the report’s built-in rules and your current access scope.

## Pipeline report

### What it shows

The Pipeline report groups opportunities by stage and owner.

| Column   | Meaning                                |
| -------- | -------------------------------------- |
| Stage    | Current opportunity stage              |
| Owner    | User responsible for the opportunity   |
| Count    | Number of opportunities in the group   |
| Amount   | Combined unweighted opportunity value  |
| Weighted | Combined value adjusted by probability |

### Weighted pipeline

Weighted value estimates risk-adjusted pipeline:

```text
Opportunity amount × probability percentage
```

An opportunity worth ₹10,00,000 at 40% contributes ₹4,00,000 to weighted pipeline.

### Why and when to use it

Use the report for stage balance, owner workload, and forecast discussion. Do not treat weighted value as committed revenue.

### Example interpretation

If one owner has most opportunities in Qualification and none in Proposal Sent, review whether leads are progressing or whether stage updates are missing.

## Lead cohorts report

### What it shows

Lead cohorts group leads by the month they were received, for up to the report’s recent history window.

| Column                 | Meaning                                                               |
| ---------------------- | --------------------------------------------------------------------- |
| Received month         | Month in which the leads entered the CRM                              |
| Received               | Number of leads received in that cohort                               |
| Converted              | Number currently converted from that cohort                           |
| Average first response | Average time between lead receipt and first recorded customer contact |

### Why and when to use it

Use it to compare intake quality, conversion, and response speed across months. The converted number is based on current lead status. A recent month may look weaker simply because its leads have not had enough time to mature.

### Important first-response rule

The first Call, Email, or Meeting records customer contact. Internal notes do not count. Accurate activity types are therefore essential to this report.

## Performance report

### What it shows

Performance groups opportunity outcomes by region/branch and owner.

| Column        | Meaning                                     |
| ------------- | ------------------------------------------- |
| Region/branch | Organization area connected to the records  |
| Owner         | Responsible CRM user                        |
| Won           | Number of won opportunities                 |
| Lost          | Number of lost opportunities                |
| Won value     | Combined amount of won opportunities        |
| Open value    | Combined amount of opportunities not closed |

### Why and when to use it

Use it for team coaching, pipeline reviews, and outcome analysis. Interpret it with context: a new territory, a few unusually large deals, or missing stage updates can materially affect the totals.

## Renewals report

### What it shows

| Column   | Meaning                                               |
| -------- | ----------------------------------------------------- |
| Contract | Contract reference                                    |
| Account  | Customer organization                                 |
| Reminder | Calculated date to begin renewal work                 |
| Expiry   | Contract end date                                     |
| Status   | Current contract or renewal state shown by the report |

### Why and when to use it

Account managers should review this tab regularly to begin renewal work before the reminder date. The reminder is calculated from the expiry date and renewal-notice days stored on the contract.

## Account expansion report

### What it shows

This report highlights sales activity by account.

| Column        | Meaning                                     |
| ------------- | ------------------------------------------- |
| Account       | Customer organization                       |
| Branch        | Responsible branch                          |
| Opportunities | Total opportunity count                     |
| Won           | Won opportunity count or value as displayed |
| Open          | Open opportunity count                      |
| Open pipeline | Combined value of open opportunities        |

### Why and when to use it

Use it to identify customers with active expansion potential, accounts with only one service, or accounts whose open opportunities need follow-up.

## Recommended management workflow

1. Review Dashboard for immediate work.
2. Use Pipeline report for stage and owner balance.
3. Use Lead cohorts for response and conversion trends.
4. Use Performance for branch/region and won/lost review.
5. Use Renewals to plan account actions.
6. Use Account expansion to identify cross-service opportunities.
7. Open the underlying account, opportunity, or contract before acting on an unusual number.

## Data-quality responsibilities

Reports are only as reliable as the records behind them. Users should keep these fields current:

- lead status and first customer contact;
- opportunity owner, amount, probability, stage, and expected close;
- loss reason and context;
- contract dates and renewal notice days; and
- account and branch relationships.

## Common questions

**Why do my totals differ from my manager’s?**  
The manager may have access to more branches, users, or records.

**Why is report value different from finance revenue?**  
CRM reports use opportunity and contract records. They are not invoices, collections, or recognized revenue.

**Why does a won deal still appear incorrectly?**  
Open the opportunity and verify its stage and amount. Also check whether you are reading Won value or Open value.

**Can I export or print a report?**  
The current Reports page has no export or print action. Do not use the Leads export as a substitute for report data.

**Can I choose a custom date range?**  
The current page does not have report date filters.

## Related guides

- [Dashboard](02-dashboard.md)
- [Opportunities, activities, and tasks](05-opportunities-activities-and-tasks.md)
- [Contracts, renewals, and handovers](08-contracts-renewals-and-handovers.md)
- [Roles, permissions, notifications, and files](11-roles-permissions-notifications-and-files.md)
