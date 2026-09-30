# HHCIL CRM User Guide

Welcome to the user guide for the HHCIL Customer Relationship Management (CRM) application. This guide explains the application as it works today: the screens users can open, the information they can enter, the actions available to each role, and the business process that connects leads, opportunities, quotes, contracts, and handovers.

## What the CRM is for

The CRM gives HHCIL one place to manage the commercial journey from a new enquiry through ongoing account management. It helps teams:

- capture enquiries and respond on time;
- keep customer, contact, and service-location information together;
- qualify leads and build a sales pipeline;
- collect service requirements and schedule site surveys;
- prepare, approve, send, and retain versions of commercial quotes;
- activate contracts and track renewal dates;
- prepare operational handovers; and
- review performance using permission-aware reports.

The application also records important actions in an audit trail. What each person can see and do depends on their assigned role, branch, region, and record ownership.

## Who should use this guide

This guide is intended for:

- sales executives managing leads and opportunities;
- branch and regional managers supervising their teams;
- sales leaders reviewing organization-wide performance;
- commercial approvers reviewing quotes;
- account managers managing contracts and renewals;
- operations users involved in handovers; and
- administrators maintaining users, services, stages, and business rules.

If a page or button in this guide is not visible to you, your account probably does not have the required permission or record scope. Ask your CRM administrator or reporting manager before assuming the feature is unavailable.

## Main features

- Dashboard with lead, task, and pipeline summaries
- Lead capture, editing, safe archiving, website intake, duplicate suggestions, CSV import, and CSV export
- Account, contact, location, and account-review records with permission-controlled maintenance
- Opportunity pipeline in table and Kanban views, including editing, stage changes, and safe archiving
- Activities, follow-up tasks, priorities, and due dates
- Service requirement forms and approved requirement snapshots
- Site-survey scheduling
- Versioned quotes, calculated totals, approval steps, and PDF downloads
- Contracts, signed-agreement upload, amendments, renewals, and handovers
- Pipeline, conversion, performance, renewal, and account-expansion reports
- Administration for users, roles, branches, regions, services, templates, and workflow rules

## Recommended starting point

If you are new to the CRM, read these first:

1. [Getting started, login, and navigation](01-getting-started-login-and-navigation.md)
2. [Dashboard](02-dashboard.md)
3. [Leads and CSV import/export](03-leads-and-import-export.md)
4. The guide for your role's main area, such as opportunities, approvals, or administration
5. [Complete business scenarios](12-complete-business-scenarios.md)
6. [Glossary, status reference, FAQs, and troubleshooting](13-glossary-statuses-faq-and-troubleshooting.md)

## Documentation index

| Guide                                                                                                         | What it covers                                                                                              |
| ------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------- |
| [01 — Getting started, login, and navigation](01-getting-started-login-and-navigation.md)                     | Signing in, password help, menus, sessions, navigation, and common page behavior                            |
| [02 — Dashboard](02-dashboard.md)                                                                             | Dashboard statistics, pipeline summary, overdue work, and daily usage                                       |
| [03 — Leads and CSV import/export](03-leads-and-import-export.md)                                             | Lead creation, fields, response targets, activities, duplicates, conversion, import, and export             |
| [04 — Accounts, contacts, and locations](04-accounts-contacts-and-locations.md)                               | Customer organizations, people, service locations, reviews, and account maintenance                         |
| [05 — Opportunities, activities, and tasks](05-opportunities-activities-and-tasks.md)                         | Pipeline views, stages, values, next actions, loss handling, follow-ups, and task completion                |
| [06 — Requirements and site surveys](06-requirements-and-site-surveys.md)                                     | Service requirement forms, templates, approval snapshots, and survey scheduling                             |
| [07 — Quotes and approvals](07-quotes-and-approvals.md)                                                       | Quote lines, totals, statuses, approval decisions, sending, versions, and PDFs                              |
| [08 — Contracts, renewals, and handovers](08-contracts-renewals-and-handovers.md)                             | Contract creation, activation, amendments, renewal dates, and operational handovers                         |
| [09 — Reports and analytics](09-reports-and-analytics.md)                                                     | Pipeline, lead cohorts, won/lost performance, renewals, and account expansion                               |
| [10 — Administration and settings](10-administration-and-settings.md)                                         | Users, services, templates, stages, lead rules, branches, regions, organization settings, and audit history |
| [11 — Roles, permissions, notifications, and files](11-roles-permissions-notifications-and-files.md)          | What each role normally does, visibility boundaries, alerts, uploads, downloads, and restricted actions     |
| [12 — Complete business scenarios](12-complete-business-scenarios.md)                                         | End-to-end examples showing how modules connect                                                             |
| [13 — Glossary, status reference, FAQs, and troubleshooting](13-glossary-statuses-faq-and-troubleshooting.md) | Plain-language terminology, status meanings, common questions, and problem solving                          |

## Complete CRM workflow at a glance

```text
New enquiry
   ↓
Lead is assigned and given a response target
   ↓
Salesperson records contact and follow-up
   ↓
Lead is qualified and converted
   ↓
Account + Contact + Opportunity + Follow-up are created together
   ↓
Requirements are collected and approved
   ↓
Site survey is scheduled when needed
   ↓
Quote is prepared → approved → marked sent
   ↓
Opportunity is moved to Won
   ↓
Contract is created → signed agreement uploaded → contract activated
   ↓
Operational handover is prepared and sent
   ↓
Account reviews, amendments, and renewal reminders continue
```

Not every deal needs every middle step. For example, a survey is normally used when the service or location must be inspected before pricing. The CRM still enforces important commercial gates: all saved requirements must be approved before a quote is created, and an opportunity cannot be marked **Won** without an approved or sent quote.

## Important current-application notes

This guide describes only user-facing behavior that currently exists. In the present application:

- opportunities are created by converting a lead; there is no separate **New opportunity** form;
- lead reassignment, merge, and disqualification are supported by the wider system but do not yet have buttons on the current screens;
- authorized users can archive leads, accounts, contacts, locations, and eligible opportunities, but there is no restore screen or permanent-delete action;
- site surveys can be scheduled, but there is not yet a screen for completing the checklist or uploading survey findings;
- tasks can be edited, cancelled, and completed, but there is no general **New task** button;
- quote revisions and resubmission after rejection do not yet have a user-facing button;
- handover acknowledgement and manual retry do not yet have user-facing controls;
- the bell icon opens Tasks; there is not yet a separate notification inbox; and
- password-reset requests can be submitted, but there is not yet a normal end-user page for choosing a new password from the reset link.

Where one of these cases affects your work, contact your CRM administrator or process owner.

## How to use the examples

Examples use fictional organizations and values. Replace them with verified customer information. Do not enter placeholder information into real records simply to bypass a required field. Required information is part of the business record and may later appear in quotes, contracts, reports, or handovers.
