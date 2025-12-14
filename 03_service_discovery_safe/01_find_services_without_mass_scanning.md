# 5) Service discovery without mass scanning

In CTFs it is common to scan an entire subnet.
In an educational and defensive tutorial, we avoid this.

Safer strategy:
1) Identify the default gateway and nearby hosts
2) Select a very small number of likely candidates
3) Validate services manually

Pseudocode (conceptual, not copy-paste scanning):
- Determine gateway / local network info
- Choose 1–3 candidate hosts
- Manually test a service with a strict timeout

