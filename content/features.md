---
date: "2024-07-19T13:52:10+10:00"
draft: false
images:
- images/workstation-header.webp
title: Features
description: "An overview of Trimclient's core capabilities: central management, IPTV and media, filtered web and email, print management, and content delivery."
url: /features
---

Trimclient was developed for adult corrections and is now deployed across a range of managed environments, including youth detention, mental health facilities, call centres, and others. The capabilities described on this page are available across all deployments; which are enabled, and how they are configured, depends on the requirements of the site. A call centre and a youth detention facility share the same underlying platform while presenting very different experiences to their respective users (referred to throughout as "residents" or "clients" depending on your environment).

# Secure central management

Authorised staff can manage site policies and user desktops from a secure central location. Users cannot circumvent policy or access capabilities beyond what staff have explicitly permitted.

Trimclient is designed to give staff flexibility. Routine tasks and many responses to incidents can be handled remotely, without requiring a room visit. This reduces workload and avoids placing staff in unnecessarily difficult situations.

Each desktop can be assigned to a designated user or group of users, allowing staff to implement access or privilege systems without requiring physical access to rooms. Desktops can be grouped into categories (known as realms), each with its own application set, access policy, and curfew schedule, allowing a single Trimclient deployment to serve different wings, wards, or functions with appropriately different configurations managed from the same console.

## Enforced curfews

Desktop access is restricted according to a predefined schedule. During curfew periods users cannot access the system; access is restored automatically when the curfew lifts.

Individual services (television, printing, web browsing) can have independent curfew schedules applied, giving staff granular control over which capabilities are available at any given time.

## Passive discipline

Staff can suspend individual user privileges (email, television, web access, and others) directly from the management console, without visiting the room. Suspensions can be applied to individual users or to groups.

## Consolidated device

Trimclient consolidates television, radio, education, email, web access, and entertainment into a single managed unit per room, replacing the collection of discrete devices that would otherwise need to be individually secured, monitored, and maintained. [More on why consolidation matters.](/why-consolidated)

## Desktop and software management

From the secure console, staff can broadcast alerts to individual users or groups, remotely monitor or control any desktop, and power up, shut down, or entirely disable individual desktops or groups — all without a room visit where the situation allows it.

Trimclient runs applications on the local desktop hardware while preventing users from accessing the underlying operating system or modifying any software.

---

> Trimclient puts the power of system management squarely in the hands of staff, allowing them to perform their duties remotely and efficiently.

---

# Integrated IPTV and media

Free-to-air television and radio content is distributed to user desktops, with staff able to block specific programmes or channels that conflict with site policy. Content can also be cached and time-shifted for scheduled delivery.

## Closed-circuit channels

Facilities can broadcast video and audio on internal channels accessible to all or selected users. Typical uses include educational content, induction material, time-shifted free-to-air programming, and information services.

## Media restrictions

Where desktops are equipped with optical drives, users can access audio CDs and video DVDs that have been explicitly approved by staff. Unapproved optical media is rejected automatically. All USB storage devices are blocked regardless of content.

Staff are encouraged to use internal IPTV channels for media distribution where possible. This provides greater control, removes the handling of physical media, and eliminates physical media as a potential source of policy violations.

---

# Filtered web and email

## Email

The email system is configurable from no restrictions through to full monitoring and archiving, on a per-user or per-cohort basis.

Where monitoring is enabled, staff have individual control over each user's correspondence. Each user has their own approved addressee list, which staff can configure independently. Addresses can be designated as privileged (delivered without staff review, such as legal representatives) or trusted (with attachments permitted, such as education providers). All other correspondence is subject to deep content filtering.

Each message, both inbound and outbound, passes through the filtering mechanism before delivery. Messages that fail the filter are automatically quarantined for staff review; staff can approve or reject them before delivery.

The filtering mechanism handles the substantial majority of correspondence automatically. All non-privileged correspondence is archived regardless of filter outcome, giving staff full visibility of user communications at any time.

## Web access

Users can be selectively granted access to a limited list of approved websites, such as distance education providers or approved external resources. Attempts to access unapproved sites are blocked and logged.

---

# Print management

Where print monitoring is required, documents printed by users are watermarked with the identity of the user who printed them, regardless of the application used. Electronic copies are retained automatically in secure storage, inaccessible to users, for staff review.

---

# Content delivery

Trimclient supports the secure delivery of educational content from both local providers and online sources. Applications covering basic literacy and numeracy through to vocational and tertiary programmes can be offered through the platform, giving users access to the tools they need for education, skills development, and meaningful engagement.
