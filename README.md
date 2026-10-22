# Pg_Recon: Payment Gateway Reconciliation & Financial Analysis

An end-to-end financial data pipeline and reconciliation framework designed to match payment gateway transactions against bank statements, reconcile order logs, audit MDR rate cards, and generate executive-ready dashboards.

## Project Overview

Payment gateway reconciliation is critical for identifying revenue leakage, tracking settlement discrepancies, and ensuring financial accuracy. This repository contains a structured financial model and data pipeline built to process raw transaction data, apply business logic, map bridges, and summarize key financial insights for stakeholders.

## Repository Structure

```text
├── Assumptions_Note.pdf          # Key financial, accounting, and matching assumptions
├── CFO_Summary.pdf               # Executive summary and financial health overview
├── Formulas.xlsx                 # Documentation of core calculation logic and formulas
├── bank_statement_cleaned.xlsx   # Standardized and cleaned bank settlement records
├── bridge.xlsx                   # Reconciliation bridge matching payouts to transactions
├── dashboard.xlsx                # Visualizations and high-level performance metrics
├── data_quality_log.xlsx         # Audit trail tracking data cleansing and anomaly logs
├── mdr_rate_card_cleaned.xlsx    # Standardized Merchant Discount Rate (MDR) rate card
├── orders_cleaned.xlsx           # Cleaned internal order management system (OMS) logs
└── pg_transaction_cleaned.xlsx   # Cleaned raw payment gateway transaction logs

Core Components
Data Ingestion & Cleaning: Standardized raw logs from orders (orders_cleaned.xlsx), payment gateways (pg_transaction_cleaned.xlsx), and bank statements (bank_statement_cleaned.xlsx).

MDR & Fee Auditing: Validates gateway deductions using the normalized mdr_rate_card_cleaned.xlsx.

Reconciliation Bridge: bridge.xlsx maps discrepancies between expected revenue, gateway settlements, and bank deposits.

Reporting: Combines structured metric logs (data_quality_log.xlsx), visual dashboards (dashboard.xlsx), and executive takeaways (CFO_Summary.pdf).

Usage
Review Assumptions_Note.pdf for scope, matching criteria, and definitions.

Inspect Formulas.xlsx to understand the underlying calculation logic.

Open dashboard.xlsx for interactive performance metrics and reconciliation output.