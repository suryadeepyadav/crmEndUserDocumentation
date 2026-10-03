# Requirements and Site Surveys

## Service requirements

### What a requirement is

A **Requirement** records what the customer needs for one service in an opportunity. It combines common planning information with service-specific questions supplied by a requirement template.

Requirements provide a controlled basis for pricing, quote approval, and later handover. If an opportunity covers several services, create a requirement for each service as needed.

### Why and when to use it

Create requirements after qualification and before preparing a quote. Use them to replace informal, incomplete notes with a clear service scope.

Do not approve a requirement while key facts are still uncertain. Once approved, its snapshot is treated as the agreed basis for later work.

## Creating a requirement

1. Open the opportunity.
2. Open **Add** and select **Requirement**.
3. Choose a **Service** from the services already attached to the opportunity.
4. Choose a **Requirement template** if an appropriate one is available.
5. Complete the common and template-specific fields.
6. Save.

### Common fields

| Field                   | Guidance                                                                    |
| ----------------------- | --------------------------------------------------------------------------- |
| Service                 | The service whose scope is being recorded; required                         |
| Requirement template    | The approved question set for that service; optional if none applies        |
| Anticipated start       | Expected service start date, when known                                     |
| Anticipated end         | Expected end date for fixed-duration work, when applicable                  |
| Expected volume / scale | Quantified size, such as number of guards, square footage, shifts, or sites |
| Special instructions    | Constraints, certifications, timing, access, or customer-specific needs     |

If no template is selected, the common fields can still be saved. However, use a suitable template when one exists so that required information is collected consistently.

### Template-specific fields

The questions depend on the service and template version. A question may be:

- a short text field;
- a longer text area;
- a number;
- a date;
- a Yes/No checkbox; or
- a selection from approved options.

Required questions must be completed. Help text below a field explains any special expectation.

### Example

For a security requirement at a manufacturing plant:

- Expected volume / scale: “3 gates, 2 shifts, 12 guards plus 2 supervisors”
- Anticipated start: 1 January
- Special instructions: “All guards require customer safety induction; night-shift transport to be included.”
- Template answers: number of gates, shift pattern, visitor volume, patrol requirement, and control-room availability

## Requirement statuses

| Status   | Meaning                                                                     |
| -------- | --------------------------------------------------------------------------- |
| Draft    | Information has been saved but can still be reviewed before approval.       |
| Approved | The CRM has frozen an approved snapshot for commercial and operational use. |

## Freezing and approving a requirement

1. Review the requirement card on the opportunity.
2. Confirm that dates, quantities, and service-specific answers are complete.
3. Select **Freeze & approve**.
4. Read the immutable-snapshot warning and select **Freeze & approve** again to confirm, or **Go back** to review the requirement.

Approval creates an immutable snapshot so later quote and handover records can point to the exact information that was approved. Treat this as a business approval, not a draft-save shortcut.

Before approval, select **Edit** on the requirement card to correct its service, dates, scale, instructions, or template answers. Save the draft, review it again, and then approve it. Approved requirements cannot be edited; a new approved scope needs the organization's change process.

## Requirement gates for quotes

Before a quote can be created:

- every requirement already attached to the opportunity must be approved.

Use a requirement whenever the scope or price needs a controlled record. If one has been added and remains Draft, complete and approve it before creating the quote. Your commercial process may require a requirement even where the screen does not prevent an otherwise valid quote from being started.

## Site surveys

### What a site survey is

A **Site survey** is a planned visit to a customer location to inspect conditions, confirm scope, or collect details needed for service design and pricing.

### Why and when to use it

Schedule a survey when the physical location materially affects staffing, equipment, safety, access, logistics, or price. Not every opportunity requires a survey.

### Before scheduling

The account must have at least one service location. If no location is available:

1. open the connected account;
2. add the service location; and
3. return to the opportunity.

### Scheduling a site survey

1. Open the opportunity.
2. Open **Add** and select **Site survey**.
3. Choose the **Location**.
4. Choose **Assign survey to**.
5. Set the **Visit date/time**.
6. Enter **Preparation notes**.
7. Save.

| Field             | Guidance                                                                                                          |
| ----------------- | ----------------------------------------------------------------------------------------------------------------- |
| Location          | Exact account site to be visited; required                                                                        |
| Assign survey to  | The eligible user responsible for the visit. The list is limited to users you are allowed to assign; required.   |
| Visit date/time   | Confirmed or agreed appointment time; required                                                                    |
| Preparation notes | Access rules, people to meet, documents to carry, PPE, questions, or other preparation                            |

The form initially selects the opportunity owner when that person is eligible. Change it when another eligible colleague will perform the visit. The survey card then shows the assigned person. The location must belong to the opportunity's account.

Each new survey starts with a five-item checklist covering access and safety, scope, measurements or headcount, constraints, and follow-up actions.

### Example

- Location: Pune Plant 1
- Visit date/time: 4 October, 10:30 AM
- Preparation notes: “Meet Kavita at Gate 2. Carry photo ID and safety shoes. Measure all common areas and confirm three-shift occupancy.”

## Completing a survey and adding evidence

1. On the opportunity, find the survey under **Site surveys**.
2. Select **Complete** after the visit. Enter a result for every checklist item; use the notes field for findings and follow-up details.
3. Save. The status changes from **Scheduled** to **Completed** and the completion time is recorded. A completed survey cannot be completed again.
4. Select **Documents** to add or review survey photographs and supporting files, if your role has file access.

The opportunity page is the survey list for that opportunity; there is no separate all-surveys menu. Scheduling alone does not mark a survey complete. Upload files to the correct survey, and never use a checklist result merely to hide an unresolved finding.

### Creating follow-up work from a survey

Use **Follow-up** on a survey card when the visit creates work for someone to do later, such as confirming a measurement, obtaining a safety document, or arranging a second visit.

1. Select **Follow-up** on the relevant survey.
2. The standard task form opens with a title beginning `Survey follow-up:` and the current opportunity already linked.
3. Confirm or change the title, choose an eligible assignee, priority, and due date/time, then add useful details.
4. Save the task.

The task appears in the opportunity's **Follow-up tasks** list and follows the usual task reminder and notification process. The button is visible only to users who can manage activities and tasks. Record the survey finding in the survey itself as well; the task is the action to take afterwards.

## Related features

- The opportunity determines which services can be selected.
- Account locations provide the survey venue.
- Any requirements saved against the opportunity must be approved before quote creation.
- Approved requirement snapshots later support contract handover.
- Administrators create and version requirement templates.

## Important notes

- Use quantities and units, not vague terms such as “large site.”
- Record assumptions clearly when facts are not final.
- Verify dates against customer confirmation.
- Approval is permanent evidence of what was known at that point.
- Do not use one service’s template for another service merely to continue the workflow.
