# 4) DHCP, IP address, and link verification

Goal:
- Obtain a valid IPv4 address via DHCP
- Confirm the interface is connected to the expected SSID

Checks (conceptual):
- Does the interface have an IPv4 address?
- Is the link status reported as ‘Connected’?

Note:
- DHCP messages indicating an existing address may simply mean a lease already exists.

Report wording example:
> “The interface received a DHCP address and link status confirmed connection to SSID X.”
