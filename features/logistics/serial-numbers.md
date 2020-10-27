# Serial Numbers

@@name supports tracking serial numbers tracking throughout the supply chain.

## Relation to lot tracking

Serial numbers tracking is a separate feature from [Lot Tracking](lot-tracking.md).
Lots and serial numbers can be tracked simultaneously.

## Going down the document chain

Serial numbers can (optionally) be specified up from the initial document in the [chain](xref:document-chain) and transferred down to the last.

For example, even the Sales Order can specify concrete serial number, if so is desired.
In this case, the serial number is transferred through the document chain down to the Store Order and eventually issued with the Store Transaction.

However, if the serial number is left blank in the Store Order, it can be specified later in the chain - most probably when picking the product from the warehouse.

## More information

For detailed information about the related entities see:

* @Crm.Sales.SalesOrders
* @Logistics.Inventory.StoreOrders
* @Logistics.Inventory.StoreTransactions
* @Logistics.Inventory.StoreTransactionLines
