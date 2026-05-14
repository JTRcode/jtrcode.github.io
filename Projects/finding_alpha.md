---
layout: post
title: Finding Alpha
category: project
description: Research-first equity screening and alpha-validation platform for testing interpretable technical setups.
image: /assets/images/coding_room.jpg
date: 2026
skills:
    - Python
    - pandas
    - Streamlit
    - Parquet
    - DuckDB
    - Plotly
nav-menu: false
---

<ul class="actions">
  <li><a href="https://findingalpha.streamlit.app/" class="button special" target="_blank" rel="noopener">Open Demo Dashboard</a></li>
  <li><a href="https://github.com/JTRcode/findingalpha" class="button" target="_blank" rel="noopener">View Repository</a></li>
</ul>

Finding Alpha is a research-first equity screening and alpha-validation platform for testing whether interpretable technical setups have predictive value across future return horizons. It is intentionally framed as research infrastructure, not a trading bot: the system does not place orders, does not connect to broker execution, and does not treat a high score as a validated trading signal.

The project turns discretionary setup ideas into versioned, testable hypotheses. A scan ingests historical market data, computes technical and liquidity features, saves timestamped signal snapshots, and evaluates whether ranked candidates later outperformed across 1D, 5D, 10D, 20D, and 60D horizons. The active research workflow focuses on Setup B, a trend-pullback continuation pattern.

## What I Built

The core system is a Python package with separated layers for data providers, storage, feature generation, signal scoring, research diagnostics, and dashboard presentation. Market data providers are isolated behind interfaces, raw and processed outputs are stored separately as Parquet artifacts, and every screener run can preserve the signal state that existed at research time.

Setup B is implemented as a frozen v1 baseline rather than a constantly moving rule set. The scanner uses a broad candidate gate for research sample size, strict audit gates for chart-quality review, and continuous quality scores for bucket testing. Proposed v2 changes are documented before implementation so new indicators or thresholds do not silently rewrite historical meaning.

## Research Methodology

The project evaluates signals with forward-return buckets, top-minus-bottom spreads, benchmark-relative returns against SPY and QQQ, date-declustered diagnostics, slice and interaction analysis, outlier checks, and yearly consistency reports. It also records negative findings, such as cases where stricter confirmation or volume dry-up did not clearly improve results.

This matters because a screen can look convincing after the fact without being a useful signal. Finding Alpha is built around the question: did the information available at the time predict future returns, or did it only look good after the outcome was known?

## Dashboard

The Streamlit dashboard is designed for research review rather than execution. It includes the latest daily screener snapshot, Setup B candidate tables, candlestick and volume chart review, broad vs strict gate audits, diagnostic indicator panels, filter funnels, score buckets, benchmark-relative diagnostics, outlier checks, and prototype intraday views.

For public review, the hosted demo uses a small sanitized dataset with public ticker symbols and prebuilt research artifacts. It is suitable for evaluating the workflow and interface, not for making trading or performance claims.

## Engineering Signals

- Modular provider and storage architecture for reproducible research runs.
- Timestamped signal snapshots for later validation against future outcomes.
- Versioned setup definitions and ADR-backed methodology decisions.
- Explicit separation between screens, signals, research diagnostics, strategy, and execution.
- Research reports documenting baseline evidence, transition criteria, and rejected hypotheses.
- Risk and compliance notes covering survivorship bias, lookahead risk, market-data licensing, and the exclusion of automated trading.
- Test coverage for providers, feature generation, scoring, forward returns, Setup B diagnostics, universe loading, and validation.

## Safe Interpretation

Finding Alpha does not claim to have discovered a profitable trading strategy. The defensible claim is narrower and more professional: it is a reproducible research platform for testing technical signal hypotheses with clear methodology, audit trails, dashboard review, and risk boundaries.
