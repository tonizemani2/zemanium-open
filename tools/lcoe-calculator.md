Tool · [Toni Zemani](https://zemanium.com/about#toni-zemani) · 27 November 2026

# LCOE calculator: the levelized cost of energy of any power plant.

Enter what a plant costs to build and run, how much it produces and how long it lasts, and the calculator returns its levelized cost of energy (LCOE) in dollars per megawatt-hour. It uses the simple formula the US national laboratories publish, and starts on a new geothermal plant built to Lazard's 2026 assumptions: $91.11 per megawatt-hour.

Presets are midpoints of the low and high inputs in Lazard's Levelized Cost of Energy+ version 19.0 (July 2026). The calculator leaves out taxes, depreciation and cost escalation, so its results sit near Lazard's published ranges without matching them exactly.

01 / Calculator

## Calculate LCOE. Start from Geothermal, new plant (Lazard 2026 midpoint) Solar PV, utility scale (Lazard 2026 midpoint) Wind, onshore (Lazard 2026 midpoint) Gas combined cycle (Lazard 2026 midpoint) Nuclear (Lazard 2026 midpoint) Your own numbers Capital cost, $ per kW Fixed operating cost, $ per kW per year Variable operating cost, $ per MWh Fuel cost, $ per MWh Capacity factor, % Own use of output (pumps, auxiliaries), % Life, years Discount rate (cost of capital), % Plant size, MW Levelized cost of energy $91.11 per MWh

Capital share

$72.15

Fixed operating share

$2.03

Variable operating cost

$16.93

Fuel

$0.00

Capital recovery factor

0.0913

Net output per year

372,300 MWh

Capital cost of the plant

$294.3 million

Change any field and the result updates. Plant size changes the totals, not the cost per megawatt-hour.

The calculator needs JavaScript. The formula below gives the same result by hand.

For geothermal plants with a simulated reservoir behind them, our [power-cost model](https://zemanium.com/confidence/) runs 1,080 scenarios on GEOPHIRES-X output and shows how the price moves with well cost, plant cost and the cost of money.

02 / Meaning

## What is the levelized cost of energy (LCOE)?

The levelized cost of energy (LCOE), also called the levelized cost of electricity, is the constant price per megawatt-hour at which a power plant earns back everything spent on it over its life, including the return its lenders and owners expect. It puts plants with very different cost structures on one scale: a solar farm that is cheap to build and produces a quarter of the time, a geothermal plant that is expensive to drill and runs day and night, and a gas plant that is cheap to build and pays for fuel every hour.

03 / Formula

## The LCOE formula.

The full definition discounts every year's cost and every year's output back to today:

`LCOE = sum over years t of (capital + operating + fuel cost in year t) / (1 + r)^t, divided by sum over years t of (electricity in year t) / (1 + r)^t`

When the plant is built at once and costs and output are the same each year, that reduces to the simple form the National Laboratory of the Rockies (NLR, formerly NREL) publishes, which this calculator uses:

`LCOE = (capital cost per kW x CRF + fixed O&M per kW-year) x 1000 / (8760 x capacity factor) + variable O&M + fuel cost`

`CRF = r (1 + r)^n / ((1 + r)^n - 1)`

Here `r` is the discount rate, `n` the life in years and CRF the capital recovery factor, the share of the capital cost that has to be recovered each year. The factor 1000 turns kilowatts into megawatts and 8760 is the number of hours in a year.

04 / Worked example

## How to calculate LCOE, step by step.

A new geothermal plant on Lazard's 2026 midpoint inputs: $5,885 per kW to build, $15.125 per kW-year fixed and $16.925 per MWh variable operating cost, no fuel, an 85% capacity factor, a 25-year life and a 7.7% discount rate.

1. Capital recovery factor: 0.077 x 1.077^25 / (1.077^25 - 1) = 0.0913.
2. Yearly cost per kW: $5,885 x 0.09129 + $15.125 = $552.37.
3. Yearly output per kW: 8,760 hours x 85% = 7,446 kWh, or 7.446 MWh.
4. Fixed cost per MWh: $552.37 / 7.446 = $74.18.
5. Add variable cost and fuel: $74.18 + $16.925 + $0 = $91.11 per MWh.

The same plant costs $69.55 per MWh at a 4% discount rate and $106.03 at 10%. Almost all of a geothermal plant's cost is paid before it runs, so the cost of money moves its price more than any operating figure. Our [guide to geothermal electricity cost](https://zemanium.com/guides/geothermal-electricity-cost) shows what sets each input.

05 / Comparison

## LCOE by energy source in 2026.

| Technology | Unsubsidized LCOE, $/MWh | Average | Capital cost, $/kW | Capacity factor |
|---|---|---|---|---|
| Onshore wind | $37 to $99 | $68 | $1,900 to $2,750 | 30% to 55% |
| Solar PV, utility scale | $40 to $98 | $69 | $1,250 to $1,850 | 20% to 30% |
| Geothermal | $67 to $111 | $89 | $5,135 to $6,635 | 80% to 90% |
| Gas combined cycle | $51 to $129 | $90 | $1,450 to $2,100 | 30% to 90% |
| Coal | $72 to $177 | $125 | $3,495 to $7,405 | 65% to 85% |
| Offshore wind | $105 to $167 | $136 | $5,600 to $7,100 | 45% to 55% |
| Gas peaking | $144 to $276 | $210 | $1,100 to $1,650 | 10% to 15% |
| Nuclear | $175 to $255 | $215 | $12,300 to $17,570 | 89% to 94% |

Source: Lazard, Levelized Cost of Energy+ version 19.0, July 2026, new-build plants in the United States without tax credits.

06 / Limits

## What LCOE leaves out.

- When the power arrives. A megawatt-hour at 7 pm on a still winter evening is worth more to a grid than one at noon in spring. Lazard publishes a separate cost of firming intermittency for that reason.
- Grid costs. Transmission, interconnection and balancing sit outside the LCOE of a single plant.
- Output that changes with age. The simple formula assumes the same output every year. A geothermal reservoir can cool and a solar panel degrades; the full discounted formula takes a year-by-year output instead.
- Risk. Exploration wells that miss, construction overruns and fuel price swings shift the real cost. Our [power-cost model](https://zemanium.com/confidence/) draws 2,000 combinations of them.

07 / Questions

## Common questions.

### What does LCOE stand for?

Levelized cost of energy, or levelized cost of electricity. It is the price per megawatt-hour at which a power plant exactly pays back its lifetime costs, including the return on the money invested.

### How do you calculate LCOE?

Multiply the capital cost per kilowatt by the capital recovery factor, add the fixed operating cost per kilowatt-year, divide by the megawatt-hours each kilowatt produces in a year (8.76 times the capacity factor), then add variable operating and fuel cost per megawatt-hour.

### How do I calculate LCOE in Excel?

The capital recovery factor is =PMT(rate, years, -1), for example =PMT(0.077, 25, -1) returns 0.0913. Then LCOE = (capex_per_kW * CRF + fixed_OM) * 1000 / (8760 * capacity_factor) + variable_OM + fuel.

### What is a good LCOE?

It depends on what the plant delivers. In Lazard's 2026 figures new onshore wind and utility solar average $68 and $69 per megawatt-hour, geothermal $89 and gas combined cycle $90. Geothermal and gas run when needed; wind and solar need storage or backup for that.

### What is the LCOE of geothermal energy?

Lazard puts new geothermal at $67 to $111 per megawatt-hour in 2026, average $89. Public US geothermal power contracts signed from 2019 to mid-2025 priced at $67.50 to $99. The US Department of Energy targets $45 for enhanced geothermal by 2035.

### Is this LCOE calculator free?

Yes. It runs in your browser, needs no account and stores nothing. The text and tables on this page are CC BY 4.0, and the calculator code is MIT licensed.

08 / Sources

## Sources.

1. Lazard, [Levelized Cost of Energy+, version 19.0](https://www.lazard.com/research-insights/levelized-cost-of-energyplus-lcoeplus/), 13 July 2026 (ranges, capital costs, capacity factors, preset inputs).
2. National Laboratory of the Rockies, [Simple Levelized Cost of Energy (LCOE) Calculator Documentation](https://nlr.gov/analysis/tech-lcoe-documentation), read 27 November 2026 (formula).
3. National Laboratory of the Rockies, [Annual Technology Baseline 2025: geothermal](https://atb.nlr.gov/electricity/2025/2023/geothermal), read 27 November 2026 (power purchase agreements).
4. US Department of Energy, [Enhanced Geothermal Shot](https://www.energy.gov/articles/doe-launches-new-energy-earthshot-slash-cost-geothermal-power), 8 September 2022.

Text and tables on this page are licensed [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/); the calculator code is MIT. Cite as: Toni Zemani, "LCOE calculator", Zemanium, 27 November 2026. [All open models, records and drawings ](https://zemanium.com/open/)

---
Source: https://zemanium.com/lcoe-calculator
Publisher: Zemanium (https://zemanium.com/). Contact: toni@zemanium.com
Licence: text and figures CC BY 4.0 (https://creativecommons.org/licenses/by/4.0/); code MIT.
