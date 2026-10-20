# User types

For operational and licensing purposes, user accounts are divided in several main types:

## Internal users

The internal users are all users, who create value for the enterprise.
These usually include, but are not limited to:

* Employees
* Sub-contractors
* Partners
* etc.

These users can login in the system and access the data (according to their permissions).

> [!TIP]
> Logged internal users count directly against the licensed concurrent session limits.

## External users

External users are all users, which are related in some way, but do not create value for the enterprise.

These usually include:

* Customers
* Suppliers
* Partners
* Fans
* etc.

External users cannot login directly in the system, but can usually access specialized web views for limited functionality.
The web applications operates with the ERP instance using Application Accounts on behalf of the external users.

> [!TIP]
> External users do not directly count towards the licensed concurrent session limits.
> However, the underlying web applications can consume sessions, usually much less than the operating external users (usually just 1 session).

## Application accounts

Application accounts are special types of users, used by service applications.

They have special kind of non-human login, but are otherwise identical to internal users.

> [!TIP]
> For all licensing and operational purposes, application accounts are considered similar to internal users.

## Virtual users

Virtual users cannot login in the system or access any web content.
Their primary purpose is for temporary assignment of tasks or other internal purposes, requiring user accounts, which are not available at some moment.

> [!TIP]
> Virtual users cannot login and are not counted towards the license limits.