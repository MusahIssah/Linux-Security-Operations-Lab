# Linux Security Operations Lab

I’m building a hands-on Linux administration and security lab using Windows 11, Hyper-V, and Red Hat Enterprise Linux 9.8.

This repository documents my progress through practical exercises, commands, troubleshooting notes, and screenshots. Each completed milestone builds toward operating, securing, and maintaining Linux servers.

## Lab environment

- **Host:** Windows 11 with Hyper-V
- **Guest:** Red Hat Enterprise Linux 9.8
- **Server:** `linux-test`
- **Network:** Hyper-V Default Switch
- **Administration:** SSH from Windows PowerShell

## Project series

| Part | Topic | Status |
|---|---|---|
| [01 — Remote Administration and Log Integrity](./01-remote-administration/README.md) | Network configuration, SSH, administrative access, authentication logs, SCP, and SHA-256 verification | Completed |
| [02 — Linux File Ownership and Permissions](./02-file-permissions/README.md) | File modes, directory access, deletion controls, umask, and group-based access tests | Completed |
| 03 — Patching and Change Control | Update assessment, change documentation, validation, and recovery planning | Planned |
| 04 — Vulnerability Management | Nessus scanning, finding analysis, remediation, and rescanning | Planned |

## Completed milestone: Part 1

- Enabled automatic network connection for the Linux VM.
- Connected from Windows to Linux over SSH and verified the host-key fingerprint.
- Confirmed the server identity, user account, and sudo access.
- Reviewed SSH authentication logs and distinguished connection sources.
- Saved login logs and transferred the evidence to Windows using SCP.
- Compared SHA-256 hashes to verify that the transferred file matched the original.

[View the commands, results, and screenshots for Part 1](./01-remote-administration/README.md).

## Current limitation

Red Hat subscription registration remains unresolved. The web console shows an active Developer subscription, but the registration service does not recognize an accessible organization for the account. Subscription-backed patching has not yet been demonstrated.

## Scope

This is a personal learning environment. Completed work is supported by evidence within each milestone; planned topics are not claims of completed experience. The screenshots use private lab IP addresses.
