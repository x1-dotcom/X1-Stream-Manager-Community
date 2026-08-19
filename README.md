<p align="center">
  <img src="./assets/x1-stream-manager-hero.svg" alt="X1 Stream Manager Community" width="100%" />
</p>

<p align="center">
  <strong>SELF-HOSTED · COMMUNITY · FULLY FUNCTIONAL</strong>
</p>

# X1 Stream Manager Community

**X1 Stream Manager Community** is a public, self-hosted stream-management project from X1.

It is designed for operators who need a practical control layer for **authorized live-stream sources**, playlist delivery, customer/line access and compatible playback workflows.

> **Free means functional.**
> This public release is intended to be useful as released. It is not a deliberately crippled demo built around paid unlocks.

---

<p align="center">
  <img src="./assets/x1-stream-manager-flow.svg" alt="X1 Stream Manager delivery flow" width="100%" />
</p>

## What it does

- Manages configured live-stream sources from one self-hosted interface.
- Generates and serves managed playlist outputs.
- Provides customer/line access management.
- Supports expiring access credentials and channel/package assignment.
- Exposes compatibility endpoints for supported IPTV-client workflows.
- Includes browser-facing playback and operational status tooling.
- Runs on a standard PHP hosting stack without requiring a large external platform.

The focus is operational simplicity: **configure → authorize → deliver → monitor**.

---

## X1 Community position

This repository is part of the **public X1 software family**.

It is separate from the private X1 IPTV Platform, X1 SaaS and other commercial X1 systems. Public X1 projects are not presented as incomplete modules that require a commercial platform to become usable.

**This project can stand on its own.**

---

## Requirements

A typical deployment requires:

- PHP 8.x
- a web server such as Nginx, Apache or Caddy
- PHP cURL / JSON / mbstring / zlib / OpenSSL support
- write access for the application's local data directory

Exact compatibility can vary by environment. Validate the project in your own server stack before production use.

---

## Basic installation

1. Download or clone the repository.
2. Place the application in the intended web root.
3. Make the required writable data path available to the web-server user.
4. Open the application and complete the first-run setup.
5. Configure only sources and endpoints you are authorized to use.

Example permission command on a conventional Linux deployment:

```bash
chmod -R 775 data/
```

Do not apply broad permissions blindly on shared or hardened servers; use the minimum permissions required by your deployment model.

---

## Access and delivery model

X1 Stream Manager separates the operator-facing control layer from client-facing delivery.

The operator controls configured sources, access rules, lines and playlist outputs. Clients consume only what the operator has explicitly made available to them.

<p align="center">
  <img src="./assets/x1-stream-manager-boundary.svg" alt="X1 Stream Manager responsibility boundary" width="100%" />
</p>

---

## Content and rights

This software does **not** grant rights to third-party streams, channels or media.

Use it only with content, endpoints and services that you are legally authorized to access, manage, relay and distribute.

X1 provides the management software. The operator remains responsible for the sources configured in the installation and for compliance with applicable laws, service terms and distribution rights.

---

## Security direction

For any Internet-facing deployment:

- run behind TLS;
- restrict administrative access;
- use strong unique credentials;
- keep PHP and the host OS patched;
- isolate writable application data appropriately;
- monitor access logs and abnormal traffic;
- back up configuration before upgrades.

A public repository is not a substitute for proper server hardening.

---

## X1 design rule

**CONTROL THE SOFTWARE.**  
**KNOW THE SOURCE.**  
**AUTHORIZE THE ACCESS.**  
**DELIVER ONLY WHAT YOU ARE ALLOWED TO DISTRIBUTE.**

<p align="center">
  <strong>X1 // STREAM OPERATIONS</strong><br>
  <strong>FREE MEANS FUNCTIONAL.</strong>
</p>
