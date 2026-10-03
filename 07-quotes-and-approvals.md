# Quotes and Approvals

## What a quote is

A **Quote** is the versioned commercial offer for an opportunity. It contains line items, quantities, rates, discounts, taxes, charge types, terms, assumptions, exclusions, validity, totals, approval history, and downloadable PDFs.

Each quote version is retained. This makes it possible to understand exactly what was approved and sent at each point in the negotiation.

## Why and when to use Quotes

Create a quote after the service scope is sufficiently clear and all opportunity requirements are approved. Use it to prepare the customer-facing commercial offer and obtain internal approval before sending it.

A quote should not be used as a rough personal calculation. Draft it from verified requirements and follow the approval policy shown by the application.

## Before creating a quote

Every requirement already attached to the opportunity must be in **Approved** status.

Use requirements whenever the scope or pricing needs controlled sign-off. If quote creation is refused, return to the opportunity and check for a Draft requirement or confirm that your role can create quotes.

## Creating a quote

1. Open the opportunity.
2. Open **Add** and select **Quote**.
3. Enter the validity and payment terms.
4. Add one or more line items.
5. Add assumptions and exclusions.
6. Save the draft.

### Header and commercial fields

| Field         | What to enter                                            | Required? |
| ------------- | -------------------------------------------------------- | --------: |
| Valid until   | Last date on which the offer remains valid               |       Yes |
| Payment terms | Clear timing and conditions for payment                  |       Yes |
| Assumptions   | Facts used to calculate the offer but not yet guaranteed |        No |
| Exclusions    | Items specifically outside the offered scope or price    |        No |

The quote currency comes from the opportunity.

### Line-item fields

| Field       | Meaning                                                                 |
| ----------- | ----------------------------------------------------------------------- |
| Description | Clear service, staffing, equipment, or fee description                  |
| Quantity    | Number of units being priced                                            |
| Unit        | Pricing unit, such as month, person, visit, or item                     |
| Rate        | Price for one unit before discount and tax                              |
| Discount %  | Percentage reduction for that line, if authorized                       |
| Tax %       | Applicable tax percentage                                               |
| Type        | **Recurring** for repeating charges or **One-time** for a single charge |

Use **Add line** for another line. Extra lines can be removed while preparing the draft.

### How totals are calculated

The CRM calculates totals on the server using two-decimal money rules:

1. Quantity × Rate = line subtotal
2. Discount is deducted from the subtotal
3. Tax is applied after discount
4. The result becomes the line total
5. Line totals are combined into the quote total

### Calculation example

For 10 units at ₹20,000, with 5% discount and 18% tax:

- Subtotal: ₹2,00,000
- Discount: ₹10,000
- Amount after discount: ₹1,90,000
- Tax: ₹34,200
- Line total: ₹2,24,200

Always review the displayed total before submitting. If tax treatment is uncertain, consult the authorized commercial or finance owner.

## Quote statuses

| Status            | Meaning                                          | Typical next action                                |
| ----------------- | ------------------------------------------------ | -------------------------------------------------- |
| Draft             | Commercial offer is being prepared               | Review and submit for approval                     |
| Pending approval  | One or more approvers must decide                | Wait for or follow up with the current approver    |
| Approved          | All required approvals are complete              | Mark sent after issuing the approved version       |
| Rejected          | Approver declined the version                    | Review comments; revise or resubmit as appropriate |
| Changes requested | Approver requires revision                       | Review comments; revise or resubmit as appropriate |
| Withdrawn         | Submission was withdrawn from approval           | Create a revision or resubmit the unchanged version |
| Superseded        | Historical pending version was replaced by a newer current version | Use the current version; the historical record remains read-only |
| Sent              | Approved version has been issued to the customer | Continue follow-up and negotiation                 |

Only an approved quote can be marked Sent.

## Quote detail page

The quote page shows:

- current version and status;
- validity date;
- itemized charges and totals when your role can view protected commercial rates;
- payment terms, assumptions, and exclusions;
- version history;
- approval history and comments; and
- available workflow actions.

Depending on status and permission, actions include:

- **PDF** — open/download the quote document;
- **Revise draft lines** or **New version** — prepare a new immutable commercial version from the current lines;
- **Submit for approval** — send a draft into the approval process; and
- **Mark sent** — record that an approved quote was issued to the customer.

Some users may open a quote to review its status and approval history but see a notice that rates, discounts, taxes, and totals are restricted. This is intentional. Quote PDF download is also available only when the user has both the PDF-download permission and protected commercial-rate access. Do not ask another user to share a quote PDF or commercial values outside the approved access process.

## Submitting for approval

1. Review every line, rate, discount, tax, date, and term.
2. If your role provides PDF download, open the generated PDF and confirm the customer-facing result. Otherwise, follow the authorized commercial review process for the restricted version.
3. Select **Submit for approval**.
4. Review the confirmation message and select **Submit for approval** again.
5. The status becomes Pending approval when approval steps apply.

The current approval rules can be configured by branch, quote amount, maximum line discount, and ordered approver roles. The rule chosen when a version is submitted remains attached to that approval request, so a later policy change does not change who must decide an already-submitted version. Users should not bypass the process by changing a value without a genuine business reason.

## Approval inbox

Users with commercial approval access can open **Approvals**. Each pending card shows information such as:

- account and opportunity;
- quote version;
- submission date; and
- approval policy and current step; and
- amount, when the user is allowed to view protected rate details.

The inbox is deliberately limited. A pending version appears only when it is in a branch the approver is allowed to access and the approver's current role matches the required approval step. It is normal for an approver to see an empty inbox while work for a different branch or role remains pending.

### Making a decision

1. Open or review the quote and PDF.
2. Confirm requirements, calculations, discounts, taxes, terms, and exceptions.
3. Choose:
   - **Approve**;
   - **Changes**; or
   - **Reject**.
4. Enter a meaningful comment of at least two characters.
5. Confirm the decision.

### Decision meanings

- **Approve** — the version is acceptable for this approval step.
- **Changes** — the commercial offer may proceed only after specific revisions.
- **Reject** — the version should not proceed in its current business context.

Approval may be serial. One approval can move the quote to the next approver rather than making it fully Approved. The final required approval changes the quote to Approved.

### Good approval comments

- Approve: “Pricing and 18% tax verified against approved scope.”
- Changes: “Separate mobilization as a one-time line and correct validity to 30 days.”
- Reject: “Discount exceeds authorized commercial position; renegotiation required.”

Avoid comments such as “OK” when important commercial judgment is involved.

## Marking a quote sent

After the approved PDF has actually been issued to the customer:

1. open the approved quote;
2. select **Mark sent**; and
3. confirm that the approved version was actually issued to the customer by selecting **Mark sent** again in the confirmation dialog.

Do not mark it Sent merely because approval completed. Sent means the customer received that approved version through the organization’s approved communication process.

## Version history and PDFs

The quote page retains every version. A draft PDF may carry a draft indication. Historical versions remain available so authorized users can verify what was previously offered.

PDF and commercial-rate access can be separately restricted. If the PDF control or sensitive rates are unavailable, ask an authorized user rather than sharing another user’s download.

Quote PDF download requires both the PDF-download permission and protected commercial-rate access. If the PDF control or sensitive rates are unavailable, ask the commercial access owner to review your role rather than sharing another user's download.

## Revising a quote

Select **Revise draft lines** on a Draft quote, or **New version** on a resolved or Sent quote. Review the copied line items, rates, discounts, taxes, validity, terms, assumptions, and exclusions. Save to create a new Draft version, then submit that version for approval. Earlier versions and their approval history remain available to authorized users.

A version with **Pending approval** cannot be changed or replaced. This prevents an approver from deciding a commercial version that changed after submission. If the work must stop or change:

1. The person who submitted the current version (or a System Administrator) opens **Approval history**.
2. Select **Withdraw**, enter a clear reason, and confirm.
3. After withdrawal, select **New version** if any commercial field must change. Create and submit the revised draft.

For a current version that is **Rejected**, **Changes requested**, or **Withdrawn**, the original submitter (or a System Administrator) can instead select **Resubmit** in **Approval history** when the exact same version should go through approval again. Enter a meaningful comment. Resubmission creates a new approval request using the rules captured when that version was first submitted; it does not erase the earlier decision.

## Real-world example

For the Northstar opportunity:

- Recurring line: Monthly housekeeping manpower, 1 month × ₹4,50,000
- One-time line: Mobilization and equipment setup, 1 × ₹1,25,000
- Valid until: 31 October
- Payment terms: Monthly invoice payable within the agreed period
- Assumption: Customer provides water and electricity at service points
- Exclusion: Specialized façade cleaning not included

After all requirements are approved, the salesperson creates the quote and submits it. The commercial approver requests a clearer mobilization line. The salesperson opens **New version**, corrects the line, and submits the new draft for approval. The rejected version stays in history.

## Related features

- Requirements provide the approved scope.
- Opportunity stage history records commercial progress.
- Approval policies determine who must approve.
- An approved or sent quote is required before Won.
- A won opportunity with approved commercial evidence can become a contract.

## Important notes

- Rates, discounts, and PDFs are commercially sensitive.
- A user may be able to review approval status without being allowed to see commercial totals or download the PDF.
- Never send a Draft, Pending approval, Rejected, or Changes requested version.
- Protected commercial changes require a new controlled version and approval.
- Approval comments and old versions are permanent history.
- “Approved” is an internal status; “Sent” confirms customer delivery.
