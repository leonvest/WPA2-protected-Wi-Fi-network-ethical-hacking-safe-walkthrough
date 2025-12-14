# Logging & Alerting Recommendations

## Wireless controller / AP
- Log associations and deauth events
- Alert on first-time devices connecting to sensitive SSIDs
- Alert on repeated failed auth attempts per device

## DHCP/DNS
- Keep lease logs
- Alert on unusual lease churn
- Monitor DNS queries from Wi-Fi ranges for internal admin hostnames

## Web / reverse proxy
- Log source networks and user agents
- Alert on access to internal-only services from Wi-Fi segments
- Add rate limits and authentication where appropriate
