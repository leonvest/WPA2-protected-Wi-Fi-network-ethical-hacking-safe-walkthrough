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

## Defensive considerations
- Restrict allowed sudo commands carefully
- Monitor association and DHCP activity
- Segment Wi-Fi networks and limit exposed services
