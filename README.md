# Stabilizing Kelly | R&FM Capstone

**Spring 2026 — STAT GR 5291 Capstone: R&FM Track / Advanced Data Analysis:** Columbia graduate capstone on stabilizing Kelly portfolio optimization under estimation risk through shrinkage, regime conditioning, and detection-boundary analysis.

## Project Context

- **Date:** Spring 2026
- **Course:** STAT GR 5291 — Capstone: R&FM Track
- **Institution:** Columbia University
- **Project Type:** Graduate capstone / advanced data analysis project
- **Authors:** Syed Bashir Hydari and Mykola Kishmar
- **Research Area:** Kelly Criterion, portfolio optimization, estimation risk, regime conditioning, shrinkage, and Sharpe-ratio inference

## Overview

This project studies why plug-in Kelly portfolio optimization fails out-of-sample on equity panels and tests which regularization layer best stabilizes performance.

The central finding is that **mean-estimation noise**, not covariance ill-conditioning, is the binding constraint. Static mean shrinkage helps modestly, while regime-conditional moment estimation drives the largest improvement.

## Methods

- Long-only Kelly portfolio optimization
- 2x2 shrinkage factorial: mean shrinkage and covariance shrinkage
- Ledoit-Wolf covariance shrinkage
- Mean shrinkage toward the risk-free target
- Non-parametric macro regime classification
- RegimeFilter: regime labels used for moment estimation
- RegimeDial: regime labels used for fractional Kelly sizing
- Delta-method Sharpe-ratio inference
- Analytical power calibration
- Merton jump-diffusion Monte Carlo stress testing

## Key Result

The strongest strategy is the fully stacked **Combined** variant, which applies mean shrinkage and covariance shrinkage to regime-filtered data. It achieves a net Sharpe of 0.66, compared with 0.46 for long-only minimum variance and 0.09 for naive plug-in Kelly.

The project also shows that regime information can be used in two distinct ways: **RegimeFilter** maximizes Sharpe, while **RegimeDial** improves drawdown control through state-dependent fractional Kelly exposure.

## Note

This repository contains selected academic materials from a Columbia R&FM capstone project. It is not investment advice and does not contain production trading infrastructure.
