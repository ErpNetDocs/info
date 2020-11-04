# Customer Relationship Management (CRM) Subsystem

The CRM subsystem in @@name is used to manage customer relationships and other front-office activities of a company.

## General concepts and processes

The main process in the CRM subsystem is:

> *Activity* → *Opportunity* → *Offer* → *Sales Order* → *Invoice Order* → *Invoice*

* **[Activity](xref:General.Contacts.Activities)** - generic activity, related to a party. Includes support for calendar appointments, reminders, questionnaires, etc. Can be used to represent appointments, scheduled meetings, visits, contracts and just about any generic document.
* **[Opportunity](xref:Crm.Presales.Deals)** - sales opportunity, with expected revenue and probability. It does not have detail line items.
* **[Offer](xref:Crm.Presales.Offers)** - sales offer (quote), with line items. It allows optional selection of some of the items, which the customer has accepted.
* **[Sales Order](xref:Crm.Sales.SalesOrders)** - sales order from the customer. The main sales document. All documents before it are optional. The sales order initiates the logistics and financial processes, related to the sale.
* **[Invoice Order](xref:Crm.Invoicing.InvoiceOrders)** - an order to issue an invoice. This is an internal document, which is used to track the invoices, which we have to issue.
* **[Invoice](xref:Crm.Invoicing.Invoices)** - legal and financial document, finalizing the sales process.

> [!NOTE]
> The above diagram shows only the CRM part of the whole process.
> The full process involves many different modules of the ERP system.

## Modules

There are many modules in the CRM subsystem.
They are used to manage the different aspects of the CRM processes:

* **[Contacts and tasks](contacts-and-tasks.md)** - calendar appointments, party definitions, etc.
* **[Pre-sales](presales.md)** - Opportunities management, quotation, etc.
* **[Sales](sales.md)** - Sales Orders, customers, etc.
* **Invoicing** - Invoicing process management, invoices and BI.
* **POS** - Manage point-of-sale activities in physical stores.
* **Marketing** - Marketing campaigns, activities, distribution channels, etc.
* **Distribution** - field sales, sales person targets management, etc.
* **Pricing** - price lists management.
* **[Product Configurator](product-configurator.md)** - create products based on specs for job shops (made-to-order and engineer-to-order environments).
* **Products** - manage products master data - products and product measurements, codes, variants, channel, pictures, groups, etc.
