# Airline Threat Model — Fraud (External)

Fraud in airlines is dominated by **account takeover** and **stored value theft** (loyalty points/miles) plus **refund/chargeback manipulation**.

## Primary fraud scenarios
- Loyalty account takeover (ATO) → points theft and redemption
- Miles laundering (conversion to third-party value)
- High-value redemption abuse (premium cabins, last-minute value)
- Refund exploitation (policy gaming, chargeback loops)
- Synthetic identity accounts used for promotion farming

## What legacy tooling misses
- Correlation between **identity risk** (new device, MFA state), **behavior** (velocity/bot), and **value timing** (high-value redemption right after login changes).

## Required controls
- Step-up auth (WebAuthn/MFA) on high-risk loyalty actions
- Velocity limits on login, redemption, refund flows
- Cool-down periods after credential changes
