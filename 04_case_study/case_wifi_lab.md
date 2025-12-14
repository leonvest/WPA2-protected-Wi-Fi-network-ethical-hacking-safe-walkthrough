# Case Study: WPA2 Wi-Fi Lab

## Summary
1) Scanned Wi-Fi networks and identified SSID and RSN (WPA2)
2) Created and secured a WPA configuration file
3) Connected using wpa_supplicant while handling sudoers restrictions
4) Obtained and verified IP configuration and link status
5) Identified an internal web service using limited manual validation
6) Retrieved the page and confirmed the presence of the flag

## Why this worked
- Only allowed commands were used
- WPA handshake and link status confirmed connectivity
- DHCP provided valid network configuration
- Service discovery was targeted and minimal




# Segmentation Strategy (Defensive)

Goal: even if an attacker connects to Wi-Fi, they should NOT reach internal services.

Principles:
- Treat Wi-Fi clients like “untrusted endpoints”
- Enforce explicit allow-lists
- Separate:
  - guest Wi-Fi
  - employee Wi-Fi
  - admin/management networks
  - server networks

Validation (defensive):
- Periodically test that Wi-Fi ranges cannot reach internal admin portals
- Monitor firewall rule drift and document changes
