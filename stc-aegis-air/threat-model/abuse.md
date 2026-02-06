# Airline Threat Model — Abuse (Gray-Zone)

Abuse is repeatable exploitation that often stays below fraud thresholds until patterns are aggregated.

## Primary abuse scenarios
- Bot-driven seat holds / inventory locking
- Promotion exploitation (multi-account cycling)
- Refund abuse just below manual-review thresholds
- Partner API scraping (fare data, availability)
- Account sharing for loyalty benefits

## What legacy tooling misses
- Abuse requires **time-window aggregation** and **entity graphing** (device ↔ account ↔ payment instrument ↔ IP ↔ booking patterns).

## Required controls
- Bot controls (challenge/MFA, device reputation)
- Rate limits per identity/device/network
- Pattern-based throttling for repeated low-grade abuse
