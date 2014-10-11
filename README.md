# FinMarkets

FinMarkets.jl will help you describe and model financial market objects in
Julia.

For example:

```julia
# Load packages
using Dates, FinMarkets
# Create US Dollar object
USD = USD()
# Create 3m USD LIBOR
depo = Deposit(USD, Month(3), 0.05)
# Price depo at trade date
price(depo)
```
## Features

Objects such as:

- Compounding constants, interest rates, discount factors
- Financial market calendars, day counters and roll conventions
- Currencies
- Stub types
- Schedules
- Cash flows
- Interest rate indices
- Instruments

Modelling such as:

- Year fraction calculations
- Conversion between interest rates and discount factors and between different interest rates
- Identifying good (and bad) days
- Adjusting and shifting dates
- Creating swap date schedules
- Pricing instruments

## Installation

Install FinMarkets.jl by running:

```julia
Pkg.clone("https://github.com/imanuelcostigan/FinMarkets.jl")
```

## Obligatory badges

[![Build Status](https://travis-ci.org/imanuelcostigan/FinMarkets.jl.png)](https://travis-ci.org/imanuelcostigan/FinMarkets.jl)
[![Coverage Status](https://coveralls.io/repos/imanuelcostigan/FinMarkets.jl/badge.png?branch=release%2F0.1)](https://coveralls.io/r/imanuelcostigan/FinMarkets.jl?branch=release%2F0.1)
[![Documentation Status](https://readthedocs.org/projects/finmarketsjl/badge/?version=master)](https://readthedocs.org/projects/finmarketsjl/?badge=master)
