# STC-Aegis-Air

**One sentence:** Airline risk intelligence that detects, scores, and explains fraud, abuse, and insider threats across the full passenger and operational lifecycle, using **RiskDNA** and governed by **STC AI**.

## What this repo is
STC-Aegis-Air is the **airline-specific adapter** for the SecureTheCloud risk stack.

- **RiskDNA (upstream):** canonical risk scoring + explainability.
- **Aegis-Air (this repo):** airline domain model (threats, signals, narratives).
- **STC Shield (downstream):** executive UI and storyboards.

## Core principle
Airline fraud prevention is not one model and not one event. It is lifecycle correlation:

**Booking → Loyalty → Check-in → Airport Ops → Refunds → Partners**

## Repo layout
- `mgf/` — governance + STC AI integration contract
- `threat-model/` — fraud, abuse, insider risk
- `signals/` — canonical airline signal taxonomy
- `adapters/` — wiring to RiskDNA + Shield
- `docs/` — executive and technical docs

## Status
MGF governed. Deterministic by default. Explainability required.
