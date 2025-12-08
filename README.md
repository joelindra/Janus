

# Janus Web Shell v6.1

<img width="1982" height="822" alt="image" src="https://github.com/user-attachments/assets/9b40e8e7-cc59-422d-b74f-38abd531dcf0" />

<div align="center">

![Version](https://img.shields.io/badge/version-6.1-blue.svg)
![PHP](https://img.shields.io/badge/PHP-7.0%2B-purple.svg)
![License](https://img.shields.io/badge/license-Authorized%20Use%20Only-red.svg)

**Advanced PHP Web Shell with modern UI, defense, and post-exploitation tooling**

[Features](#-features) • [Install](#-installation) • [Usage](#-usage) • [Changelog](#-changelog) • [Warning](#-warning)

</div>

---

## 📋 Description

Janus is a full-featured PHP web shell for authorized red-team operations and system administration. The v6.1 release keeps the modern single-page UI and adds deeper discovery, privilege-escalation helpers, encryption tooling, and stronger WAF evasion.

### Highlights
- 🎨 Modern dark UI with fast single-page interactions
- 🛡️ Auto-Defend + Anti-Delete with multi-location backups
- 🌐 Network stack: reverse/bind shells, port scan, pivoting, DNS tunnel, C2
- 🗄️ File ops at scale: mass upload, compare, monitor, exfil packager
- 🧠 Post-exploitation: privesc checks, exploit suggester, password cracker
- 🔐 HADES encryption, ransomware builder/decryptor, code obfuscator
- 🧭 80+ modules spanning discovery, persistence, stealth, and automation

---

## ⚠️ Warning

> **Authorized use only.**
> Operating this shell on systems without explicit permission is illegal. You are solely responsible for all actions and outcomes when using this tool.

---

## 🎯 Features

### Access, Defense, Stealth
- Auto-Defend `.htaccess`/PHP fallback with secret token
- Anti-delete watchdog + multi-location backup installer
- Log cleaner, advanced multi-log cleaner, log evasion, process hiding
- Notifications center, self-destruct, system tools (phpinfo), real-time file watcher
- Open_basedir bypass generator; security headers and secret token gate

### File & Data Operations
- File manager with breadcrumb, search (basic/advanced), selection, delete
- File preview & file comparison views
- In-browser editor, code templates, steganography helper
- Mass uploader (multi-dir), batch file execution
- Wget/downloader, git integration helper
- File/dir change monitor; activity log; performance view
- Data exfiltration packager (ZIP); sensitive file finder
- File encryption/decryption (AES) plus HADES multi-layer/ransomware encrypt/decrypt

### Command & Execution
- Terminal with multi-method execution & fallback
- PHP code evaluator; memory-only PHP execution (no drop)
- Command aliases manager; key management; service manager
- Batch runner, env manager, system command chaining

### Network, Pivoting, C2
- Port scanner; reverse shell; bind shell with connection helper
- Port forwarding/pivot tool; internal subnet scanner
- Packet capture (tcpdump), DNS tunneling
- Firewall view/flush; DoS/CPU hog tester
- C2 communication helper

### Discovery & Intelligence
- Dashboard: live stats, system info, cwd, green/writable dirs
- System profiler; server fingerprint; user/OS info; kernel info
- Domain intelligence (DNS, reverse IP, subdomains)
- Credential harvester; content search (grep); config grabber
- File watcher; activity log; performance monitor
- Process manager; user context & sudo check

### Privilege Escalation & Persistence
- Privesc checker (Linux/Windows); exploit suggester
- Privilege scanners: SUID/GUID finder; world-writable finder
- Cron manager; SSH key manager; `.htaccess` prepend persistence
- Multi-location backup; process hiding; log evasion; notifications

### Database & CMS
- Database client (MySQLi); database dumper; column dumper
- WordPress admin creator; config finder
- cPanel toolkit: symlinker, credential finder, reset/contact helper
- WHMCS decoder; fake mail sender

### Payloads & Backdoors
- Code injector; backdoor installer; memory execution; payload templates
- Shell generator + shell finder (JANUS identifier)
- Phishing page deployer; password cracker + wordlist generator
- WAF bypass tester; code obfuscator; DNS tunnel/C2 comms; ransomware builder/decryptor

---

## 📦 Installation

### Requirements
- PHP 7.0+
- Apache/Nginx with PHP enabled
- Write permission where the shell is placed

### Quick Start
1) Upload `janus-ori.php` (rename to `janus.php` if you prefer a shorter name).
2) Set safe permissions:
```bash
chmod 644 janus-ori.php
```
3) Browse to the file:
```
http://your-server/janus-ori.php
```
4) First access auto-enables protection, generates secret token, and drops backups/watchdog files for anti-delete.

---

## 🚀 Usage Overview
- File manager: browse, edit, upload/download, compare, mass upload.
- Terminal: run commands with multi-method fallback; use PHP Eval for inline PHP.
- Network: port scan, reverse/bind shell, pivot/port-forward, DNS tunnel, packet capture.
- Database: run MySQL queries, dump DB/columns, create WP admin.
- Discovery: credential harvester, config grabber, domain intel, fingerprinting, exploit suggestions.
- Persistence/stealth: cron manager, SSH key manager, `.htaccess` prepend, log evasion, process hiding, multi-backup.
- Payloads: generate shells, inject/backdoor files, phishing deployer, HADES encryption/ransomware, password cracking.

---

## 🛡️ Security Notes
- Protect access: use the generated secret token and restrict via `.htaccess` where possible.
- Clean traces: use log cleaner/advanced cleaner after high-noise actions.
- Persistence is detectable: backups, cron, `.htaccess` prepend, and key installs can trigger alerts.
- Network tools may be rate-limited or blocked by local firewalls/WAF.

---

## 🔄 Changelog

### v6.1
- Stronger WAF evasion defaults and encoding fixes.
- New/expanded modules: domain intelligence, privesc checker, subnet scanner, firewall control, phishing deployer, server fingerprint, cPanel toolkit (symlinker/creds/reset/contact), WHMCS decoder, fake mailer.
- Added pivoting/port forwarder, DNS tunneling, packet capture, memory-only execution, ransomware encrypt/decrypt (HADES 13-layer), process hiding/log evasion, multi-backup UI, shell generator/finder.
- UI polish, multi-method execution stability, better notifications and performance view.

### v6.0
- Modernized UI and auto-defend improvements.
- Anti-delete upgrades and broader feature coverage.

---

## 📚 Reference
- Key routines: `setup_auto_defend()`, `setup_anti_delete()`, `hades_encrypt()`, WAF evasion encoders, execution fallbacks.
- API-style actions remain POST-based (see code for `action` switch in `janus-ori.php`).

---

## ⚖️ License & Disclaimer

Educational and authorized use only.
You are fully responsible for compliance with local laws and for any impact caused by this software.

---

## 👤 Author

Joel Indra — [@joelindra](https://github.com/joelindra)

---
