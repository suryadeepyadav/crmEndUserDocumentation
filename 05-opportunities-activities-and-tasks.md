# Opportunities, Activities, and Tasks

## What an opportunity is

An **Opportunity** is a specific potential sale being actively pursued for an account. It records the service interest, estimated value, expected close date, probability, owner, pipeline stage, and next action.

An account can have more than one opportunity. For example, an existing security customer may have a separate housekeeping expansion opportunity.

## Why and when to use Opportunities

Use an opportunity after a lead has been qualified and converted. It provides the commercial workspace for requirements, surveys, quotes, stage progress, and eventually a contract.

Create an opportunity by converting a qualified lead or by opening an existing account and selecting **New opportunity**. Use the account route when a customer has a fresh service or site request that is separate from an earlier deal.

## Pipeline page

The Pipeline page provides two views of visible opportunities.

### Kanban view

Kanban groups opportunity cards into stage columns. A card shows the account, opportunity title, value, and expected close date. Select a card to open it.

The current Kanban is for viewing; cards cannot be dragged between columns. Use **Change stage** on the opportunity page.

### Table view

The table shows:

- opportunity and account;
- current stage;
- expected value;
- expected close date; and
- owner.

Use the view toggle to switch between Kanban and table. Search and press Enter to narrow the results, or select Refresh. The current page loads up to 100 visible opportunities and has no pagination or clickable column sorting.

## Opportunity details

Open an opportunity to review:

- account and title;
- current stage and status;
- expected value and currency;
- probability;
- expected close date;
- next action and due time;
- interested services;
- requirements;
- quotes; and
- stage-change history.

Buttons available according to status and permission include **Edit**, **Change stage**, **Log activity**, **New task**, **Archive**, and an **Add** menu for Requirement, Site survey, Quote, or Contract. Contract creation is shown only after the opportunity is Won. The page also shows activities, linked tasks, and documents. Each Add-menu item is shown only when the user has the matching permission.

## Editing an opportunity

Select **Edit** and update the relevant fields.

| Field            | What it means and what to enter                         |
| ---------------- | ------------------------------------------------------- |
| Title            | Clear description of this specific potential deal       |
| Services         | One or more HHCIL services included in the opportunity  |
| Amount           | Best current estimate of total commercial value         |
| Currency         | Three-letter code such as INR                           |
| Probability      | Estimated chance of winning, from 0 to 100              |
| Expected close   | Realistic date when the commercial decision is expected |
| Next action      | The specific action needed to progress the deal         |
| Next action time | Deadline for the next action                            |

The current edit form requires a next action and next-action time. Keep them specific and current.

## Archiving an opportunity

Users with opportunity-management permission can select **Archive** for an opportunity created in error or otherwise eligible to leave the active pipeline. Enter a clear reason and confirm.

The CRM blocks archiving when the opportunity has any requirement, site survey, quote, or non-archived contract. These records are commercial evidence and must retain their opportunity connection. When archiving is allowed, the opportunity and its related task records leave active pipeline/task views, while audit history remains. There is currently no Restore button.

Do not archive a genuine unsuccessful deal. Move it to **Lost** with the correct loss reason so performance and history remain meaningful.

### Strong and weak next actions

| Weak         | Better                                                    |
| ------------ | --------------------------------------------------------- |
| Follow up    | Call Kavita to confirm the approved headcount             |
| Send details | Email revised scope and obtain written confirmation       |
| Meeting      | Conduct pricing review with the customer procurement team |

## Pipeline stages

The initial CRM configuration uses the following stages:

| Stage                  | Default probability | Meaning                                                     |
| ---------------------- | ------------------: | ----------------------------------------------------------- |
| Qualification          |                 10% | Confirming fit, need, authority, timing, and next step      |
| Requirement Collection |                 20% | Capturing service and scope information                     |
| Site Survey            |                 30% | Inspecting or planning the service location where needed    |
| Proposal Preparation   |                 40% | Building the commercial solution and quote                  |
| Internal Approval      |                 50% | Quote or commercial exception is being reviewed internally  |
| Proposal Sent          |                 60% | Approved proposal has been issued to the customer           |
| Negotiation            |                 75% | Commercial or scope terms are being discussed               |
| Won                    |                100% | Customer has agreed and the commercial evidence is complete |
| Lost                   |                  0% | Opportunity will not proceed                                |
| On Hold                |                 25% | Work is temporarily paused but not closed                   |

Administrators can configure stage names and probabilities, so follow the values shown in your application if they differ.

## Changing a stage

1. Open the opportunity.
2. Select **Change stage**.
3. Choose the **New stage**.
4. Add **Reason / context** explaining the movement.
5. If moving to Lost, select a **Loss reason** and provide clear context.
6. Save.

Each change is added to Stage history. This provides a timeline rather than replacing the previous stage without explanation.

### Rules for closed stages

- **Won:** The opportunity must have an approved or sent quote. Use Won only after the customer has accepted the commercial basis.
- **Lost:** Select a configured loss reason and enter meaningful context, such as the decision date and known cause.
- **On Hold:** Explain what is paused and when it should be reviewed.

### Example lost context

- Loss reason: Competitor selected
- Reason / context: “Customer selected an incumbent supplier on 28 September based on nationwide coverage. Revisit before next annual tender.”

Avoid vague text such as “not interested” if more accurate information is known.

## Activities versus tasks

| Record         | Purpose                                 | Example                                       |
| -------------- | --------------------------------------- | --------------------------------------------- |
| Activity       | Records something that already happened | “Called customer; staffing details received.” |
| Task/follow-up | Records work that still needs to happen | “Prepare initial staffing plan by Friday.”    |

Lead, account, and opportunity pages provide **Log activity**. Choose the activity type, actual date and time, subject, notes, and outcome. The entry remains in the related record's timeline. An account review can also be recorded on an account. Tasks remain open until completed or cancelled.

## Tasks page

The Tasks page shows current and historical work assigned to you or visible within your scope. First choose a Task status:

- **Open** — work that still needs action;
- **Completed** — finished work, including completion time and recorded outcome;
- **Cancelled** — work that was no longer required; or
- **All** — open, completed, and cancelled tasks together.

When Open is selected, use the Due date filters:

- **All open** — every open task in the current result set;
- **Today** — tasks due today;
- **Overdue** — due time has passed; and
- **Upcoming** — due after today.

The current page loads up to 100 tasks for the selected view. Open work is ordered by due time; completed work shows the most recently completed items first. The page does not offer pagination, search, or clickable column sorting.

Each task shows:

- title;
- due date and time;
- priority;
- description; and
- status.

## Task priorities

| Priority | When to use it                                                       |
| -------- | -------------------------------------------------------------------- |
| Low      | Useful work with limited time sensitivity                            |
| Normal   | Standard follow-up or planned action                                 |
| High     | Important work where delay could affect the deal or customer         |
| Urgent   | Immediate action needed to avoid serious impact or missed commitment |

Do not mark every task urgent. Priority is useful only when it distinguishes truly time-sensitive work.

## Editing a task

Select **Edit** and update:

- Title
- Description
- Priority
- Due at

Reschedule only when there is a valid new date. If a customer delays a meeting, update the due time and make the reason clear in the task description or connected notes.

## Completing a task

1. Perform the actual work.
2. Select **Complete**.
3. Enter an outcome of at least two characters.
4. Confirm.

Write an outcome that helps the next person understand the result, for example: “Customer confirmed survey for 4 October; access instructions received.”

Completed tasks leave the Open view. Select **Completed** to review the completion time and outcome, or **All** to see them together with other task statuses.

## Cancelling a task

Use **Cancel** when the task is no longer required, not when it is merely late. Review the confirmation message and select **Cancel task** to continue, or **Go back** to keep it open. A cancelled task leaves the Open view but remains available under Cancelled and All.

## Creating a task

Select **New task** on Tasks or from a lead, account, or opportunity. Enter a clear title, an optional description, an assignee, priority, and due date/time. From Tasks, you can also choose a visible linked record; from a detail page, the current record is preselected. Sales executives can assign to themselves; managers can select eligible users in their managed scope. The assignee receives an in-app notification and the due time schedules a reminder.

Lead conversion also creates its first follow-up task from the opportunity's next action. When that action is done, record the outcome and create the next task if more work is needed.

## Real-world example

After converting the Northstar lead:

- Opportunity: Pune plants housekeeping FY27
- Stage: Qualification
- Amount: ₹18,00,000
- Probability: 10%
- Expected close: 30 November
- Next action: Collect site-wise staffing and shift details
- Next action due: 3 October, 4:00 PM

The follow-up appears in Tasks. After the customer supplies the details, complete the task with the outcome and move the opportunity to Requirement Collection.

## Important notes

- Opportunity amount is an estimate until commercial terms are agreed.
- Probability is not a guarantee; it helps calculate weighted pipeline.
- Keep expected close dates realistic so forecasts are useful.
- Never move a deal to Won simply to improve a report.
- Stage history and task outcomes should explain what changed and why.

## Related guides

- [Leads and CSV import/export](03-leads-and-import-export.md)
- [Requirements and site surveys](06-requirements-and-site-surveys.md)
- [Quotes and approvals](07-quotes-and-approvals.md)
- [Reports and analytics](09-reports-and-analytics.md)
