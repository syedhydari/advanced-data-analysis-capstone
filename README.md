# Stabilizing Kelly | R&FM Capstone

**Spring 2026 — STAT GR 5291 Capstone: R&FM Track / Advanced Data Analysis:** Columbia graduate capstone on stabilizing Kelly portfolio optimization under estimation risk using shrinkage, regime conditioning, and Sharpe-ratio detection-boundary analysis.

## Project Context

- **Date:** Spring 2026
- **Course:** STAT GR 5291 — Capstone: R&FM Track
- **Institution:** Columbia University
- **Project Type:** Graduate capstone / advanced data analysis project
- **Authors:** Syed Bashir Hydari and Mykola Kishmar
- **Research Area:** Kelly Criterion, portfolio optimization, estimation risk, regime conditioning, and Sharpe-ratio inference

## Overview

This project investigates why plug-in Kelly portfolio optimization fails out-of-sample on equity panels and which regularization layer best stabilizes performance.

The central finding is that the binding constraint is **mean-estimation noise**, not covariance ill-conditioning. Static shrinkage helps modestly, while regime-conditional moment estimation drives the largest improvement.

## Methods

- Long-only Kelly portfolio optimization
- Mean and covariance shrinkage
- Ledoit-Wolf covariance estimation
- Non-parametric macro regime classification
- RegimeFilter and RegimeDial variants
- Delta-method Sharpe-ratio inference
- Analytical power calibration
- Jump-diffusion Monte Carlo stress testing

## Key Result

The strongest strategy is the fully stacked **Combined** variant, which applies shrinkage to regime-filtered data. It achieves a net Sharpe of 0.66, compared with 0.46 for long-only minimum variance and 0.09 for naive plug-in Kelly.

## Reproducibility Note

This repository contains the final written report and selected academic materials. The original QMD/RMD analysis file is available upon reasonable request; a cleaned public reproduction file may be added later. Note, it is not investment advice and does not contain production trading infrastructure.
