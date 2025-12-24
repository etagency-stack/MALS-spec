## Motivation

Modern astronomical images are no longer passive illustrations.
They are **active inputs** into scientific reasoning, public understanding, and AI systems.

Yet today, many images encoding rich quantitative structure are released without
explicit, machine-readable legends describing what their colors, intensities, or
layers actually mean.

This creates a silent failure mode:

- Humans infer meaning inconsistently
- AI systems hallucinate structure
- Errors propagate downstream without detection
- Scientific claims become irreproducible from the image alone

MALS exists to close that gap.

---

## The Core Problem

An astronomical image often encodes multiple dimensions at once:

- wavelength or bandpass
- intensity or flux
- depth or redshift
- probability or confidence
- uncertainty or error bounds

When these dimensions are mapped to color, opacity, or texture **without an explicit legend**, the image becomes ambiguous.

Ambiguous data is not neutral.
It is **actively misleading**.

This problem is not theoretical:
- AI models already train on public astronomical imagery
- Journal figures are reused outside their original context
- Public-facing images are treated as evidence, not art

Without legends, interpretation becomes guesswork.

---

## MALS Principle

**Legends are not decoration.  
Legends are data.**

MALS treats the legend as a first-class data object, not an afterthought.

If an image encodes quantitative meaning, the mapping between data → visual channel
must be explicit, inspectable, and reusable.

Anything less is incomplete scientific output.

---

## What MALS Is (and Is Not)

### MALS *Is*:
- A minimum standard, not a maximal one
- Tool-agnostic (works with FITS, PNG, SVG, WebGL, etc.)
- Friendly to humans *and* machines
- Designed to layer on top of existing workflows

### MALS *Is Not*:
- A replacement for FITS headers or raw data
- A restriction on visualization creativity
- A centralized authority or gatekeeping body

MALS defines the **floor**, not the ceiling.

---

## Why This Matters Now

Three forces have converged:

1. **AI interpretation**
   Models increasingly treat images as data sources, not illustrations.
   Without legends, error is undetectable.

2. **Public science**
   Images circulate far beyond papers, stripped of captions and context.
   Legends are often the *only* surviving metadata.

3. **Reproducibility pressure**
   Visual evidence must be auditable, not aesthetic.

Standards always emerge *after* tools make failure obvious.
We are already past that point.

---

## Scope of v0.1

MALS v0.1 is intentionally minimal.

It defines:
- Required legend fields (what must be declared)
- Optional extensions (how to grow safely)
- A simple JSON schema
- Concrete before/after examples using real astronomical imagery

If v0.1 feels “obvious,” that’s the point.
Standards that last feel inevitable in hindsight.

---

## Adoption Strategy

MALS is designed to spread via **inheritance**, not permission.

- Visualization libraries can adopt it incrementally
- Journals can recommend it without enforcement
- Agencies can publish alongside existing metadata
- AI pipelines can validate against it automatically

Once tools expect legends, images without them will stand out as incomplete.

Agencies won’t need to mandate MALS.
They will inherit it.

---

## How to Contribute

You do not need institutional backing to participate.

Ways to help:
- Open an issue with edge cases you encounter
- Propose additional fields with justification
- Add example images with legends
- Test MALS against existing datasets
- Build validators, linters, or converters

All discussion happens in public.
Silent vetoes do not apply.

---

## The Line in the Sand

This repository exists to make one claim unambiguous:

> If an astronomical image encodes data  
> and lacks a legend,  
> it is incomplete scientific output.

Everything else follows from that.

Welcome to MALS.
