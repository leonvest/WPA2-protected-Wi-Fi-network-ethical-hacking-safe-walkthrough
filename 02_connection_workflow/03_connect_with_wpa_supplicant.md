# Case Study (Sanitized): WPA2 Wi-Fi Access → Internal Web Service

## Summary
In a lab environment:
- A WPA2-protected SSID was identified
- Successful association and handshake granted network access
- The client obtained valid IP configuration
- An internal web service was reachable from the Wi-Fi network
- The web service exposed sensitive content in its response

## What made the scenario vulnerable
- Internal service exposure to the Wi-Fi segment
- Lack of strong authentication on the service (or weak access controls)
- Insufficient segmentation between “Wi-Fi clients” and “internal services”

## Evidence an analyst would collect
- SSID and security type (WPA2/RSN)
- Proof of connection (handshake success + link status)
- Proof of IP configuration (address + gateway)
- Proof of reachable service (response status, headers, screenshot)

## Defensive takeaway
Connecting to Wi-Fi should not grant broad reachability to internal services.
Treat Wi-Fi as an untrusted network zone by default.
