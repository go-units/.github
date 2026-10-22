<p align="center"><img src="https://raw.githubusercontent.com/go-units/brand/main/social/go-units.png" alt="go-units" width="720"></p>

# go-units

🌐 **[Website](https://go-units.github.io)** · 📚 **[Documentation](https://go-units.github.io/docs/)**

**Units and physical constants in pure Go (CGO=0). Planned, wave 2: no library exists yet.**

go-units is the organisation the [go-scikit parity plan](https://github.com/go-scikit/roadmap/blob/main/PLAN.md)
names for what MATLAB's `symunit` and `physconst` and Mathematica's `Quantity`
offer. Nothing is released and no code is written: this page, the website and
the documentation say what the organisation will cover and how each part will be
checked. The state of every item is in
[STATUS.md](https://github.com/go-scikit/roadmap/blob/main/STATUS.md).

## What it will cover

| Planned package | What it will provide | Validated against |
|-----------------|----------------------|-------------------|
| `units` | a dimension vector of rational exponents, quantities, conversion, a parser for the UDUNITS grammar, the SI, US customary and derived units, offset units (degC, degF), dimensional analysis; later (wave 4) user-defined unit systems such as EMU, ESU and atomic | exact dimension vectors; pint and astropy; NIST SP 811 |
| `constants` | the CODATA 2022 recommended values, generated from NIST's ASCII table by a reproducible tool that records the edition | a table diff against `allascii.txt`; `scipy.constants` |

The package names are provisional. The plan places go-units in wave 2 (item 9,
size S) and user-defined unit systems in wave 4 (item 21). The references are the
BIPM SI Brochure, CODATA 2022, UDUNITS-2 and UCUM; no existing Go unit package
is a dimensional-analysis engine, so none is a dependency. Dates and time scales
stay with go-datetime.

## Repositories

| Repo | What it is |
|------|------------|
| [**docs**](https://github.com/go-units/docs) | the documentation site (Hugo + Hextra), served at [/docs/](https://go-units.github.io/docs/) |
| [**go-units.github.io**](https://github.com/go-units/go-units.github.io) | the landing page (Hugo) |
| [**brand**](https://github.com/go-units/brand) | logo, icons and social images |

No library repository exists yet: each is created when its first pull request is ready.
