---
layout: page
permalink: /privacy/
title: Privacy Policy
description: How Grupa collects, uses, shares, and deletes your personal data.
---

**Effective {{ site.legal.effective_date }}**

This policy explains what {{ site.legal.entity }} ("Grupa", "we", "us") collects when you use the Grupa mobile app and this website, why we collect it, who else sees it, and how long we keep it.

Grupa is a shared app. Almost everything you do in it — tasks, messages, group membership — is meant to be seen by the other people in your group. This policy is mostly about what happens to that data beyond your group, and about what remains when you leave.

## What we collect

**Account information.** When you create an account we store an email address and a username. If you sign in with Google or Apple, we receive your email address, your name, and a stable identifier from that provider, and we store a link between your Grupa account and your provider account. If you sign in with a password instead, we store a cryptographic hash of it, never the password itself.

**Profile information you choose to add.** First and last name, a display name, phone number, gender, and date of birth. These are optional, and you can leave them blank.

**Content you create.** Groups you belong to, tasks you create or are assigned, task titles, descriptions and due dates, invitations you send or receive, chat messages you send, any images or files you attach to a message, and which messages you have read.

**Technical information.** Our servers record ordinary request logs — IP address, timestamp, the endpoint called, and the app version and device type — for security, debugging, and abuse prevention.

## What we do not do

We do not sell your personal data. We do not share it with advertisers, we do not run ads in Grupa, we do not use your messages or tasks to build an advertising profile, and we do not use third-party analytics or tracking SDKs in the app.

## How we use it

To run the service: authenticating you, showing your groups and tasks to the right people, delivering chat messages, and tracking what you have read so unread counts work. To keep the service secure and to investigate abuse. To respond to you when you contact support. And to meet our legal obligations.

If you are in the EEA or UK, our legal bases are: **performance of a contract** for everything needed to operate your account and deliver the app; **legitimate interests** for security, abuse prevention, and debugging; **consent** where we ask for it specifically, such as push notification permission; and **legal obligation** where a law requires us to keep or produce something.

## Sign in with Google

If you use Google to sign in, Grupa requests only your basic profile: your name, email address, profile picture, and Google account ID. We use these solely to create and identify your Grupa account. We do not request access to your Gmail, Drive, Calendar, or Contacts.

Grupa's use and transfer of information received from Google APIs adheres to the [Google API Services User Data Policy](https://developers.google.com/terms/api-services-user-data-policy), including the Limited Use requirements.

You can disconnect Grupa from your Google account at any time in your [Google account permissions](https://myaccount.google.com/permissions). Doing so stops you signing in with Google; it does not delete your Grupa account.

## Sign in with Apple

If you use Apple to sign in, we receive your name and either your email address or Apple's private relay address, depending on what you chose. We use these the same way as above. When you delete your Grupa account, we also revoke your Sign in with Apple token with Apple.

## Who else sees your data

**Other members of your groups.** This is the main one. Your display name, and any tasks, messages, and attachments you add to a group, are visible to everyone else in that group. Anyone can be added to a group by an existing member, so treat a group the way you would treat a group chat.

**Our infrastructure providers.** Grupa runs on Heroku (Salesforce), which hosts our application servers and our PostgreSQL database in the United States. Heroku processes this data on our instructions and does not use it for its own purposes.

**Google and Apple**, for identity, as described above.

**This website** loads fonts from Google Fonts, which means Google receives your IP address when you view a page. The app itself does not do this.

We may also disclose data if we are legally required to — a court order, a lawful request from an authority — or where it is necessary to protect someone's safety or our legal rights. We will tell you when we are permitted to.

## International transfers

Our servers are in the United States. If you use Grupa from the EEA or the UK, your data is transferred there. Where required, these transfers rely on the European Commission's Standard Contractual Clauses.

## How long we keep it

While your account is open, we keep your data for as long as you use Grupa. Server logs are kept for a short operational window and then rotated out.

## Deleting your account

You can delete your account from inside the app, under Settings. We want to be exact about what that does, because "we delete everything" would not be true.

**Deleted outright:**

- Your email address, username, first and last name, display name, phone number, gender, and date of birth.
- Your password hash and all active sessions and refresh tokens.
- The links between your Grupa account and your Google or Apple account. Your Sign in with Apple token is revoked with Apple.
- Your read-tracking data.
- The copy of your name and email address held by our task service.

**Retained, with your identity removed:**

- An empty account record, keyed only by an internal identifier, recording that an account existed and when it was deleted. This is an audit record and contains no personal details.
- Tasks and groups you created. Other members are still using them, so they remain and show as created by a deleted user.
- **Chat messages you sent, including their text and any attachments.** Your name is removed and they render as coming from a deleted user, but the content stays, so that conversations other members are still reading remain intact.

That last point is the one to read twice. If you have posted something in a chat that you specifically want erased — a phone number, an address, anything you would not want to persist — deleting your account will not remove it. Email us at [{{ site.legal.contact_email }}](mailto:{{ site.legal.contact_email }}) and we will erase the content itself.

Deletion of your profile is immediate. Removing your details from our task and chat services is currently done as a separate step and may take a few days to complete.

Deleted data also persists in our routine database backups for up to {{ site.legal.backup_retention }}, after which those backups expire. If we ever restore from a backup, we re-apply deletions afterwards.

## Your rights

Depending on where you live, you have some or all of the following rights: to access the data we hold about you, to correct it, to delete it, to receive a copy in a portable format, to object to or restrict certain processing, and to withdraw consent you have given.

Most of these you can exercise directly in the app — edit your profile, or delete your account. For anything else, email [{{ site.legal.contact_email }}](mailto:{{ site.legal.contact_email }}). We will respond within one month.

We do not discriminate against you for exercising these rights. If you are in the EEA or UK and you are unhappy with how we have handled a request, you can complain to your local data protection authority.

## Children

Grupa is not intended for children under 13, or under 16 in the EEA and UK. We do not knowingly collect data from them. If you believe a child has created an account, email us and we will remove it.

## Security

We serve all traffic over HTTPS, hash passwords, store data in a managed database that is not publicly reachable, and restrict access to production systems to the people who need it.

To be clear about what we do **not** do: Grupa messages are not end-to-end encrypted. They are encrypted in transit and at rest, but we hold the keys, which means we are technically capable of reading message content and are obliged to produce it under a valid legal order. No system is perfectly secure, and we cannot guarantee absolute security.

## Cookies

This website sets no cookies and runs no analytics. The mobile app stores authentication tokens on your device so you stay signed in; these are not advertising identifiers and are cleared when you sign out.

## Changes

We will update this page when our practices change, and we will change the effective date at the top. For material changes we will notify you in the app or by email before they take effect.

## Contact

Questions, requests, or complaints: [{{ site.legal.contact_email }}](mailto:{{ site.legal.contact_email }}).

{{ site.legal.entity }}, {{ site.legal.address }}
