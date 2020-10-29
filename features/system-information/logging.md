# Log of everything

Everything in an @@name instance can be logged.
This includes, but is not limited to:

* User session events - login, logout, etc.
* Updates - create, update and even delete of records.
* Updates to system settings, business workflow rules, etc.
* Tracking of updates to specific data attributes, even BLOBs.
* Read access, e.g. a user just opening a document.
* System events.
* Results of scheduled jobs.

...and much more.

Most of the logging is subject to activation.

## Personal data privacy

GDPR and other regulations require "privacy by design".
Because of this, some entities have always-on access logging enabled.

For more information, see @default-logging-levels.

## Read access logging

Logging of read access is a special stand-out feature.
When activated for an entity type, it can log all user access, even through the API.

Read access logging can be invaluable tool for internal investigations.
However, the data storage requirements might not be trivial.
Consult with your implementation company for details.

## Third party logging apps

There are third party apps, which deal with the system logs.

This includes:

* Apps saving the logs to a block-chain secured storage.
* Apps transferring logs to external destinations.

etc.
