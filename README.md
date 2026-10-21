# -Enterprise-Gateways-Firewalls-Cloud-CVEs
A curated collection of hands-on cybersecurity CTF labs covering Citrix Bleed, PAN-OS GlobalProtect, Fortinet SSL VPN, Cisco ASA/IOS XE, F5 BIG-IP, Pulse Secure, VMware vCenter/ESXi, and Oracle WebLogic CVEs from Learn SecByte.
# Learn SecByte CTF & Cybersecurity Labs Collection

Welcome to the **Learn SecByte CTF & Cybersecurity Labs Collection**. This repository is a dedicated, searchable index of hands-on enterprise network gateway, perimeter firewall, SSL VPN appliance, hypervisor infrastructure (VMware ESXi & vCenter), application server (Oracle WebLogic), and load balancer (F5 BIG-IP) CVE exploitation labs—including Citrix Bleed, PAN-OS GlobalProtect, Fortinet FortiOS, Cisco ASA / IOS XE, Pulse Secure, VMware OpenSLP/vCenter, and WebLogic—designed for cybersecurity students, CTF players, vulnerability researchers, SOC analysts, network security architects, and red team operators.

---

## Table of Contents
- [Introduction](#introduction)
- [Lab Collection & Index](#lab-collection--index)
- [Categories](#categories)
- [Learning Path](#learning-path)
- [How to Use the Labs](#how-to-use-the-labs)
- [Disclaimer](#disclaimer)

---

## Introduction

Edge appliances, VPN concentrators, hypervisors, and enterprise middleware represent high-value targets for advanced persistent threat (APT) actors and ransomware groups. Hosted on [Learn SecByte](https://learn.secbyte.org/), this advanced perimeter infrastructure, SSL VPN appliance, virtualized hypervisor, and enterprise application server exploitation collection provides practical, hands-on technical training to audit, reproduce, and mitigate high-impact enterprise vulnerabilities.

From analyzing buffer over-read session token leaks in Citrix NetScaler (`Citrix Bleed`), unauthenticated command injection in Palo Alto Networks PAN-OS GlobalProtect, and administrative URI authentication bypasses in Fortinet FortiOS and F5 BIG-IP to exploiting privilege escalation flaws in Cisco IOS XE Web UI, arbitrary file reads in Pulse Secure, heap overflows in VMware ESXi OpenSLP, unauthenticated RCEs in VMware vCenter, and HTTP header path-traversal bypasses in Oracle WebLogic, these exercises prepare security professionals to defend enterprise infrastructure perimeters.

---

## Lab Collection & Index

Below is the complete, searchable index of all enterprise gateway, SSL VPN, firewall, hypervisor, and application server CVE challenges in this collection:

| # | Lab / Challenge Name | Category | Focus / Key Topics | Lab Link |
|---|----------------------|----------|---------------------|----------|
| 1 | **Citrix Bleed: NetScaler ADC Session Token Leakage** | Enterprise Perimeter, Gateway & SSL VPN CVEs | Buffer over-read vulnerability, session cookie/token memory extraction, multi-factor authentication (MFA) bypass | [Access Lab](https://learn.secbyte.org/ctf/citrix-bleed-netscaler-adc-session-token-leakage) |
| 2 | **Citrix ADC Gateway CVE-2019-19781 Directory Traversal RCE** | Enterprise Perimeter, Gateway & SSL VPN CVEs | Path traversal via HTTP requests, Perl script execution, unauthenticated remote code execution, web shell placement | [Access Lab](https://learn.secbyte.org/ctf/citrix-adc-gateway-cve-2019-19781-directory-traversal-rce) |
| 3 | **PAN-OS GlobalProtect CVE-2024-3400 Command Injection** | Enterprise Perimeter, Gateway & SSL VPN CVEs | Unauthenticated OS command injection in telemetry processing, arbitrary file creation, root remote code execution | [Access Lab](https://learn.secbyte.org/ctf/pan-os-globalprotect-cve-2024-3400-command-injection) |
| 4 | **Fortinet FortiOS SSL VPN CVE-2022-40684 Authentication Bypass** | Enterprise Perimeter, Gateway & SSL VPN CVEs | HTTP request header spoofing (`Report-Runner`), administrative REST API bypass, rogue SSH key injection | [Access Lab](https://learn.secbyte.org/ctf/fortinet-fortios-ssl-vpn-cve-2022-40684-authentication-bypas) |
| 5 | **FortiOS SSL VPN Heap Overflow CVE-2023-27997** | Enterprise Perimeter, Gateway & SSL VPN CVEs | Pre-authentication heap-based buffer overflow in SSL VPN web interface, memory corruption, remote code execution | [Access Lab](https://learn.secbyte.org/ctf/fortios-ssl-vpn-heap-overflow-cve-2023-27997) |
| 6 | **Pulse Secure VPN CVE-2019-11510 Arbitrary File Read** | Enterprise Perimeter, Gateway & SSL VPN CVEs | Pre-authenticated path traversal, arbitrary file disclosure (`/etc/passwd`, plain-text credentials, session keys) | [Access Lab](https://learn.secbyte.org/ctf/pulse-secure-vpn-cve-2019-11510-arbitrary-file-read) |
| 7 | **Cisco IOS XE Web UI CVE-2023-20198 Privilege Escalation** | Network Switch, Router & Firewall CVEs | Unauthenticated HTTP web UI exploit, Level 15 privilege account creation, implants deployment, full device compromise | [Access Lab](https://learn.secbyte.org/ctf/cisco-ios-xe-web-ui-cve-2023-20198-privilege-escalation) |
| 8 | **Cisco ASA CVE-2020-3452 Path Traversal Lab** | Network Switch, Router & Firewall CVEs | Directory traversal in WebVPN/AnyConnect endpoints, arbitrary system file reading, sensitive configuration disclosure | [Access Lab](https://learn.secbyte.org/ctf/cisco-asa-cve-2020-3452-path-traversal-lab) |
| 9 | **F5 BIG-IP TMUI CVE-2020-5902 Remote Code Execution** | Network Switch, Router & Firewall CVEs | Traffic Management User Interface (TMUI) path traversal (`..;`), unauthenticated REST API access, arbitrary command execution | [Access Lab](https://learn.secbyte.org/ctf/f5-big-ip-tmui-cve-2020-5902-remote-code-execution) |
| 10 | **VMware vCenter CVE-2021-21985 RCE** | Virtualization Infrastructure & Application Server CVEs | Unauthenticated remote code execution in vSphere Client plugin (`Virtual SAN Health Check`), JNDI injection, root access | [Access Lab](https://learn.secbyte.org/ctf/vmware-vcenter-cve-2021-21985-rce) |
| 11 | **VMware ESXi OpenSLP CVE-2021-21974 Heap Overflow** | Virtualization Infrastructure & Application Server CVEs | Pre-authentication heap overflow in OpenSLP service (port 427), memory corruption, hypervisor host takeover | [Access Lab](https://learn.secbyte.org/ctf/vmware-esxi-openslp-cve-2021-21974-heap-overflow) |
| 12 | **Oracle WebLogic CVE-2020-14882 RCE** | Virtualization Infrastructure & Application Server CVEs | Unauthenticated HTTP administrative console path traversal (`.png`), handle chaining, arbitrary OS command execution | [Access Lab](https://learn.secbyte.org/ctf/oracle-weblogic-cve-2020-14882-rce) |

---

## Categories

### 1. Enterprise Perimeter, Gateway & SSL VPN Security
Analyze vulnerabilities in enterprise gateways and VPN concentrators, including Citrix Bleed token leakage, PAN-OS GlobalProtect command injection, Fortinet SSL VPN auth bypasses/heap overflows, and Pulse Secure arbitrary file reads.
- [Citrix Bleed: NetScaler ADC Session Token Leakage](https://learn.secbyte.org/ctf/citrix-bleed-netscaler-adc-session-token-leakage)
- [Citrix ADC Gateway CVE-2019-19781 Directory Traversal RCE](https://learn.secbyte.org/ctf/citrix-adc-gateway-cve-2019-19781-directory-traversal-rce)
- [PAN-OS GlobalProtect CVE-2024-3400 Command Injection](https://learn.secbyte.org/ctf/pan-os-globalprotect-cve-2024-3400-command-injection)
- [Fortinet FortiOS SSL VPN CVE-2022-40684 Authentication Bypass](https://learn.secbyte.org/ctf/fortinet-fortios-ssl-vpn-cve-2022-40684-authentication-bypas)
- [FortiOS SSL VPN Heap Overflow CVE-2023-27997](https://learn.secbyte.org/ctf/fortios-ssl-vpn-heap-overflow-cve-2023-27997)
- [Pulse Secure VPN CVE-2019-11510 Arbitrary File Read](https://learn.secbyte.org/ctf/pulse-secure-vpn-cve-2019-11510-arbitrary-file-read)

### 2. Network Switches, Routers, Firewalls & Load Balancers
Audit core routing and firewall management planes, including Cisco IOS XE privilege escalation, Cisco ASA path traversal, and F5 BIG-IP TMUI remote code execution.
- [Cisco IOS XE Web UI CVE-2023-20198 Privilege Escalation](https://learn.secbyte.org/ctf/cisco-ios-xe-web-ui-cve-2023-20198-privilege-escalation)
- [Cisco ASA CVE-2020-3452 Path Traversal Lab](https://learn.secbyte.org/ctf/cisco-asa-cve-2020-3452-path-traversal-lab)
- [F5 BIG-IP TMUI CVE-2020-5902 Remote Code Execution](https://learn.secbyte.org/ctf/f5-big-ip-tmui-cve-2020-5902-remote-code-execution)

### 3. Virtualization Infrastructure & Enterprise Application Servers
Exploit bare-metal hypervisors and middleware application servers, including VMware ESXi OpenSLP heap overflows, VMware vCenter plugin RCEs, and Oracle WebLogic administrative path traversals.
- [VMware vCenter CVE-2021-21985 RCE](https://learn.secbyte.org/ctf/vmware-vcenter-cve-2021-21985-rce)
- [VMware ESXi OpenSLP CVE-2021-21974 Heap Overflow](https://learn.secbyte.org/ctf/vmware-esxi-openslp-cve-2021-21974-heap-overflow)
- [Oracle WebLogic CVE-2020-14882 RCE](https://learn.secbyte.org/ctf/oracle-weblogic-cve-2020-14882-rce)

---

## Learning Path

Follow this structured progression path to master enterprise SSL VPN exploitation, firewall management plane breaches, hypervisor compromise, and middleware RCEs:

1. **Phase 1: Arbitrary File Reads & Path Traversal Flaws** — Master path traversal techniques on Cisco ASA, Pulse Secure, and Citrix ADC:
   - [Cisco ASA CVE-2020-3452 Path Traversal Lab](https://learn.secbyte.org/ctf/cisco-asa-cve-2020-3452-path-traversal-lab)
   - [Pulse Secure VPN CVE-2019-11510 Arbitrary File Read](https://learn.secbyte.org/ctf/pulse-secure-vpn-cve-2019-11510-arbitrary-file-read)
   - [Citrix ADC Gateway CVE-2019-19781 Directory Traversal RCE](https://learn.secbyte.org/ctf/citrix-adc-gateway-cve-2019-19781-directory-traversal-rce)

2. **Phase 2: Authentication Bypass & Privilege Escalation** — Bypass authentication filters on Fortinet FortiOS, Cisco IOS XE, and F5 BIG-IP:
   - [Fortinet FortiOS SSL VPN CVE-2022-40684 Authentication Bypass](https://learn.secbyte.org/ctf/fortinet-fortios-ssl-vpn-cve-2022-40684-authentication-bypas)
   - [Cisco IOS XE Web UI CVE-2023-20198 Privilege Escalation](https://learn.secbyte.org/ctf/cisco-ios-xe-web-ui-cve-2023-20198-privilege-escalation)
   - [F5 BIG-IP TMUI CVE-2020-5902 Remote Code Execution](https://learn.secbyte.org/ctf/f5-big-ip-tmui-cve-2020-5902-remote-code-execution)

3. **Phase 3: Memory Leaks, Command Injections & Heap Overflows** — Analyze memory leaks in Citrix NetScaler (`Citrix Bleed`), command injection in PAN-OS, and heap memory corruption in Fortinet:
   - [Citrix Bleed: NetScaler ADC Session Token Leakage](https://learn.secbyte.org/ctf/citrix-bleed-netscaler-adc-session-token-leakage)
   - [PAN-OS GlobalProtect CVE-2024-3400 Command Injection](https://learn.secbyte.org/ctf/pan-os-globalprotect-cve-2024-3400-command-injection)
   - [FortiOS SSL VPN Heap Overflow CVE-2023-27997](https://learn.secbyte.org/ctf/fortios-ssl-vpn-heap-overflow-cve-2023-27997)

4. **Phase 4: Virtualization Hypervisors & Middleware Servers** — Compromise enterprise management backbones on VMware ESXi, vCenter, and Oracle WebLogic:
   - [Oracle WebLogic CVE-2020-14882 RCE](https://learn.secbyte.org/ctf/oracle-weblogic-cve-2020-14882-rce)
   - [VMware vCenter CVE-2021-21985 RCE](https://learn.secbyte.org/ctf/vmware-vcenter-cve-2021-21985-rce)
   - [VMware ESXi OpenSLP CVE-2021-21974 Heap Overflow](https://learn.secbyte.org/ctf/vmware-esxi-openslp-cve-2021-21974-heap-overflow)

---

## How to Use the Labs

1. Select a challenge link from the index or category sections above.
2. Read the scenario directives, firmware/software version specs, and vulnerability parameters on [Learn SecByte](https://learn.secbyte.org/).
3. Deploy analysis toolsets (Burp Suite, Python, Metasploit, Curl, OpenSSL CLI, Scapy, GDB) inside an isolated workstation.
4. Execute memory dump scripts, manipulate HTTP request headers, craft path traversal URIs, trigger remote code execution, and capture target flags.

---

## Disclaimer

This repository and its linked challenge resources are strictly intended for educational, threat research, and authorized technical security training purposes. Never deploy real-world enterprise CVE exploits, memory extraction scripts, or remote code execution payloads against unauthorized network appliances, perimeter firewalls, cloud hypervisors, or production systems.
