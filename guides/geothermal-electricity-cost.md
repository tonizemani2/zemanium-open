Guide · Toni Zemani · 20 November 2026

# What geothermal electricity costs, and what sets the price.

A geothermal plant is paid for almost entirely before it produces anything. The cost of each megawatt-hour then depends on four things: what the wells cost, how much power each well delivers, how long that output lasts, and the interest rate on the money.

Numbers marked SIMULATED come from our own model and are scenarios built on assumptions. They are requirements for a design, and no plant has been built to them. Numbers from other organisations are quoted with their source.

01 / In brief

## The short answer.

- The US Department of Energy wants enhanced geothermal power at $45 per megawatt-hour by 2035. It describes that as a cut of about 90% from where the technology stood in 2022.
- ARPA-E's SUPERHOT program aims lower for wells above 375 °C: under $30 per megawatt-hour by 2040.
- In our own model the same simulated plant costs $83.02, $43.35 or $35.00 per megawatt-hour depending on its capital cost and discount rate. The rock and the wells are identical in all three cases.
- Zemanium's development target is $30 to $45 per megawatt-hour. It is what our hardware program is designed toward.

02 / Method

## How LCOE is calculated.

The levelized cost of electricity (LCOE) is the price per megawatt-hour at which a plant pays back everything spent on it over its life, including the return its lenders and owners expect. It divides discounted lifetime cost by discounted lifetime output:

`LCOE = sum of (cost in year t / (1 + r)^t) / sum of (electricity exported in year t / (1 + r)^t)`

Here `r` is the discount rate and `t` runs from construction to the last operating year. For geothermal the largest costs fall in year zero: drilling, completing the wells and building the power plant. Fuel is free. That makes the answer sensitive to the discount rate and to how long the wells keep their output.

Use exported electricity in the denominator. A geothermal plant spends some of its own output on pumps and auxiliaries, and an LCOE computed on gross generation flatters the plant. Our model exports gross generation minus pumping minus 5% of gross for auxiliaries.

03 / Targets

## Published cost targets.

| Who | Target | By | Applies to |
|---|---|---|---|
| US Department of Energy, Enhanced Geothermal Shot | $45/MWh | 2035 | enhanced geothermal systems |
| ARPA-E, SUPERHOT program | under $30/MWh | 2040 | reservoirs above 375 °C and 22 MPa, 10 to 20 GW |
| Zemanium | $30 to $45/MWh | development target, no date claimed | our hardware and well program |

The analysis behind the Department of Energy figure put developed deep enhanced geothermal at $45.60 per megawatt-hour in 2035, rounded to $45. All three rows are goals.

04 / Worked example

## One simulated plant, three prices.

Our power-cost model holds the physics fixed and changes only the money. The reservoir starts at 200 °C, runs for 25 simulated years, and feeds a plant sized to its peak output of 28.322 MW gross.

| Case | Capital assumptions | Real discount rate | LCOE |
|---|---|---|---|
| Reference | reference plant and well costs | 8% | $83.02/MWh |
| Target package | $1,500 per gross kW plant, $15m subsurface, $3m other | 8% | $43.35/MWh |
| Target package, cheaper money | same | 4% | $35.00/MWh |

SIMULATED · assumption scenarios · 5 October 2026

Halving the cost of capital takes $8.35 off each megawatt-hour without touching a single piece of equipment. Getting from $83.02 to $43.35 needs the plant and the wells to cost roughly what the target package says. No supplier has quoted those prices. They tell us what our hardware has to achieve.

The model runs 1,080 cost scenarios on output trajectories from GEOPHIRES-X 3.18.3, the open source simulator from NREL. It charges 2% of installed capital a year for operations, make-up water and $8 per exported megawatt-hour, books a $5m event in year 12 and $2m in year 25, and assumes the plant runs 90% of the time. A stress test draws 2,000 combinations of discount rate (4% to 12%), capital overrun (0.8 to 1.2 times) and a mid-life replacement of up to $10m.

05 / Drivers

## What moves the cost.

### Wells

The Department of Energy calls lower well construction cost a requirement for expanding enhanced geothermal, and puts casing and cementing alone at 30% to 40% or more of what a well costs. Drilling time is falling: Fervo Energy reports reaching 19,448 feet of measured depth in 21 days on its Sawtooth 7 well in July 2026.

### Power per well

A well that produces twice the power halves the drilling bill per megawatt. ARPA-E says today's equipment limits enhanced geothermal to about 220 °C and about 10 megawatts of electricity per production well, and that wells above 375 °C could reach 30 to 50. That gap is why developers want [superhot rock](https://zemanium.com/guides/superhot-rock-geothermal).

### How long the output lasts

Cold water injected into hot rock cools the rock it touches. If the water sweeps a small volume, the produced temperature falls early and every later year earns less. Our model includes a case that fails this way: with the reservoir volume cut from 1 cubic kilometre to 0.014, the plant ends up importing power, and we publish no price for it.

### Cost of capital

Because nearly all spending comes first, the discount rate acts on the whole bill. The example above moves 19% between 8% and 4%.

### The plant on the surface

Hotter fluid converts a larger share of its heat to electricity, so a 200 °C plant needs more equipment per kilowatt than a hotter one. The model lets you set installed plant cost from $1,500 to $4,500 per gross kilowatt.

06 / Tool

## Run the model yourself.

The [power-cost model](https://zemanium.com/confidence/) runs in your browser with no account. Set the plant cost, subsurface cost, discount rate and a target price, and it returns the LCOE and the capital the design can afford. It also shows the cases that fail. The 3D [reservoir explorer](https://zemanium.com/demo/) shows how flow, well spacing and rock temperature change thermal decline and pumping.

If you want this analysis for a specific project, or an independent review of a forecast, write to [toni@zemanium.com](mailto:toni@zemanium.com).

07 / Questions

## Common questions.

### Is geothermal energy expensive?

It is expensive to build and cheap to run. Almost all of the cost is drilling and plant construction paid up front, so the price per megawatt-hour depends on well cost, output per well, how long that output lasts and the interest rate. The US Department of Energy target for enhanced geothermal is $45 per megawatt-hour by 2035.

### How is the LCOE of a geothermal plant calculated?

Add up every cost over the plant's life, discount each year's cost back to today, and divide by the discounted electricity exported over the same years. Subtract pumping and auxiliary power from generation first, because the plant consumes them itself.

### How much does a geothermal well cost?

It depends on depth, rock and temperature, and few operators publish their costs. The US Department of Energy says casing and cementing make up 30% to 40% or more of a well's cost. Our model treats the whole subsurface scope as an allowance of $15m, $25m or $37m per case. Those are assumptions for comparison, and no contractor has quoted them.

### Is there a free geothermal LCOE calculator?

Yes. The Zemanium power-cost model at zemanium.com/confidence runs in a browser and needs no account. For full reservoir and plant simulation, GEOPHIRES-X is open source.

### Why does the discount rate matter so much for geothermal?

Nearly all the money is spent before the first megawatt-hour is sold, so the financing cost applies to almost the whole budget. In our simulated example the same plant costs $43.35 per megawatt-hour at an 8% real discount rate and $35.00 at 4%.

08 / Sources

## Sources.

1. US Department of Energy, [DOE launches new Energy Earthshot to slash the cost of geothermal power](https://www.energy.gov/articles/doe-launches-new-energy-earthshot-slash-cost-geothermal-power), 8 September 2022.
2. US Department of Energy, [Energy Earthshots initiative report](https://www.energy.gov/sites/default/files/2025-01/doe-energyearthshots-initiativereport.pdf), January 2025 ($45.60/MWh basis).
3. ARPA-E, [SUPERHOT program](https://arpa-e.energy.gov/programs-and-initiatives/view-all-programs/superhot), read 20 November 2026.
4. US Department of Energy, Office of Geothermal, [Enhanced geothermal systems](https://www.energy.gov/hgeo/geothermal/enhanced-geothermal-systems), updated 20 August 2026 (casing and cementing share of well cost).
5. Fervo Energy, [third-generation well design release](https://fervoenergy.gcs-web.com/news-releases/news-release-details/fervo-energy-learning-curve-continues-3rd-generation-well-design), 8 July 2026. Company statement.
6. Zemanium, [power-cost model](https://zemanium.com/confidence/), 5 October 2026. SIMULATED.
7. NREL, [GEOPHIRES-X](https://github.com/NREL/GEOPHIRES-X), version 3.18.3.

Text and figures on this page are licensed [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). Cite as: Toni Zemani, "What geothermal electricity costs, and what sets the price", Zemanium, 20 November 2026. [All open models, records and drawings ](https://zemanium.com/open/)

---
Source: https://zemanium.com/guides/geothermal-electricity-cost
Publisher: Zemanium (https://zemanium.com/). Contact: toni@zemanium.com
Licence: text and figures CC BY 4.0 (https://creativecommons.org/licenses/by/4.0/); code MIT.
