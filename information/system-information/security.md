# Security in @@name

## Access Keys

The security system in @@name is based on **Access Keys**.

Many types of resources can be protected with keys:

* Subsystems
* Entity types
* Individual records
* Individual attributes
* Visuals, like forms, panels, etc.
* etc.

To access a protected resource, the user must possess the required access key.

## User Groups

Permissions are managed through User Groups.
A user group gives access to a list of access keys.
The members of the user group receive access to all keys in the group.

> [!note]
> There is no way to revoke access to specific access key for specific user.
> When a user is added to a security group, they receive all keys.
> Design carefully your security framework, so that revoking is not required.

## Action permissions

Access keys give general permission to access a resource.
This gives the permission to retrieve the resource from the database.

However, this might not give permission for specific operations (actions) over the resource.

Each resource type has a pre-defined set of actions, which might require permissions.
When a security group is assigned an access key, the assignment also specifies which actions are allowed.

Basic actions, which most data resource types define are:

* Update
* Delete

> [!note]
> Read is included in the access key.
