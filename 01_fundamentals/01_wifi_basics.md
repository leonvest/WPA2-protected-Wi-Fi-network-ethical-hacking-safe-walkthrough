# Wi-Fi Basics (802.11 Overview)

This section introduces the core concepts needed to understand Wi-Fi labs
before touching any tools or commands.

The goal is **understanding**, not exploitation.

---

## What is Wi-Fi?

Wi-Fi is a family of wireless networking standards (IEEE 802.11) that allow
devices to communicate over radio instead of cables.

A typical Wi-Fi network consists of:
- **Access Point (AP)** – provides network access
- **Client (station)** – your laptop, VM, or lab machine
- **SSID** – the network name broadcast by the AP

---

## SSID

- The **SSID** is the human-readable network name
- Multiple APs can broadcast the same SSID
- An SSID alone does **not** indicate security level

Example:
> SSID: 'Stevewifi' or 'hackerscafe'

---

## Security Modes (High level)

Common Wi-Fi security modes:
- **Open** – no authentication
- **WPA / WPA2 / WPA3** – encrypted and authenticated
- **Enterprise (802.1X)** – uses a backend authentication server

In labs and CTFs, WPA2-PSK is very common.

---

## Stations and Interfaces

On Linux, Wi-Fi adapters appear as network interfaces:
- Examples: `wlan0`, `wlp2s0`, `sta3-wlan0`

Each interface can be:
- DOWN or UP
- DISCONNECTED or CONNECTED
- Associated with exactly one AP at a time

---

## Typical Wi-Fi Connection Flow

Conceptually, connecting to Wi-Fi looks like this:

1) Scan for available networks  
2) Select an SSID  
3) Authenticate (e.g., WPA2 handshake)  
4) Associate with the access point  
5) Obtain IP configuration (DHCP)  

This repo follows **that same logical order**.

---

## Defensive Perspective

From a defensive standpoint:
- Wi-Fi is an **entry point** into the network
- Segmentation and monitoring are critical
- Wireless access should never imply internal trust

---

## Key Takeaway

> Wi-Fi labs are not about “breaking crypto”, but about understanding
> how wireless access integrates into normal IP networking.
