# Routing examples

This article contains workflow examples and zone-based rules.
The rules are portrait in a simplified manner just for demonstration purposes.
The actual rules, although more complicated, are still easy to manage by the WMS process designers.

## Typical flow

In the typical flow, the zones are sequantially numbered from 1 to 6, depending on their closeness to shipping.

> 1 IN → 2 INSP → 3 BULK → 4 PICK → 5 PACK → 6 OUT

### RECEIVE

ON RECEIVE process rules for each zone:

1. IN → INSP
1. Q:OK INSP → BULK
1. Q:NOT-OK INSP → QUARANTINE

The receive process moves the goods from the inbound docks to the inspection zone.
After the goods are inspected, they are moved either to the bulk storage zone or to the quarantine zone.

### OPTIMIZE

1. BULK → PICK (based on minimal qty)

The optimize process is run twice per day.
It ensures, that the picking zone has enough quantities to serve sales orders.

### DISPATCH

1. PICK → PACK
1. PACK → OUT
1. OUT: DISPATCH

After a sales order is picked, it is sent to the packing tables and then to the outbound docks.

## Flow with kitting

With the kitting workflow, some items might need kitting, before they are sent to the customers.

> 1 IN → 2 INSP → 3 BULK → 4 PICK → 5 KIT → 6 PACK → 7 OUT

### RECEIVE

1. IN → INSP
1. Q:OK INSP → BULK
1. Q:NOT-OK INSP → QUARANTINE

The receive process moves the goods from the inbound docks to the inspection zone.
After the goods are inspected, they are moved either to the bulk storage zone or to the quarantine zone.

### OPTIMIZE

1. BULK → PICK (based on minimal qty)
1. PICK: KIT 

The optimize process is run twice per day.
It ensures, that the picking zone has enough quantities to serve sales orders.
The kitting task is performed in the picking zone, again based on minimal quantities.

### DISPATCH

1. PICK → PACK
1. KIT → PACK
1. PACK → OUT
1. OUT: DISPATCH

Here, two rules compete for the quantities of the order.
If there are enough quantities in the picking zone, the order is picked immediately.
If not, the remaining quantities are scheduled for kitting first.

After a sales order is kitted and picked, it is sent to the packing tables and then to the outbound docks.

## Cross-docking

> 1 IN → 2 OUT

### RECEIVE

1. IN: IF CROSS_DOCK → OUT

### DISPATCH

1. OUT: DISPATCH

Of course, the above rules can be easily combined with other rules.

## Labelling

The rules for labelling can easily be combined with other rules:

### OPTIMIZE

1. PICK: LABEL (based on minimal qty)

### DISPATCH

1. PICK: LABEL (based on order qty)
