# Contracts, Renewals, and Handovers

## What a contract is

A **Contract** is the controlled record of an agreed customer service after an opportunity is won. It connects the commercial basis to the service dates, customer operational contact, service locations, signed agreement, renewal reminder, amendments, and operational handovers.

The CRM contract record supports the business process; it does not replace legal review or the signed document.

## Why and when to use Contracts

Create a contract when:

- the opportunity is in the Won stage;
- the approved commercial evidence is available;
- the service locations are known; and
- an operational customer contact can be selected.

The **Add Contract** action is available from a won opportunity. There is no general New Contract button on the Contracts list.

## Contracts list

Open **Contracts** to see up to 100 contracts you are allowed to view. The table shows:

- contract reference;
- opportunity;
- account;
- status;
- effective date; and
- expiry date.

Contracts are presented in expiry-related order to support renewal planning. The current list does not provide search, filters, pagination, or clickable sorting. Select a row to open the contract.

## Creating a contract

1. Open a Won opportunity.
2. Open **Add** and select **Contract**.
3. Complete the contract form.
4. Save.

| Field               | What to enter                                                       | Required? |
| ------------------- | ------------------------------------------------------------------- | --------: |
| Contract reference  | Unique official reference used to identify the agreement            |       Yes |
| Effective date      | Date service or agreement becomes effective                         |       Yes |
| Expiry date         | Date the contract ends; must be after the effective date            |       Yes |
| Operational contact | Customer contact responsible for operational coordination           |       Yes |
| Service locations   | One or more account sites covered by the contract                   |       Yes |
| Renewal notice days | Number of days before expiry to begin renewal action, from 1 to 730 |       Yes |

The opportunity services and owner are carried into the contract automatically.

### Before opening the form

Confirm on the account that:

- an accurate operational contact exists and is marked for Operations;
- every covered service location has been added; and
- the won opportunity points to the correct customer and approved quote.

### Example

- Contract reference: HHCIL/NORTHSTAR/2027/001
- Effective date: 1 January 2027
- Expiry date: 31 December 2027
- Operational contact: Kavita Rao
- Service locations: Pune Plant 1; Pune Plant 2
- Renewal notice days: 90

The initial contract is created in **Draft** because the current creation form does not upload a signed agreement at the same time.

## Contract statuses

| Status | Meaning                                                                              |
| ------ | ------------------------------------------------------------------------------------ |
| Draft  | Contract record exists but the signed agreement has not been uploaded and activated. |
| Active | Signed agreement has been uploaded and the contract is in force in the CRM.          |

The current application does not automatically show separate Expired or Renewed contract statuses. Use dates and renewal information to monitor approaching or passed expiry.

## Activating a contract

### What activation does

Activation confirms that signed commercial evidence has been attached. This is required before an operational handover can be created.

### How to activate

1. Open the Draft contract.
2. Find the **Activate** section.
3. Choose the signed agreement file.
4. Select **Upload and activate**.
5. Confirm that the status changes to Active.

The screen accepts PDF, JPEG, and PNG files, up to 10 MB. Upload a complete, legible, authorized document. The production environment may apply additional file-security checks.

Do not upload unrelated documents or unsigned drafts merely to activate the record.

## Contract detail page

The page shows:

- contract reference and status;
- effective and expiry dates;
- renewal reminder date and status;
- signed-agreement state;
- services;
- service locations;
- amendment history; and
- handover history.

Use it as the main place to verify the current contractual and renewal position.

## Amendments

### What an amendment is

An amendment records an approved change to an existing contract while preserving the previous contract snapshot. It is appropriate for changes such as expiry extension or renewal-notice adjustment.

### How to add an amendment

1. Open the contract.
2. Select the amendment action.
3. Complete:
   - **Reason**;
   - **Expiry date**;
   - **Renewal notice days**; and
   - **Approved change notes**.
4. Save.

### Field guidance

| Field                 | Guidance                                                      |
| --------------------- | ------------------------------------------------------------- |
| Reason                | Short business reason, such as “Six-month extension approved” |
| Expiry date           | New valid expiry date                                         |
| Renewal notice days   | Updated lead time for the renewal reminder                    |
| Approved change notes | Reference the agreed change and its approval evidence         |

Saving an amendment retains history and recalculates the renewal reminder when relevant. It does not replace the need for properly approved and signed legal documentation.

## Renewal reminders

The renewal reminder date is calculated from:

```text
Expiry date − Renewal notice days
```

For a contract expiring 31 December with 90 notice days, renewal action should begin around early October.

Renewal information appears in the contract and Renewals report. The background worker can create renewal notifications when configured, but there is no separate notification-inbox screen. Review Contracts, Reports, Tasks, and the Dashboard as part of regular renewal management.

The current contract page does not provide a **Mark renewed** action. If the customer renews, follow the approved process for amendment or a new contract record as directed by the process owner.

## Operational handovers

### What a handover is

A **Handover** packages the approved sales and contract information for operations. It helps ensure that the delivery team receives the same scope, sites, contacts, and commercial basis that were agreed during sales.

### Before creating a handover

The contract must be Active, and the following evidence must be complete:

- approved commercial basis is attached;
- service scope is confirmed;
- all service locations are confirmed;
- operational contact is confirmed; and
- approved requirement snapshots are available.

### Creating a handover

1. Open an Active contract.
2. Select the handover action.
3. Review each checklist item.
4. Keep an item selected only when it is genuinely confirmed.
5. Submit the handover.

The checklist initially includes:

- Approved commercial basis attached
- Service scope confirmed
- All service locations confirmed
- Operational contact confirmed

All required items must be confirmed. The handover is versioned so the exact information sent can be identified later.

## Handover statuses

| Status   | Meaning                                                        |
| -------- | -------------------------------------------------------------- |
| Pending  | Handover was prepared and is awaiting delivery or processing.  |
| Sent     | Handover was successfully sent to the operational integration. |
| Accepted | Receiving system or team accepted it.                          |
| Rejected | Receiving side rejected it; review the recorded reason.        |
| Failed   | Delivery attempt failed and requires controlled recovery.      |

The current page displays handover status and rejection information when available. It does not yet provide buttons for manual retry, acceptance, or rejection. Contact the integration or CRM administrator for a failed or rejected handover. Do not create repeated handovers merely to force delivery, because stable handover identifiers are intended to prevent duplicate operational sites.

## Real-world example

After Northstar accepts the approved quote:

1. The salesperson moves the opportunity to Won.
2. The account manager creates a draft contract for both Pune plants.
3. The signed agreement is uploaded, activating the contract.
4. The account manager verifies the approved requirements, commercial evidence, two locations, and operational contact.
5. A handover is created.
6. Operations monitors its status and contacts the integration owner if it fails or is rejected.
7. Ninety days before expiry, the account manager begins the renewal review.

## Related features

- Accounts provide contacts and locations.
- Opportunities provide services and the won commercial journey.
- Quotes provide approved commercial evidence.
- Requirements provide frozen scope snapshots.
- Reports provide a combined renewal forecast.
- Audit history records important contract and handover actions.

## Important notes

- Contract references must be unique.
- Verify that expiry is later than effective date.
- Uploading a signed agreement is a controlled action.
- Handover is a post-sale operational step, not a replacement for quote approval.
- Failed or rejected integrations require review; repeated manual submissions can create confusion.
- The CRM protects historical amendments and handover versions for traceability.
