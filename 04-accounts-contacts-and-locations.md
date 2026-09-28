# Accounts, Contacts, and Locations

## How these records fit together

- An **Account** is a customer or prospective customer organization.
- A **Contact** is a person associated with that organization.
- A **Location** is a physical place where a service may be delivered or surveyed.
- An **Opportunity** is a potential piece of business for the account.

One account can have several contacts, locations, opportunities, contracts, and account-review activities. Keeping these under one account gives users a shared customer history.

## Accounts

### What an account is

An account represents the organization, not an individual enquiry. It stores the legal and trade names, tax identifier, industry, branch, billing address, owner, and related business records.

### Why and when to use it

Use an account after an organization becomes a meaningful prospect or customer. Lead conversion creates an account automatically. Authorized users can also create an account from the Accounts page when there is a valid reason to establish the organization without a new lead.

Before creating one manually, search by legal name, trade name, or GSTIN to avoid duplicates.

## Finding an account

Open **Accounts**, enter all or part of a legal name, trade name, or GSTIN, and press Enter. Select **Refresh** to reload the results.

The current page loads up to 100 visible accounts and does not provide pagination or clickable column sorting. Each row shows the organization, GSTIN, and branch. Select the row to open the account.

## Creating an account manually

1. Open **Accounts**.
2. Select **New account**.
3. Complete the form.
4. Save the account.

| Field           | What to enter                                         | Required? |
| --------------- | ----------------------------------------------------- | --------: |
| Legal name      | The organization’s registered legal name              |       Yes |
| Trade name      | The brand or commonly used name, if different         |        No |
| GSTIN           | Verified Goods and Services Tax Identification Number |        No |
| Industry        | Closest available industry                            |        No |
| Branch          | HHCIL branch responsible for the relationship         |       Yes |
| Billing address | Registered or billing address, when known             |        No |

The signed-in user becomes the owner. The current form does not ask for a different owner.

### Example

- Legal name: Northstar Textiles Private Limited
- Trade name: Northstar Textiles
- GSTIN: verified customer GSTIN
- Industry: Manufacturing
- Branch: Pune
- Billing address: registered office address supplied by the customer

Do not copy a GSTIN from an unverified source. Incorrect legal or tax information can later affect quotes and contracts.

## Viewing and editing an account

The account page brings together:

- account overview;
- contacts;
- service locations;
- opportunities;
- account-review activities; and
- contracts.

Select **Edit account** to update:

- legal name;
- trade name;
- GSTIN; and
- billing address.

Use editing to correct or update the same organization. Do not change an account into a different customer. The current interface does not permanently delete accounts.

## Contacts

### What a contact is

A contact is a person at the customer organization. Contact records identify who makes decisions, provides operational information, uses the service, controls access, or receives sales, operations, or billing communication.

### Adding a contact

1. Open the account.
2. Select **Add contact**.
3. Complete the contact fields.
4. Save.

| Field      | What to enter                                             | Required? |
| ---------- | --------------------------------------------------------- | --------: |
| Name       | Full name of the person                                   |       Yes |
| Role       | Job title or business role, such as Facility Manager      |        No |
| Influence  | The person’s role in the buying or service decision       |        No |
| Email      | Verified business email                                   |        No |
| Phone      | Verified contact number                                   |        No |
| Sales      | Select if the person should be treated as a sales contact |        No |
| Operations | Select if the person is an operational contact            |        No |
| Billing    | Select if the person handles billing matters              |        No |

### Influence values

| Value          | Meaning                                                   |
| -------------- | --------------------------------------------------------- |
| Decision maker | Has final authority to approve or select the service      |
| Influencer     | Advises or shapes the decision but may not sign it        |
| User           | Will directly use or work with the service                |
| Gatekeeper     | Controls access to decision makers, sites, or information |
| Unknown        | Influence has not yet been confirmed                      |

The Sales, Operations, and Billing options are not mutually exclusive. For example, a facility head may be both the operational and decision-making contact.

### Real-world example

For Northstar Textiles, add:

- Name: Kavita Rao
- Role: Head of Administration
- Influence: Decision maker
- Sales: selected
- Operations: selected

If Kavita will be selected as the operational contact on a contract, ensure **Operations** is selected and the phone/email information is current.

### Current limitation

The current account screen can add contacts but does not provide contact edit or delete buttons. Verify the information before saving. If a saved contact must be corrected, contact an authorized administrator or process owner.

## Service locations

### What a location is

A location is a customer site where HHCIL may inspect, mobilize, or deliver a service. Locations are used by site surveys, contracts, and operational handovers.

### When to add one

Add the location as soon as a site is known, and before scheduling a site survey or creating a contract that must identify service locations.

### Adding a location

1. Open the account.
2. Select **Add location**.
3. Complete the address.
4. Save.

| Field          | What to enter                              | Required? |
| -------------- | ------------------------------------------ | --------: |
| Location name  | A recognizable name such as Pune Plant 1   |       Yes |
| Address line 1 | Building, plot, street, or primary address |       Yes |
| Address line 2 | Additional landmark, floor, or area        |        No |
| City           | City or town                               |       Yes |
| State          | State                                      |       Yes |
| PIN            | Postal PIN code                            |        No |

Use separate records for physically separate service sites, even when they belong to the same customer.

### Current limitation

The current screen does not provide location edit or delete buttons. Confirm the address before saving.

## Account reviews

### What an account review is

An account review records a structured conversation about the customer relationship, service direction, risks, expansion, or future action. It becomes part of the account’s activity history.

### How to record one

1. Open the account.
2. Select **Record account review**.
3. Enter a **Subject**.
4. Add **Discussion notes**.
5. Record the **Outcome / next direction**.
6. Save.

### Example

- Subject: Q2 service review and expansion discussion
- Discussion notes: “Customer is satisfied at Pune Plant 1 and expects a new warehouse to open in December.”
- Outcome / next direction: “Visit proposed warehouse and assess housekeeping scope by 15 October.”

Use factual, professional notes. Do not record unsupported personal judgments.

## Connected opportunities and contracts

The account page lists its opportunities and contracts. Select one to open the detailed record. This connection helps users answer:

- What business is currently being pursued?
- What has been won or lost?
- Which contracts are active?
- When are renewals due?
- Which sites and contacts are involved?

Although an empty account may prompt users to create an opportunity, the current user interface has no separate opportunity-creation form. Create new opportunities through lead conversion.

## Important notes

- Search before creating an account.
- Use the legal name for official records and the trade name for the familiar brand.
- A contact belongs to one account in the current workflow.
- A site survey cannot be scheduled until the account has at least one location.
- A contract needs an operational contact and one or more service locations.
- No Add, Edit, or View permission should be assumed from a colleague’s access; screens are role- and scope-aware.

## Related guides

- [Leads and CSV import/export](03-leads-and-import-export.md)
- [Opportunities, activities, and tasks](05-opportunities-activities-and-tasks.md)
- [Requirements and site surveys](06-requirements-and-site-surveys.md)
- [Contracts, renewals, and handovers](08-contracts-renewals-and-handovers.md)
