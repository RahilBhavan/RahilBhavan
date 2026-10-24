# Rahil Bhavan

I am a junior at the University of Michigan (B.S.E. Computer Engineering and B.S. Economics, expected May 2029). I build data pipelines, risk models and evaluated tools for on-chain markets and SEC filings, plus some processor and firmware work. Write-ups are at [rahilbhavan.com](https://rahilbhavan.com).

## Featured projects

### On-chain risk and DeFi

- [**Spine**](https://github.com/RahilBhavan/spine): live risk dashboard and liquidation backtest for Coinbase's on-chain loan book (Morpho Blue on Base). It tracks $1.63B of borrowing across nine markets (2026-09-23 snapshot), and the calibrated model matched realized cbBTC liquidation volume at 0.85x to 0.99x in three stress events. [Live](https://spine.rahilbhavan.com)
- [**Guardian pipeline**](https://github.com/RahilBhavan/guardian-pipeline): the same 12 invariants for a Solidity lending vault, checked by Foundry fuzzing in CI (99 tests, 2,000-run invariant campaign) and by a TypeScript runtime monitor. The solvency invariant caught a one-wei repayment bug. It is a testnet demo, not production. [Live](https://guardian.rahilbhavan.com)
- [**MEV sandwich study**](https://github.com/RahilBhavan/mev-sandwich-batch-study): sandwich losses on the Uniswap v3 WETH/USDT 0.01% pool over 5 to 11 Oct 2026. 236 sandwiches cost 244 victims $12,387. Under Chan, Wu and Shi's per-block two-phase clearing, no sandwich made money in replay.

### Filings and financial analysis

- [**dat-accretion**](https://github.com/RahilBhavan/dat-accretion): per-share effect of Strategy, BitMine and SharpLink capital actions on net coins per share, and the break-even price of each preferred rotation. It covers 98 filing-linked actions from June to October 2026 and has 170 tests. [Live](https://rahilbhavan.github.io/dat-accretion/)
- [**Strategy preferred coverage model**](https://github.com/RahilBhavan/strategy-preferred-coverage-model): Excel model of Strategy's preferred dividend coverage, common issuance capacity and convertible puts. At 15 Oct 2026 prices, Strategy's $4,880M reserve covers 37.5 months of cash charges before principal. [Live](https://rahilbhavan.github.io/strategy-preferred-coverage-model/)
- [**Filing research assistant**](https://github.com/RahilBhavan/filing-research-assistant): answers questions about SEC 10-K and 10-Q filings with cited source passages, or abstains. On a held-out set, checked Claude Haiku answers were correct on 26/30 questions and abstained on 10/10 unanswerable ones. The build agent wrote the labels, and no human has reviewed them.
- [**Financial metrics analyst**](https://github.com/RahilBhavan/financial-metrics-analyst): MCP server that answers financial-metric questions from SEC filings with exact-decimal arithmetic and provenance on every answer. 161/161 evaluation cases pass. A Claude agent over it chose the correct tool and arguments on 42/42 in-scope tasks in one run.

### Systems and hardware

- [**RV32I core with DOT4**](https://github.com/RahilBhavan/riscv): educational five-stage RV32I core in SystemVerilog with a custom int8 dot-product instruction. 252 programs pass in Icarus and Verilator, it matches Spike on 39/39 architecture tests, and the checkers catch 23/23 injected RTL bugs.

## More projects

On-chain risk and DeFi

- [Spine Midnight](https://github.com/RahilBhavan/spine-midnight): outcomes of Morpho Midnight fixed-maturity loans on Base. Of 148 positions due on 25 Sep 2026, 124 were repaid.
- [Yield/Fidelity](https://github.com/RahilBhavan/beefy-yield-fidelity-monitor): compares reported Beefy vault yield on Base with realized on-chain growth and the cost break-even. [Live](https://yield.rahilbhavan.com)
- [Ondo flows](https://github.com/RahilBhavan/Ondo): weekly OUSG and USDY instant mint and redeem volume, net flow and unique wallets from public on-chain data. [Live](https://ondo-nexus.vercel.app/flows)
- [x402 exception desk](https://github.com/RahilBhavan/x402-exception-desk): synthetic x402 payment exception desk on Base, with queue-policy experiments over 3,600 scenarios. [Report](https://rahilbhavan.github.io/x402-exception-desk/)
- [Limit canvas](https://github.com/RahilBhavan/limit-canvas): visual builder and verifier for 1inch Limit Order Protocol v4.3.2 extensions.
- [ShadowSolve](https://github.com/RahilBhavan/shadowsolve): advisory-only shadow solver for constant-product auctions in Rust, with Postgres provenance and fail-closed ingestion. It never submits transactions.

Filings and financial analysis

- [COIN revenue bridge](https://github.com/RahilBhavan/coin-revenue-bridge): splits Coinbase's $863.8M Q3 to Q4 2024 consumer revenue rise into volume and yield effects from SEC filings. [Live](https://revenue.rahilbhavan.com)
- [MARA credit case](https://github.com/RahilBhavan/mara-credit-case): credit committee case on a hypothetical $5M secured revolver to MARA Holdings. [Live](https://mara.rahilbhavan.com)
- [Filing tracker](https://github.com/RahilBhavan/filing-tracker): what changed between two 10-K filings, as aligned diffs of Risk Factors and MD&A with citations.
- [AuctionFlow](https://github.com/RahilBhavan/auctionflow): offline, deterministic replay of CME Micro E-mini (MES) sessions with a fail-closed risk journal. It is research only and never places orders.

Strategy capital structure: small offline tools built from Strategy's SEC filings

- [8-K ledger](https://github.com/RahilBhavan/strategy-8k-ledger): source-traceable treasury ledger with frozen SEC evidence and reconciliation checks.
- [Preferred accrual ledger](https://github.com/RahilBhavan/preferred-accrual-ledger): replays five sourced preferred dividend schedules and reports reconciliation gaps.
- [Credit curve](https://github.com/RahilBhavan/strategy-credit-curve): sourced comparisons of Strategy's preferreds and convertible scenarios.
- [STRC rate controller](https://github.com/RahilBhavan/strc-rate-controller): replays STRC's discretionary rate resets.
- [Coverage Monte Carlo](https://github.com/RahilBhavan/strategy-coverage-montecarlo): conditional funding exhaustion across reserve, common ATM and BTC-sale scenarios.
- [Fair-value earnings](https://github.com/RahilBhavan/strategy-fair-value-earnings): reproduces BTC fair-value earnings and simplified CAMT scenarios.
- [Issuance router](https://github.com/RahilBhavan/strategy-issuance-router): dated financing rules compared with SEC-disclosed weekly issuance.
- [Ask filings](https://github.com/RahilBhavan/strategy-ask-filings): answers set questions from dated filing evidence, with explicit refusals.
- [Proof of reserves](https://github.com/RahilBhavan/treasury-proof-of-reserves): regtest demo with BIP-322 asset signatures and Merkle-sum liability proofs. [Live](https://rahilbhavan.github.io/treasury-proof-of-reserves/)
- [did:btc resolver](https://github.com/RahilBhavan/did-btc-resolver): independent resolver for the did:btc draft, checked through a Bitcoin Core regtest lifecycle.
- [Mismatch investigator](https://github.com/RahilBhavan/strategy-mismatch-investigator): explains a gap between two report totals by rerunning one report with the other's filter. Synthetic records and a simulated adapter; not affiliated with Strategy.

Systems and hardware

- [Cortex-M deterministic replay](https://github.com/RahilBhavan/cortex-m-deterministic-replay): record and replay for Cortex-M firmware, run in host emulation, with an FPGA capture gateway checked in Verilator.

## Contact

- Website: [rahilbhavan.com](https://rahilbhavan.com)
- LinkedIn: [linkedin.com/in/rahil-bhavan](https://www.linkedin.com/in/rahil-bhavan/)
- Email: [rbhavan@umich.edu](mailto:rbhavan@umich.edu)

Open to internships in software engineering, product and crypto finance. I am a U.S. citizen and need no visa sponsorship.
