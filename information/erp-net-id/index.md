# Get to Know **@@name ID**

***@@name ID** gives you one unified global personal account for signing in to supported **@@name** services and maintaining a consistent identity across the **@@name** ecosystem.*

## Overview

**@@name ID** is your personal global account for signing in to supported **@@name** services.

<img width="574" height="454" alt="Sign-in form with the @@name ID button" src="https://github.com/user-attachments/assets/25f58caf-9a0d-4e7d-86f9-464913fa04af" />

Instead of creating a separate account for each service, you use one profile to keep a consistent identity across the **@@name** ecosystem.

**@@name ID** accounts are issued and authenticated by **@@name Identity**, which acts as the OpenID Connect identity provider for the **@@name** ecosystem.
Applications that support **@@name ID** sign-in redirect users to **@@name Identity**, authenticate them there, and receive standard identity claims (such as the unique user identifier, email, and name) in return.

**@@name ID** helps organizations keep one consistent identity per user across services.

## Use **@@name ID** Across Supported Services

You can use **@@name ID** with services that support **@@name ID** authentication.

Supported services include:

* **[Operator.net](https://operator.net/)** — the AI interface for operating the **@@name** ecosystem through custom-built AI agents and tailored apps.
* **[@@name Marketplace](https://marketplace.erp.net/)** — the marketplace for apps, packaged solutions, integrations, and services.
* **Marketplace Apps** — individual applications delivered through **@@name Marketplace** that accept **@@name ID** as their sign-in method.
* **[Vox](https://vox.erp.net/)** — the portal for submitting, viewing, and voting on user feature ideas, development suggestions, and business cases.
* **Your @@name instance** — when **@@name ID** sign-in is enabled on the instance and your instance user's email matches your **@@name ID** email.
* **Other @@name services** — when they support **@@name ID** authentication.

## Understand What **@@name ID** Does

**@@name ID** provides the sign-in identity that supported **@@name** services use to associate your activity with your personal profile.

Each **@@name ID** account holds:

* **Full name** — your display name across services.
* **Email address** — your sign-in handle and primary contact channel.
* **Password** — the credential you use to sign in.
* **Optional profile information** — phone number, default language, company, and a registration message.

When you sign in, **@@name Identity** creates an authenticated session and shares your identity claims with the service you're signing in to. The session is managed by **@@name Identity** and the service, not stored as part of the account itself.

## Identify the Benefits for Users and Organizations

**@@name ID** is most useful when you work with more than one **@@name** service.

A single personal account helps you move between **Operator.net**, **@@name Marketplace**, **Marketplace Apps**, **Vox**, and **enabled @@name instances** while keeping the same identity and profile details.

### For users

**@@name ID** helps you:

* sign in with one personal account;
* avoid duplicate or inconsistent accounts;
* work across services with less account-related friction.

### For organizations

When team members register their **@@name ID** with their work email, organizations benefit from:

* one consistent identity per person across **@@name** services;
* faster onboarding — a new hire can sign in to every supported **@@name** service from the same account;
* a single verified email per user for access reviews and support requests.

> [!NOTE]
> **@@name ID** is always a personal account. It does not represent organizational membership on its own.
> Linking users to a specific **@@name** instance, marketplace tenant, or organizational role is handled by each service's own access settings.

## Learn How Access Works After Sign-In

After sign-in, each service uses your **@@name ID profile** according to its own access settings, enabled features, and permission rules.

This allows one **@@name ID account** to work across multiple services, while each service or **@@name** instance still controls its own access rules.

Access can depend on:

* whether the service supports **@@name ID** authentication;
* whether your **@@name ID** account is active;
* whether **@@name ID** sign-in is enabled on the **@@name** instance you're trying to access;
* your assigned permissions;
* administrator approval, where required.

> [!NOTE]  
> **@@name ID** supports sign-in and identification.
> Service access and **@@name** instance permissions are managed according to the relevant service, organization, and administrator settings.

## Summary and Additional Resources

**@@name ID** helps you sign in to supported **@@name** services with one global personal account. 
It is especially useful when you work across multiple **@@name** entry points.

### Next Topics:

* **[Create and Use Your @@name ID Through Operator.net](~/information/erp-net-id/register-and-sign-in-to-your-erp-net-id-account.md)**
* **[Following Best Practices for Your @@name ID Account](~/information/erp-net-id/following-best-practices-for-your-erp-net-id-account.md)**

### Related Services:

* **[Operator.net](https://operator.net/)**
* **[@@name Marketplace](https://marketplace.erp.net/)**
* **[Vox (Feedback Portal)](https://vox.erp.net/)**
