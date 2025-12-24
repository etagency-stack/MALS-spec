# MALS-spec
Minimum Astronomical Legend Standard (MALS): Legends are data. No legend = incomplete scientific output.
# MALS — Minimum Astronomical Legend Standard

Scientific images without legends are incomplete data.

MALS defines the minimum required metadata and color-map semantics
for astronomical images intended for:
- scientific interpretation
- public release
- AI / ML training
- downstream analysis

## Core Claim
If an image encodes:
- wavelength
- intensity
- depth
- probability
- uncertainty

and lacks a machine- and human-readable legend,
it is **not complete scientific data**.

## v0.1 Scope
This repository defines:
- a minimal legend schema (JSON)
- before/after examples using JWST-style imagery
- guidance for agencies, journals, and toolchains

This is not a suggestion layer.
This is a **data completeness standard**.

## Status
- v0.1: Draft (RFC open)
- Community feedback welcome
- Validation pilots underway (xAI, JWST samples)

## Why Now
AI systems are already interpreting astronomical images.
Without legends, errors propagate silently.

Legends are not decoration.
Legends are data.

## Call to Action
If you produce astronomical imagery:
- include legends
- publish mappings
- expose uncertainty

Standards emerge when evidence meets pressure.
