# Quotes and Approvals

## What a quote is

A **Quote** is the versioned commercial offer for an opportunity. It contains line items, quantities, rates, discounts, taxes, charge types, terms, assumptions, exclusions, validity, totals, approval history, and downloadable PDFs.

Each quote version is retained. This makes it possible to understand exactly what was approved and sent at each point in the negotiation.

## Why and when to use Quotes

Create a quote after the service scope is sufficiently clear and all opportunity requirements are approved. Use it to prepare the customer-facing commercial offer and obtain internal approval before sending it.

A quote should not be used as a rough personal calculation. Draft it from verified requirements and follow the approval policy shown by the application.

## Before creating a quote

The opportunity must have:

- at least one requirement; and
- every requirement in Approved status.

If quote creation is refused, return to the opportunity and check for a missing or draft requirement.

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
| Rejected          | Approver declined the version                    | Review comments and contact the process owner      |
| Changes requested | Approver requires revision                       | Review comments and arrange a new version          |
| Withdrawn         | Submission was withdrawn from approval           | Confirm why and whether a new submission is needed |
| Sent              | Approved version has been issued to the customer | Continue follow-up and negotiation                 |

Only an approved quote can be marked Sent.

## Quote detail page

The quote page shows:

- current version and status;
- validity date;
- itemized charges and totals;
- payment terms, assumptions, and exclusions;
- version history;
- approval history and comments; and
- available workflow actions.

Depending on status and permission, actions include:

- **PDF** — open/download the quote document;
- **Submit for approval** — send a draft into the approval process; and
- **Mark sent** — record that an approved quote was issued to the customer.

## Submitting for approval

1. Review every line, rate, discount, tax, date, and term.
2. Open the generated PDF and confirm the customer-facing result.
3. Select **Submit for approval**.
4. Review the confirmation message and select **Submit for approval** again.
5. The status becomes Pending approval when approval steps apply.

Approval rules may depend on branch, amount, discount, commercial exception, and ordered approver roles. The CRM evaluates the configured policy; users should not bypass it by changing a value without a genuine business reason.

## Approval inbox

Users with commercial approval access can open **Approvals**. Each pending card shows information such as:

- account and opportunity;
- quote version;
- submission date; and
- amount.

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

The quote page retains every version and provides a PDF for each available version. A draft PDF may carry a draft indication. Historical versions remain available so users can verify what was previously offered.

PDF and commercial-rate access can be separately restricted. If the PDF control or sensitive rates are unavailable, ask an authorized user rather than sharing another user’s download.

## Current revision limitation

The underlying workflow supports quote versions, but the current screen does not provide a **New version**, **Withdraw**, or **Resubmit** button. If an approval is rejected or changes are requested, review the permanent approval comments and contact the authorized commercial process owner to arrange the next version. Do not edit or send the rejected version outside the controlled process.

## Real-world example

For the Northstar opportunity:

- Recurring line: Monthly housekeeping manpower, 1 month × ₹4,50,000
- One-time line: Mobilization and equipment setup, 1 × ₹1,25,000
- Valid until: 31 October
- Payment terms: Monthly invoice payable within the agreed period
- Assumption: Customer provides water and electricity at service points
- Exclusion: Specialized façade cleaning not included

After all requirements are approved, the salesperson creates the quote and submits it. The commercial approver requests a clearer mobilization line. Because the current revision button is not available, the salesperson follows the approved internal process with the commercial owner before a corrected version is resubmitted.

## Related features

- Requirements provide the approved scope.
- Opportunity stage history records commercial progress.
- Approval policies determine who must approve.
- An approved or sent quote is required before Won.
- A won opportunity with approved commercial evidence can become a contract.

## Important notes

- Rates, discounts, and PDFs are commercially sensitive.
- Never send a Draft, Pending approval, Rejected, or Changes requested version.
- Protected commercial changes require a new controlled version and approval.
- Approval comments and old versions are permanent history.
- “Approved” is an internal status; “Sent” confirms customer delivery.
