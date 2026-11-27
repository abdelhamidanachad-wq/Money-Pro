# Money Pro

Personal finance tracker for MAD (Moroccan dirham).

## Current implementation
- Browser-local transaction ledger for manually entered transactions.
- Summary of recorded income, expenses, and net cash flow.
- Separate view for the imported archived transaction history.
- Exportable JSON backup.
- Budget reference for 28 November–28 December 2026.

## Historical data
`budget-history.js` is derived from the uploaded `budget-history(1).js` source. It is kept as a distinct archive and is not mixed into the live ledger, to avoid double counting or pretending archived estimates are verified current balances.

## Run
Open `index.html` in a modern browser, or deploy the repository as a static site on Vercel with the project root and no build command.

## Data storage
New transactions are stored in browser localStorage on that browser/device. This version does not yet provide cross-device sync or server-side persistence. Export backups regularly before clearing browser data.

## Note
This repository contains the working static implementation and source archive, not a financial ledger backed by a database. Reconcile historical entries against actual records before treating totals as audited balances.
