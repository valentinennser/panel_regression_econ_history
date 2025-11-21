# Panel Regression Implementation for Presentation in Economic History

Religion and Economic Development in Germany (2012–2023)
This project investigates whether religious composition—specifically the shares of Catholic and Protestant populations—predicts economic performance across German states. Inspired by the economic history literature (Weber; Becker & Wößmann), the analysis connects historical theories to modern panel data.

## Data

The dataset combines:
Religious population shares (Protestant, Catholic, Other)
GDP per capita for all 16 German States in the Years 2012–2023
Sources: State statistical offices and the Regionaldatenbank.
All datasets are merged into a balanced state–year panel.

## Methods

The analysis uses:
Fixed-effects panel regression (within estimator) to identify how within-state changes in religion predict GDP over time
Random-effects dynamic panel model (lagged GDP) to capture persistence and between-state differences
Lagged religion variables to mitigate simultaneity
Log-linear specification for GDP

## Key Findings
Catholic share shows a stronger positive short-run correlation with next-year GDP than Protestant share. When controlling for GDP persistence, both religion effects become very small. Results suggest modest short-run correlations but strong long-run path dependence in GDP.

## Reproducibility

All analysis is performed in R using dplyr, tidyr, and plm. Run models/main_analysis.R to reproduce all results.
