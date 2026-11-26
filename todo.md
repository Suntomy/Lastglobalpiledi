# Global Pilgrim — Autonomous Robot + Payout Rails

## A. Backup & Baseline
- [x] Timestamped backup taken (backups/pre_auto_20261126T054815Z)
- [x] Read current core.js / engines.js / ui.js / app.html structure

## B. Autonomous Human-Sense Robot
- [x] Add `S.robot.auto` / `autoInvest` / `autoSweep` flags + migration
- [x] Robot auto-starts trading whenever trading balance > 0
- [x] Realised profit swept to Profit Balance then instantly to Main
- [x] Auto-reinvest idle Main Balance into trading
- [x] Robot Control toggles + live supervisor status text

## C. Payout Aggregator Rails
- [x] Payout Rails view with 7 rails (bank, SWIFT/SEPA/ACH, crypto, PayPal, gift card, bills, SIM)
- [x] Dynamic bank catalogue by country + account-name verification
- [x] Receipt fields: account no, account name, receiver, amount, date/time, serial, transaction ID
- [x] Frontend labels rails as authorisation-only; no secrets, no direct provider calls

## D. Secure Backend Scaffold
- [x] server.js with Flutterwave, Wise, ethers, PayPal, Reloadly, VTpass
- [x] PostgreSQL schema with FOR UPDATE row locking + idempotency + reversal
- [x] .env.example, package.json, migrate.js, README with security warnings
- [x] public/index.html portal calling backend only
- [x] Provider endpoints cross-checked against current docs

## E. Verify, Build, Deploy
- [x] node --check all sources
- [x] Browser test: 11 views, zero JS errors, admin + client login
- [x] Capital conservation, profit routing, auto-start, auto-sweep, seal
- [x] Rebuild index.html, backup, redeploy (179,168 bytes, live verified)
