---
uid: document-chain
---
# Document Chains

When documents are created in @@name they usually form document chains.

For example, the basic document chain in CRM is:

> *Activity* → *Opportunity* → *Offer* → *Sales Order* → *Invoice Order* → *Invoice*

The subsequent documents in the chain are usually automatically created, but can also be manually typed.

@@name tracks the relations between each document instance, so that the users can easily traverse the document chain up and down.

## Example

This feature can be especially useful for financials.
Suppose you are investigating some financial statement.
You open a @Finance.Accounting.AccountingVouchers:  

![Document-chains-accounting-vaucher-2023-07-11](https://github.com/k1kolev/info/assets/106669250/ba0dde01-b6a7-4d0d-a21a-f8a2fd95157c)

From there you traverse up the document chain and consequently find Store Transaction, Receiving Order and finally the Purchase Order.  

The saved navigation data helps you quickly spot the originating document:  

![Document-chains-purchase-order-2023-07-11](https://github.com/k1kolev/info/assets/106669250/de3f0980-35cd-4e0d-98d0-89e534b0cba5)
