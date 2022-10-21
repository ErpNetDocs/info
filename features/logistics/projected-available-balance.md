# Projected Available Balance

## Overview

Every business selling physical goods, regardless of their exact industry sector, operates **an inventory** which is comprised of **itemized products and their quantities** meant for sale to customers.  
And customers, be it **individuals** or other **companies**, normally expect their ordered goods to be **shipped within some reasonable period**.  

Knowing your exact **current product quantities** is largely important for everyday operations and is also the foundation for any **future inventory planning**. 
To **keep meeting your customers’ expectations** in the long run, as well as to **minimize downtime** due to lack of supplies for the business's own operation, a useful approach is to **define and follow** a clear inventory management strategy. 
For achieving that, however, you must first learn to **review, prepare, and organize** your inventory **beyond its current availability**.  

This is done by implementing and utilizing what is called **Projected available balance** or **PAB**.  

**Projected available balance** is an important concept in inventory management. 
It represents the inventory balance (product quantities) that is **projected** (planned to have) **into the future** and is **expected to be available** on hand when the respective time comes.  

## The Challenge of Perceptive and Lean Inventory Management

Inventory keeping is the foundation for any business trading goods and it comes with the related expenditures. 
This means **balance between supplies and sales** is the one characteristic that gets the say when planning the inventory, as it largely affects how competitive and profitable the organization gets to be.  

An efficient business model **steers clear from maintaining large amounts** of products in any store or warehouse, as this can rapidly bump up space requirements, hinder management and maintenance, and open many risks for the staff and the business. 
The prohibitive costs originating from keeping such inventory amounts make sense for businesses to **order new supplies intelligently**, avoiding hoarding of stock that may become **unsaleable with time** (also known as dead stock), especially if it could quickly expire or become outdated morally, technologically, or otherwise.  

Typical examples for dead stock can be found in most industries, such as:  

* in the **food manufacturing and distribution** with many **preservative-free food products**, which can expire in just a few days or weeks  
* in the **fashion industry**, where clothes do not expire by perishing but rather by **falling out of fashion**, therefore drifting away from market demand  
* in **IT products retail**, where products not sold within a few years are already having discontinued support and are superseded by new more modern products.  

A visionary management **never skimps on replenishments** too, on the other hand, in order to **stay away from falling short of supplies** right when customers are **inquiring** or determined to **place an order**. 
Those customers who have already placed orders with a company remain a **number one priority for allocation and expense** of the available product quantities, as your business has already **made promises which must be kept**, for the level of customer satisfaction can vastly **impact the company's reputation** among its audience.  

Avoiding going to any of these two extremes helps to **protect your business** from delivery problems, reputation damage, and profit evaporation. 
Achieving this **balance** means always **keeping the right amounts** of products in stock, no more, no less.  

Successful inventory management is a sophisticated process that requires **an insightful approach with an eye to the future**.  

## What Exactly Is Projected Available Balance?

Projected available balance is basically **a listing of your planned product amounts** that are calculated for **one or more future periods** and are expected to **be on-hand at that time**, respectively.  

These amounts are called **projected** because they are **estimated into the future** and are **planned to be on site** in the store or warehouse.  

> [!NOTE]
> Many factors can **affect the actual availability** when the time comes, as delays in supplies, problems with transportation and receiving stock, customer orders cancellation, as well as other random accidents throughout the supply chain **exert their influence** on the real product quantities that truly **get to be on hand**.  
> 
> This, however, does not make the whole concept of PAB pointless, rather **outlines even further** the importance of understanding it to make **practical and foresighted decisions**, making your business more resilient when recovering from any accidents that may happen, and also staying more flexible and productive when serving customers.  

The reason PAB is so essential is the fact it is used for several critical inventory operations, such as calculating the **Available to promise** product quantities your business can offer, releasing **Master Production Schedule (MPS)**, **making proper decisions** when the need for restocking arises, **balancing out** the manufacturing, warehouse, and delivery loads, and many others.  

## How to Find out Projected Available Balance

PAB is derived from the **current inventory balance** by subtracting **planned outbound store orders** and adding **scheduled receipts of supplies**. 
It is a **running sum** that starts from the current values and is iteratively calculated for all **consecutive future periods** until calculations **reach the desired period**.  

The general formula for calculating PAB is as follows:  

**PAB sum = PI + RS - SO**

where:  

* **PAB sum** is Projected Available Balance listing
* **PI** is currently present inventory
* **RS** are Scheduled receipts of supplies
* **SO** are planned outbound store orders (for intrastore movement or customer delivery)

all of which apply for a **single given product**.  

> [!NOTE]
> **Projected available balance** should NOT be mistaken for **Available to promise** inventory quantities.  
> 
> Projected available balance represents **the full inventory amount** that is expected to be physically at hand for any successive future period.  
> 
> Available to promise shows only this **inventory portion that remains physically available to offer for sale and delivery**, aside from fulfilling already placed customer orders or serving the company's own necessities.  
> 
> Although close in meaning and related in implementation, the two terms still express different concepts.  

## PAB Example

Suppose we run a company that trades hand tools and power tools. 
Let us take some product, for example, **a cordless drill driver**. 
We will take a look at how its quantity is projected over **the course of a week**.  

For each day we have **a number of planned orders**, and respectively, expect to receive **a number of supplies** for this product.  

We start with an initial inventory quantity of **30 drills**. 
This quantity is also the projected available balance right now, as it matches the present.  

Using the above-mentioned formula, we can calculate the number of cordless drivers we expect to have at hand on each subsequent day, shown in the last column:  

| Day | Orders | Supplies | PAB | 
| - | - | - | - | 
| Starting | N/A | N/A | 30 | 
| 1 | 22 | 11 | 19 | 
| 2 | 25 | 18 | 12 | 
| 3 | 17 | 27 | 22 | 
| 4 | 0 | 20 | 42 | 
| 5 | 39 | 0 | 3 | 
| 6 | 0 | 0 | 3 | 
| 7 | 10 | 35 | 28 | 

> [!NOTE]
> **Projected available balance** can be a **positive**, **zero**, or **negative number**, depending on the **planned orders** and s**cheduled receipts**.  
> 
> For successfully managing your store, you must make sure you enter each consequent time period with an inventory that is suited to the market demand. 
> This means the **sum** of the **projected available balance for the current period** and the **scheduled supplies for the current period** must **at least match** the **outbound orders for the next period**.  

You can find more information on how PAB is calculated in @@name on the following document:  

[**Projected Available Balance - Technical Documentation**](xref:PAB)

## Why PAB Matters in Your Business

Projected available balance is a **powerful inventory management tool** that can help you gain **better insight** into your inventory. 
Understanding it can help you **make smarter decisions** when replenishing and spending up your inventory.  

**Utilizing** projected available balance and coming up with a **solid inventory management strategy** allows your business to **keep its promises** to customers while **avoiding overstocking or underdelivering**.  

## PAB implementation into @@name

Projected available balance is **deeply integrated** into @@name's Logistics subsystem.  

PAB functionality in @@name, similarly ATP, **operates in real time**, so your business can **always receive the latest and most up to date inventory data**.  

If any new orders are planned or supplies are scheduled, they will immediately take effect on PAB and ATP quantities and reports. 
This way you can always stay tuned with your inventory movements and know what promises to make to your partners, customers, and other parties.  

## Benefits of Understanding and Utilizing PAB Concept

By mastering **Projected available balance** and utilizing it via your @@name platform, your business can go a long way towards:  

* Preventing accumulation of dead stock or stock shortages 
* Increasing the efficiency of inventory operations
* Reducing accumulation of outdated or waste materials and damaged goods in the warehouse
* Enhancing the general view of the inventory
* Lightening and redistributing the load on equipment, people, and others.

## More Information

You can find more information on the exact calculation methods and ATP algorithm, the technical implementation and reporting of ATP, as well as the data and documents used in handling ATP quantities in @@name on the following article:  

[**Projected Available Balance - Technical Documentation**](xref:PAB)
