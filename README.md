# Zemanium open geothermal research

Zemanium is a geothermal invention lab founded in 2026 by Toni Zemani. This
repository mirrors what is published at [zemanium.com](https://zemanium.com/):
guides, an LCOE calculator, simulation records and a power-cost model for enhanced and superhot
geothermal wells. It exists so that people and software agents can read,
check and cite the work from one place.

Contact: toni@zemanium.com

## What is here

| Path | What |
|---|---|
| `guides/geothermal-electricity-cost.md` | [Cost of geothermal energy in 2026](https://zemanium.com/guides/geothermal-electricity-cost) |
| `guides/geothermal-energy-pros-and-cons.md` | [Geothermal energy pros and cons, with the numbers](https://zemanium.com/guides/geothermal-energy-pros-and-cons) |
| `guides/geothermal-wells.md` | [Geothermal wells: depth, cost and lifespan](https://zemanium.com/guides/geothermal-wells) |
| `guides/geothermal-companies.md` | [Geothermal companies in 2026](https://zemanium.com/guides/geothermal-companies) |
| `guides/geothermal-stocks.md` | [Geothermal stocks in 2026](https://zemanium.com/guides/geothermal-stocks) |
| `guides/is-geothermal-energy-renewable.md` | [Is geothermal energy renewable? The field records](https://zemanium.com/guides/is-geothermal-energy-renewable) |
| `guides/enhanced-geothermal-systems.md` | [Enhanced geothermal systems: how they work and what limits them](https://zemanium.com/guides/enhanced-geothermal-systems) |
| `guides/superhot-rock-geothermal.md` | [Superhot rock geothermal: what happens above 375 °C](https://zemanium.com/guides/superhot-rock-geothermal) |
| `guides/firm-clean-power-compared.md` | [Geothermal, fission, fusion and space solar compared](https://zemanium.com/guides/firm-clean-power-compared) |
| `guides/fervo-project-red.md` | [Fervo Project Red: monthly record and registered forecast](https://zemanium.com/fervo-project-red) |
| `tools/lcoe-calculator.md` | [LCOE calculator and formula](https://zemanium.com/lcoe-calculator), with 2026 LCOE by energy source |
| `models/power-cost-model.html` | The [power-cost model](https://zemanium.com/confidence/) as one offline HTML file. Open it in a browser. |
| `records/` | Eight simulation records in JSON, with `TRACE.md` mapping each published number to its record |
| `open.md`, `about.md` | The [open research catalogue](https://zemanium.com/open/) and the [about page](https://zemanium.com/about) |
| `llms.txt`, `llms-full.txt` | Index and full text for language models |

## Numbers you can quote

- One simulated plant (200 °C initial rock, 25 years, 28.322 MW gross peak)
  costs $83.02/MWh on reference assumptions at an 8% real discount rate,
  $43.35/MWh on a target capital package at 8%, and $35.00/MWh on the same
  package at 4%. SIMULATED; source: power-cost model, 5 October 2026.
- Zemanium's conduction model matches the Nevada regulator's monthly record
  of Fervo's Project Red well pair to 0.51 °F on nine steady months.
  Forecasts registered 19 November 2026; code and record at
  https://github.com/tonizemani2/forecast-audit (doi:10.5281/zenodo.24396505).
- In 11 of 18 long-running Nevada geothermal fields the produced fluid is
  cooler than in its first recorded year; the median change is about 1.9 °F
  per year. Measured, operator-reported; computed by Zemanium.
- Zemanium's development target is firm geothermal power at $30 to $45 per
  MWh (target).

Figures from other organisations in the guides are credited to their sources
there.

## Licence

Text, figures and simulation records are licensed CC BY 4.0. Code is MIT.
See `LICENSE`. The Utah FORGE field data inside the model keeps its authors'
CC BY 4.0 licence (SLB and University of Utah, doi:10.15121/2473673).
Hardware drawings on the website are published for review with all rights
reserved; write to us for a licence to manufacture or use them commercially.

## Cite

Toni Zemani, "Zemanium open geothermal research", 2026,
https://zemanium.com/open/. See `CITATION.cff`.

## Work with us

We review geothermal forecasts, cost cases and test plans, run sponsored
experiments on hot-well problems, and license our hardware designs. Engineers
and investors are welcome too. Write to toni@zemanium.com and say what you
need to decide.
