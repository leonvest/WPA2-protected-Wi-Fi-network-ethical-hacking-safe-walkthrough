# 3) Connect using wpa_supplicant (sudoers constraints)

In some labs, sudoers rules:
- allow execution of a command
- but restrict certain flags (e.g., daemon mode)

Learning point:
- A process can be run in the background using the shell (`&`)
  without relying on a restricted flag.

Indicators of success:
- “Associated with …”
- “Key negotiation completed”
- “CTRL-EVENT-CONNECTED”

Report wording example:
> “wpa_supplicant confirmed successful association and WPA key negotiation.”
