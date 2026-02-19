# STC Ecosystem Wiring — Aegis-Air

Aegis-Air is the authoritative definition layer for Airline Identity Risk.

Flow of truth:

1. Aegis-Air
   - Defines airline entities, signals, and risk scenarios
2. RiskDNA
   - Scores Aegis-Air signals deterministically
3. STC Shield
   - Visualizes RiskDNA outputs and blast radius
4. STC Intelligence Core
   - Provides deterministic explanations
5. Copilot / Voice
   - Translate explanations for humans
6. STC Academy
   - Teaches the exact labs that mitigate the risk

Canonical demo cases in `demo/` are the single source of truth
for all ecosystem demonstrations.
