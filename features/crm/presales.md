# Presales

The presales module is used to manage the presales process.

## Deals (Opportunities)

> *Activity* → **Opportunity** → *Offer* → *Sales Order* → *Invoice Order* → *Invoice*

The deals in the @Crm.Presales.Deals are used to manage sales opportunities to new or existing customers.

> [!note]
> Deal is synonymous to opportunity.

The deals:

* Have appointed sales representative, managing the deal.
* Do not have line items. They are used to manage deals, which are still not clear enough to detail at this level.
* Have a percentage **probability of success**. The percentage is set by the sales representative, based on their own judgement.
* Have expected **sales revenue**.
* Have expected **close date**.

Based on the data above, the team leaders and sales managers have instant and clear visibility over the sales processes.


The deals are usually initially created based on @General.Contacts.Activities.
However, once a deal is created, it can be used to create many more sub-activities to manage related tasks.

## Offers (quotes)

> *Activity* → *Opportunity* → **Offer** → *Sales Order* → *Invoice Order* → *Invoice*

The deals documents can be easily transformed into Offers (quotes), which contain detailed line items.

Entries in the @Crm.Presales.Offers allows the customer to be presented with optional items.
After approving some or all of the optional items, the offer can generate @Crm.Sales.SalesOrders in the [Sales](sales.md) module.
