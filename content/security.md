---
date: "2024-07-19T13:50:32+10:00"
draft: false
images:
- images/security-header.webp
title: Hardened Security
description: "Trimclient is designed from the ground up with security as its foundation: a multi-layered, default-deny architecture built specifically for high-accountability environments."
url: /security
---

Trimclient employs a [multi-layered default-deny](https://en.wikipedia.org/wiki/Defense_in_depth_(computing)) security policy throughout. Each layer is designed to operate independently, so that if one mechanism is bypassed, the layers beneath it continue to protect the system. No single point of failure exposes the environment to risk.

The capabilities described on this page are available across all Trimclient deployments. Which are enabled, and how strictly they are applied, depends on the requirements of the deployment: different environments, cohorts, and organisations will configure the platform differently. A call centre and a youth detention facility will share the same underlying architecture while presenting very different experiences to their respective users.

The security architecture covers the full stack: desktop hardware, physical peripherals, server infrastructure, network topology, device connectivity, and media access. Each is addressed by design, not by policy alone.

## Desktop security

Trimclient desktops can fully operate without any local writable storage; no hard drive, no USB storage, no writable optical media. The operating environment is read-only and immutable. Users cannot install software, modify system configuration, or persist any changes across sessions. The desktop state is identical at every login.

This architecture makes the desktops inherently resistant to malware, keyloggers, spyware, and any attempt at unauthorised software installation. Not because of antivirus software, but because there is nothing to write to.

## Physical security

Trimclient runs on standard commercial off-the-shelf desktop hardware. There is no proprietary client device; facilities can use hardware from their preferred vendor, existing stock, or equipment repurposed from another division.

Forbidden peripherals (hard drives, cameras, microphones, WiFi adaptors, and similar) are disabled at the kernel level. The hardware may physically contain these components, but they are inaccessible to the operating environment. In higher-security deployments, physical removal of these components provides an additional layer of assurance, but it is not a requirement for a secure Trimclient installation.

Firmware is configured to prevent booting from unapproved media, ensuring the managed operating environment cannot be bypassed at startup.

## Server security

Each user's file storage is isolated on the servers, accessible only to that user and to authorised staff. Users cannot access each other's data, and no shared storage exists that could be used to pass files between users.

Staff retain full visibility and access to all user storage. Archival snapshots with a managed retention policy additionally allow staff to access files that have since been deleted by users.

## Network security

The management console is protected against intrusion from unauthorised users and unauthorised network locations. All system authentication is encrypted in transit. The user network and the staff network are architecturally separated; staff systems are not reachable from user desktops under any circumstances.

## Device and media security

Trimclient operates on an explicit allow-list model for connected devices. Any device not on the approved list (USB storage, mobile broadband adaptors, WiFi controllers, webcams, Bluetooth transceivers) is rejected at connection and triggers an immediate staff alert. This is enforced through software policy rather than hardware customisation, with the exception of insecure components such as hard drives and webcams which are physically removed from desktops prior to deployment.

Optical media follows the same model. Users can only access discs that have been explicitly approved by staff. Any attempt to use unapproved media triggers a staff alert.

## Event logging and monitoring

All user sessions are logged in full. Staff can review session logs retrospectively, monitor desktops in real time, broadcast alerts to individual or groups of users, and remotely control or shut down any desktop without physical access to the room.

> "Security best practices aren't aspirational goals, they're the baseline of professional competence. They aren't the ceiling you reach for, they're the floor you stand on."
>
> — Barry Anderson, Security Architect, Cisco Systems
