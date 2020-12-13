# Zone Based Routing

## The basic idea

With Zone based routing, the rules for processing the goods are determined based on the zone, in which the goods are stored for each step. The zones are sequentially numbered, relative to their "closeness" to final shipping. For example:

> 1 IN -> 2 INSP -> 3 BULK -> 4 PICK -> 5 KIT -> 6 PACK -> 7 OUT
>
> RECEIVE ------------> --OPTIMIZE--> ----------------> DISPATCH

The main processes in the warehouse - receive, optimize and dispatch, are ordered consecutively through the zone sequence. The receive process starts at the inbound docks and runs until goods are placed in bulk. The optimization process usually deals with replenishment of the picking zones, but can also be used for pre-kitting. The planning of the dispatch process works backwards - from the final step (the dispatch from the outbound docks) to the first step (usually picking). This is similar to how MRP/DRP works, but applied for WMS.

Zone based routing and sequencing provides great flexibility in the route formation process, while keeping things simple and understandable for the process designers. It allows the process designers to focus separately on each zone, leaving the complex full routing formation to the system. Zone based routing allows programming of very complicated routes, while still keeping things simple and maintainable.

## How it works?

For each zone, there are rules, which define how the goods will be processed, when they pass the zone. The rules for a zone are defined separately for each of the WMS processes - receive, dispatch and replenishment. The full route is the concatenation of all route steps for each consecutive zone.

## Hierarchical rules

Since zones are hierarchical, for any given zone there might be multiple rules, coming from different levels of the hierarchy. All rules in the hierarchy are combined when creating the routing. Combining the rules is performed separately for each STEP NO within each zone. To determine the "winning" rule for each step, the RULE PRIORITY is used within all rules, which satisfy the RULE CONDITIONs.

## Start and finish of the process

The receive process starts at the inbound dock and is planned through the zones, until there are no more steps. Usually, it finishes at the BULK zone. The dispatch process works in the opposite way - it first determines the quantities needed at the outbound docks, and than determines what previous steps could supply these quantities. The optimization process is a middle ground - it just runs for all zones, for which there is a definition for the optimization process.
