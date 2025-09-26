**Fannie Mae 2025-21 REMIC Trust – Cashflow Model**

This project implements a Python-based cashflow model for the Fannie Mae 2025-21 REMIC Trust, a multi-class REMIC backed by two groups of UMBS collateral. The model translates the deal’s prospectus supplement into code and simulates collateral/prepayments, interest and principal waterfalls, and class-level cashflows.

* Features

Deal Structure

Sequential, accrual, floating, and inverse floating rate tranches

Notional IO classes linked to floating classes (SB, SC)

Collateral Simulation

Group 1 and Group 2 UMBS pools

Prepayment assumptions at 0 PSA and 400 PSA

Cashflow Waterfall

Principal allocation rules by group (sequential and pro-rata splits)

Accrual tranches (BZ, CZ) with interest capitalized into balance

Floating and inverse floating tranches indexed to SOFR with caps/floors

Outputs

Monthly collateral cashflows

Tranche-level principal & interest payments

Ending balances

Weighted Average Life (WAL) for each tranche

Deliverables

Colab/Jupyter notebook (documented)

Excel file with cashflows and WALs

* Tech Stack

Python 3

pandas, numpy, openpyxl

Google Colab / Jupyter Notebook

* Files in Repository

FNM2025_21_REMIC.ipynb → Main notebook with code & walkthrough

FNM2025_21_outputs.xlsx → Excel outputs (cashflows & WALs for 0 PSA and 400 PSA)

README.md → Project documentation (this file)

* How to Run

Clone this repo:

git clone https://github.com/your-username/FNM2025-21-REMIC-Model.git
cd FNM2025-21-REMIC-Model


Open the notebook in Google Colab or Jupyter.

Install dependencies if needed:

pip install pandas numpy openpyxl


Run all cells.

The Excel output (FNM2025_21_outputs.xlsx) will be generated with:

Collateral cashflows

Tranche cashflows (interest & principal)

WAL calculations

* Example Outputs

Cashflow Projections: Monthly principal & interest per tranche

WALs: Tranche-level Weighted Average Life under both PSA 0 and PSA 400
 
* Learning Outcome

This project demonstrates how to:

Convert prospectus supplement rules into executable code

Model structured finance waterfalls in Python

Apply prepayment models (PSA)

Implement SOFR-based floating & inverse floating coupons

Deliver professional Excel outputs for structured finance analysis
