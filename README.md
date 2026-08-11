<p align="center">
  <h1 align="center">Predicting Answer Features Before the Model Speaks</h1>
  <p align="center"><strong>Train maps from context activations to upcoming answer-feature probes.</strong></p>
</p>

---

## Overview

This repository implements experimental profiles for **Predicting Answer Features Before the Model Speaks**. Config, caching, hooks, metrics, ablations, reporting, and CI are built for reproducible local pilots on small open-weight models.

Hypothesis (one line): Train maps from context activations to upcoming answer-feature probes.

## Motivation

Interpretability and safety claims fail in practice for boring engineering
reasons: unpinned weights, chat templates skipped, invalid layer indices,
intervals that span zero treated as nulls, and stages that raise
`NotImplementedError`. This repo treats those as first-class bugs.

## Status

Focus: train maps from context activations to upcoming answer-feature probes. Shared infrastructure is in place; domain stages
must pass harness validation before any measured claim.

| Command | Purpose |
|---|---|
| `make install-dev` | editable install + pinned requirements |
| `make test` | full unit suite |
| `make ci` | lint + test + typecheck + api-contract + coverage |
| `make pilot` | end-to-end pilot profile |
| `make doctor` | environment / device report |
