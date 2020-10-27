# Lot Tracking

@@name supports lot tracking throughout the supply chain.

## Relation to serial number tracking

Lot tracking is a separate feature from [Serial Numbers Tracking](serial-numbers.md).
Lots and serial numbers can be tracked simultaneously.

## Going down the document chain

Lot numbers can (optionally) be specified up from the initial document in the [chain](xref:document-chain) and transferred down to the last.

For example, some customers might have special requirement for remaining expiry time or other specifics. In this case, the sales representative can specify the lot number in the Sales Order.
In this case, the lot number is transferred through the document chain down to the Store Order and eventually issued with the Store Transaction.

However, if the lot number is left blank in the Store Order, it can be specified later in the chain or left to the system to automatically choose using FIFO/FEFO/LIFO methods.

## More information

For detailed information about the related entities see:

* @Crm.Sales.SalesOrders
* @Logistics.Inventory.StoreOrders
* @Logistics.Inventory.StoreTransactions
* @Logistics.Inventory.StoreTransactionLines
