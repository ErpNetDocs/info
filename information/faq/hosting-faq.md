# Hosting & Reliability FAQ

## High Availability & Monitoring

### Does the @@name service feature high availability?

Yes.

There are many components in an ERP instance - database,
application servers, web servers, apps, reverse proxy, process manager, etc.
Each component is hosted on a hardware, which is always having a 
stand-by backup hardware, ready to take over in a case of a hardware failure.

All network components are also stacked for high availability.
Each network component is cross-connected to each host.

The point is, there is no single point of failure.

### Is the system monitored at all times?

Yes.

There is a dedicated team, monitoring all systems 24x7x365.
In case of an issue, reaction time is usually in the 5-15 minutes range, day and night.

### What happens in case of a hardware problem?

The most important part is the problem to be automatically 
detected by the watchdog systems.

Once the problem is detected, an automatic failover occurs.
The failover is usually within 30-60 seconds.

Most of the time, the users might notice just a slight delay in their processing.

### What is the reaction time in case of an issue?

First of all, most issues auto-resolve themselves, 
because each component has high-availability and the workload is automatically
transferred to another node.

However, should it reach to a human intervention, the reaction time usually is
within 5-15 minutes, day and night, 24x7x365.

### Is the system monitored from outside?

Yes.

There are at least two different locations,
usually in different countries or states,
which has automatic watchdogs setup.

Each alarm for non-availability is reviewed by human operators.

## Disaster Recovery & Backups

### Are there backups of my data?

Yes.

We hope you are joking and this is a rhetorical question 🙂.

Seriously, the backup planning, execution and control is one of most important activities out there.
You can read more about backups in the [Disaster Recovery](../system-information/disaster-recovery.md) section.

### Is the off-site backup included in the price?

Yes.

The off-site backup is included in the price for all subscription levels.
You do not need to do anything in order to be fully protected.

## Miscellaneous

### What hardware is used for the service?

There are a lot of moving parts in a proper ERP service.
Reliability is the most important factor when choosing the correct hardware.
Performance comes second, but is also of paramount importance.

It is hard to describe all hardware, but here are some quick facts:

Database servers:

* Top of the line, data center grade, specialized frequency optimized CPU.
These usually cost around 10 times more per core than regular CPUs.
* 32 GB RAM per core.
* Specialized memory-class SSD drives for caching and temp db.
* Top of the line SSDs for databases.
* 100 Gbit network connections to backup and hot-stand-by server.
* 25 Gbit network connection to application servers.

Application servers:

* Enterprise grade general-purpose CPU for application processing.
* 8 GB (up from 4 until 2023) RAM per application core.
* SSDs for storage.
* 25 Gbit network connections

Network components:

* Enterprise grade routers, switches, firewalls, etc.

### What database size to expect?

Database sizes vary depending on many factors:

* Regular user processing.
* Automation by applications.
* Storage of documents, pictures, etc.
* Use of [Track Changes](xref:track-changes) feature.

etc.

We can only try to predict, with big tolerance for error, the regular user processing.

As a rule of thumb, each user generates approximately between 0.25 and 1.00 GB of data per year.
