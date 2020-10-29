# Core capacity information

Medium to large and Internet-facing @@name instances are provided, based on "cores".

"Core" defines server processing capacity.

## User perspective

From users perspective, a core provides enough capacity for comfortable work of **30 concurrent internal users**, or up to **45 concurrent light-use users**.

However, todays workloads are rarely just internal users, using the default UI clients.
Service apps, Internet users and third-party UI apps take their toll.
Their load levels are hard to predict.

> [!note]
> Small business subscriptions are based on concurrent internal users only, and not on cores.
> They can incorporate service and Internet apps, but their load is prorated to internal users.
> Check your reseller for more information.

## Hardware capacity description

Although "core" licensing is originally based on hardware specifications, nowadays it is sized through software and the exact hardware specs are just an approximation.

Having said that, each core is allocated capacity, approximately equal to:

* 1 CPU core for SQL Server
* 32 GB RAM for SQL Server
* 1 CPU core for Application server
* 4 GB RAM for Application server (but not less than 8 GB per app server)
