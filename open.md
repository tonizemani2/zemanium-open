Open research · updated 20 November 2026

# Open models, records and drawings.

This page lists everything Zemanium has published, what each item is, and what you may do with it. Use it, check it and build on it.

Model output is labelled SIMULATED, and field data is credited to the parties who measured it.

01 / Models

## Models you can run.

| Item | What it does | Basis |
|---|---|---|
| [Forecast and audit record, Project Red](https://github.com/tonizemani2/forecast-audit) | One command refits a conduction model to the Nevada regulator's monthly record of the first enhanced geothermal well pair, recomputes its water balance, and checks forecasts that were time-stamped on 19 November 2026. The model matches nine steady months to 0.51 °F. Each forecast is scored when the regulator publishes the month. | Model results on measured regulator data; code MIT, text CC BY 4.0; [doi:10.5281/zenodo.24396505](https://doi.org/10.5281/zenodo.24396505) |
| [Power-cost model](https://zemanium.com/confidence/) | Computes the cost per megawatt-hour of a geothermal plant from plant cost, subsurface cost and discount rate across 1,080 scenarios, with a 2,000-draw financial stress test. Shows the cases that fail. | SIMULATED, on GEOPHIRES-X 3.18.3 trajectories, 5 October 2026 |
| [LCOE calculator](https://zemanium.com/lcoe-calculator) | Returns the levelized cost of energy of any power plant from capital cost, operating cost, capacity factor, life and discount rate, with presets from Lazard's 2026 figures. | Formula of the National Laboratory of the Rockies; code MIT, text CC BY 4.0, 27 November 2026 |
| [Reservoir explorer](https://zemanium.com/demo/) | A 3D reservoir where you change flow, well spacing, permeability and rock temperature and see thermal decline, power and pumping. | SIMULATED, illustrative, earlier design assumptions |
| [Utah FORGE field replay](https://zemanium.com/confidence/#field) | 518 rows of a published production-log interpretation, with the unresolved intervals shown as gaps. | Measured and published by SLB and the University of Utah for Utah FORGE; CC BY 4.0; [doi:10.15121/2473673](https://doi.org/10.15121/2473673) |

02 / Records

## Simulation records.

Each file holds the inputs, assumptions, results and source hashes of one simulation campaign, in JSON. The four dated 3 October with "earlier" in their description used checkers we later revised; the [technical dossier](https://zemanium.com/docs/04-technical-dossier#records) gives the current results.

- [Temperature and cost ladder with declared stress boxes](https://zemanium.com/room/records/ladder-reinforced-2026-10-02.json), 2 October 2026
- [Flow and completion hydraulics sweep](https://zemanium.com/room/records/room-virtual-deliverability-2026-10-03.json), 3 October 2026
- [Thermal stroke screening and unit divergence](https://zemanium.com/room/records/room-virtual-stroke-envelope-2026-10-03.json), 3 October 2026
- [Drilling cost ranking sensitivity](https://zemanium.com/room/records/room-virtual-e8-robustness-2026-10-03.json), 3 October 2026
- [Earlier assembly gate failure matrix](https://zemanium.com/room/records/room-virtual-e7-matrix-2026-10-03.json), 3 October 2026
- [Earlier control loop fault matrix](https://zemanium.com/room/records/room-virtual-e9-matrix-2026-10-03.json), 3 October 2026
- [Earlier record validator adversarial corpus](https://zemanium.com/room/records/room-virtual-record-corpus-2026-10-03.json), 3 October 2026
- [Earlier duty corner checker exercise](https://zemanium.com/room/records/room-virtual-duty-corners-2026-10-03.json), 3 October 2026

[The source trace](https://zemanium.com/room/records/TRACE.md) maps every number on the research page to the record it came from.

03 / Hardware

## Hardware drawings.

These are development drawings of engineering geometry. Release for hot service is decided by physical test campaigns at the matching duty.

- [SL-D01-A release demonstrator, dimensioned build sheet](https://zemanium.com/assets/hardware/SL-D01-A-build-sheet.svg). Room temperature, 56 mm of gate travel.
- [Release demonstrator, exploded view](https://zemanium.com/assets/hardware/shiftlatch-demo_exploded.svg), with [held](https://zemanium.com/assets/hardware/shiftlatch-demo_held.svg) and [released](https://zemanium.com/assets/hardware/shiftlatch-demo_released.svg) states.
- [E7-SPC-B specimen kit, build sheet](https://zemanium.com/assets/hardware/E7-SPC-B-kit-build-sheet.svg).
- [Sliding seal cassette, cutaway](https://zemanium.com/assets/hardware/thermoslip-cassette-cutaway.svg).
- [Thermal test bench, general arrangement](https://zemanium.com/assets/hardware/heatmux-thermal_verification_general-arrangement-preview.png).

The [research page](https://zemanium.com/room/#machines) shows each drawing with its development record.

04 / Writing

## Guides and reference.

- [What geothermal electricity costs, and what sets the price](https://zemanium.com/guides/geothermal-electricity-cost)
- [Enhanced geothermal systems: how they work and what limits them](https://zemanium.com/guides/enhanced-geothermal-systems)
- [Superhot rock geothermal: what happens above 375 °C](https://zemanium.com/guides/superhot-rock-geothermal)
- [Geothermal stocks in 2026: the listed producers and what their plants deliver](https://zemanium.com/guides/geothermal-stocks)
- [Is geothermal energy renewable? What the field records show](https://zemanium.com/guides/is-geothermal-energy-renewable)
- [The energy source of the future, compared](https://zemanium.com/guides/firm-clean-power-compared)
- [Fervo Project Red tracker](https://zemanium.com/fervo-project-red): the monthly record against our registered forecast
- For agents: MCP server at `https://zemanium.com/mcp` and JSON records under [/data/](https://zemanium.com/data/project-red-monthly.json), CC BY 4.0
- [Technical dossier](https://zemanium.com/docs/04-technical-dossier): methods, test duties and results for each program

05 / Licence

## What you may do with it.

| Material | Licence | In practice |
|---|---|---|
| Guides, page text, charts and simulation records | [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) | Copy, quote, translate and build on it, commercially or otherwise, if you credit Zemanium and link the page. |
| Code in the pages and models | [MIT](https://opensource.org/license/mit) | Use it in your own software and keep the copyright notice. |
| Hardware drawings | Published for review, all rights reserved | Read them, check them, cite them. To manufacture from them or use them commercially, ask us for a licence. |
| Utah FORGE data | CC BY 4.0, from its authors | Credit SLB, the University of Utah and Utah FORGE as the source record does. |
| The Zemanium name and logo | Not licensed | Use the name to refer to us. |

Copyright 2026 Toni Zemani.

06 / Citation

## How to cite.

For a guide: Toni Zemani, title of the guide, Zemanium, date shown on the page, and its address. For a model or record: Zemanium, name of the item, its date, its address, and the label it carries (SIMULATED).

Example: Zemanium, "Power-cost model", 5 October 2026, https://zemanium.com/confidence/. SIMULATED.

07 / Agents

## For software agents.

[llms.txt](https://zemanium.com/llms.txt) lists every page with a one-line description. [llms-full.txt](https://zemanium.com/llms-full.txt) holds the guides in one Markdown file. Each guide also has a Markdown copy at its own address with `.md` added. The [sitemap](https://zemanium.com/sitemap.xml) lists canonical addresses. Search and AI crawlers are allowed on the whole site, and the same files are mirrored at [github.com/tonizemani2/zemanium-open](https://github.com/tonizemani2/zemanium-open).

08 / Contact

## Work with us.

We publish so that specialists can check the work, and so that people with a problem we can help with can find us. Three kinds of conversation have a clear next step.

| You have | We can |
|---|---|
| A forecast, cost case or test plan you need checked | Review it independently and give you the numbers we reproduce and the ones we cannot |
| A well, tool or material problem above 200 °C | Scope a sponsored experiment with a fixed question, a named engineer and raw results at the end |
| A use for one of the hardware designs | License it, or develop it with you |

Write to [toni@zemanium.com](mailto:toni@zemanium.com) with what you need to decide. Investors and engineers who want to join are welcome at the same address.

---
Source: https://zemanium.com/open/
Publisher: Zemanium (https://zemanium.com/). Contact: toni@zemanium.com
Licence: text and figures CC BY 4.0 (https://creativecommons.org/licenses/by/4.0/); code MIT.
