# zeru_project_repo
# Aave V2 Wallet Credit Scoring

This project assigns a credit score (0–1000) to wallets based on DeFi behavior using Aave V2 data.

## Scoring Philosophy

Wallets are evaluated based on responsible behavior such as:
- High deposit and repayment volumes
- High repay-to-borrow ratio
- Consistent activity over time
- Low liquidation and sudden withdrawals

## Features Used
- `deposit`, `repay`, `borrow`, `redeemunderlying` totals
- `repay_to_borrow_ratio`
- `deposit_to_withdraw_ratio`
- `num_transactions`
- `active_days`

## Score Formula

A weighted sum of normalized features:
score = 0.3deposit + 0.2repay + 0.15*repay_to_borrow_ratio + ...
## ✅ Final Deliverables

1. ✅ Python script `score_wallets.py` that:
   - Accepts JSON
   - Cleans + engineers features
   - Outputs `wallet_credit_scores.csv`

2. ✅ `README.md` explaining methodology

3. ✅ Jupyter notebook for exploratory analysis


