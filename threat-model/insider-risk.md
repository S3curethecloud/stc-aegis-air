# Airline Threat Model — Insider Risk (Agents/Partners)

Insider risk is high-impact and under-modeled because it is politically sensitive and operationally complex.

## Primary insider scenarios
- Unauthorized PNR access and passenger data harvesting
- Agent credential misuse (shared credentials, delegation abuse)
- Loyalty balance manipulation (manual adjustments)
- Refund override abuse
- Excessive privilege and weak auditability

## What legacy tooling misses
- Treating agents as "trusted" identities instead of identities with **risk posture**.

## Required controls
- Strong identity (SSO/MFA) + least privilege + just-in-time elevation
- Immutable audit logs + anomaly detection on access patterns
- Separation of duties for high-risk actions
