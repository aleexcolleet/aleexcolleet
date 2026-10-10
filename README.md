# Alex Collet Martínez

Economics at Universitat Autònoma de Barcelona · systems programming background
from 42 Barcelona.

I build tools that measure risk, and I check them against numbers somebody else
published.

[LinkedIn](https://www.linkedin.com/in/alexcollet) · alexcollet.dev@outlook.com · [Black Orbit](https://blackorbit.dev)

---

## Projects

### [fixed-income-risk](https://github.com/aleexcolleet/fixed-income-risk) · Python

Bond valuation and interest rate risk, written from first principles with no
dependencies beyond pytest. Day count conventions, accrued interest, clean and
dirty price, yield by Newton-Raphson, zero curve and spread discounting, and
duration, convexity and DV01 computed two ways — analytically and by bumping —
with an assertion that the two agree.

It reproduces the yields the Spanish Treasury published in the BOE for its
September 2026 auction to within **0.1 basis points**, the precision they are
printed at. Reaching that meant separating three different things: a
compounding convention hidden in the ECB data, a market time measure that is
not a day count, and a real defect in my own cashflow generator that 87
property-based tests had missed. The write-up is in `docs/`.

### [MarketMakerLimitBookSim](https://github.com/aleexcolleet/MarketMakerLimitBookSim) · C++17

Limit order book and market-making simulator. It splits P&L into spread capture
and adverse selection against a latent value the maker cannot see, so the loss
to informed flow is measured rather than asserted. Freeze the latent value and
the maker is profitable again — that control is what makes the rest believable.

5,369 assertions, continuous integration on three compilers, clean under
AddressSanitizer and UBSan, and 33 design decisions documented with their costs,
including the ones I reversed.

---

## Currently

Continuing the fixed income engine: curve bootstrapping and forward rates, then
interest rate swaps, then bucketed DV01 for a portfolio.

Co-founder at Black Orbit, a Barcelona software studio, where I own backend
architecture through deployment.

Studying econometrics and time series at UAB, Hull on risk management, and bank
disclosure under Pillar 3.

---

## Tools

Python · C · C++ · Go · SQL · Bash · Linux · Docker · Git

---

Barcelona · open to internships in market risk, fixed income and asset management
