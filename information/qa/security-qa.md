# Security & Auditing Q&A

### Are login and logouts of users tracked?

Yes.

The login and logout actions are tracked automatically and available in the tracking log.
There is no need to activate anything - this functionality is always active.

### Can the system track updates to data?

Yes.

Since tracking every update could be very space-consuming, this is subject to configuration.

Track changes can track information about:

* The latest update to the record
* Each update to the record
* Each update to each attribute

For more information, see [Track Changes](xref:track-changes).

### Can the system track updates to individual data attributes?

Yes.

Track changes can track updates to attributes.

### Can updates to user defined attributes be tracked?

Yes.

Changes to user-defined attributes are tracked the same way as updates to system attributes.

### Can the system track reads?

Yes.

To achieve the highest level of audit tracking and GDPR compliance, the system can be configured to track reads.
This can be very space-consuming and should be used judiciously.

Both reads of individual records and requests for general reports can be tracked.

* Report requests tracks just as the applied filters, not the actual data read.
* Individual record reads track the Id of the opened record.

### Is access to personal data tracked?

Yes.

It is the same auditing system, used to track reads, but configured for personal data.
