# Disaster Recovery

Disaster recovery planning and testing is a basic feature of @@name and is provided for all subscription levels.
You do not need to do anything to activate it.

## Backups

The automated backup plan includes:

* Transaction log backups every 30 minutes.
* Full backups every week.
* Secondary replica of backups in a different physical location (different data center).
* Retention period - 14 days.
* Manual test restores every year to test the backup procedures.

## Backup monitoring

The proper execution of the backup procedures is monitored at all times.

The procedures include manual checks and test restores, guaranteeing proper execution of the disaster recovery solutions.

## User requested restores

We are able to execute user requested restores.
The restore takes place as a new ERP instance, which is subject to a subscription plan.

## User access to the backups

Unfortunately, users access to the backup files is not allowed for security reasons.

However, the data in an ERP instance is readily accessible through the Table API, which is a thin layer over the physical database.
The Table API, although primarily intended for BI (Business Intelligence), can be used for data dumping, subject to the security permissions.

> [!note]
> Access through the Table API is logged.
