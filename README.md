# README

## Contact
Authors and affiliations:

Johannes Ruf j.ruf@lse.ac.uk, www.maths.lse.ac.uk/Personal/jruf, London School of Economics and Political Science.

Yueying Sun y.sun63@lse.ac.uk, London School of Economics and Political Science

April 2026

## Introduction
This repository contains empirical and simulation studies for the mandate models for inelastic market hypothesis.


## Data Sources

The analysis uses publicly available U.S. financial data:

- **Flow of Funds (FoF)**  
  Source: Financial Accounts of the United States (Z.1), published by the Board of Governors of the Federal Reserve System  
  Accessed on: 29 Apr 2026  
  Link: https://www.federalreserve.gov/datadownload/Choose.aspx?rel=z1  

- **Monthly Statement of the Public Debt (MSPD)**  
  Source: U.S. Treasury Monthly Statement of the Public Debt, published by Fiscal Data  
  Accessed on: 29 Apr 2026  
  Link: https://fiscaldata.treasury.gov/datasets/monthly-statement-public-debt/summary-of-treasury-securities-outstanding  

- **CRSP (Center for Research in Security Prices)**  
  Accessed on: 29 Apr 2026 via WRDS (Wharton Research Data Services)  
  



## Notebooks

### 1. `Simulation.ipynb`
- Simulates mandate-implied stock capitalisation under two specifications for the bond capitalisation process: a binomial model and a geometric Brownian motion.
- Examines how the mandates affect the response of stock capitalisation to changes in bond capitalisation  
- Reproduces the results of Section 2.2 of the thesis "Two Topics in Mathematical Finance: Mandate Models and Mean-Variance Hedging".

---

### 2. `DataComparison.ipynb`
- Processes data from FoF, MSPD, and CRSP  
- Compares different data sources for U.S. bond and equity capitalisation.
- Assesses consistency across datasets and verifies whether they exhibit similar dynamics over time.
- Reproduces the results of Section 2.3.1 of the thesis "Two Topics in Mathematical Finance: Mandate Models and Mean-Variance Hedging".

---

### 3. `EmpiricalAnalysis.ipynb`
- Constructs the bond and equity capitalisation series using Flow of Fund data.
- Estimates two parametrised mandate models: the power mandate and the constant mandate.
- Evaluates performance via backtesting 
- Reproduces the results of Section 2.3.2 of the thesis "Two Topics in Mathematical Finance: Mandate Models and Mean-Variance Hedging".

---

