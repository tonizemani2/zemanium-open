Guide · [Toni Zemani](https://zemanium.com/about#toni-zemani) · 27 November 2026

# The geothermal gradient: how much hotter the Earth gets with depth.

The geothermal gradient is the rate at which rock temperature rises with depth. In most continental crust away from plate boundaries it is about 25 to 30 °C per kilometre. It varies with the heat flowing up from below and with the rock: across the United States it runs from 15 to 35 °C per kilometre, averaging 25 in the east and 34 in the west. On the world's median heat flow, 200 °C rock sits about 8.5 km down.

Gradients by region are quoted from the US Geological Survey and the Geological Society. The depth table and maps are a Zemanium conduction model (labelled [MODEL]) run on the measured values of the IHFC Global Heat Flow Database 2024.

01 / Answer

## What is the geothermal gradient?

It is the increase in temperature per unit of depth below the surface, usually given in °C per kilometre. Away from plate boundaries and hotspots, temperature rises about 25 to 30 °C per kilometre in the lithosphere, by the Geological Society's teaching guidance.

| Where | Gradient | Source |
|---|---|---|
| Typical continental crust | 25 to 30 °C per km | Geological Society |
| Most of the contiguous United States, to 2 km | 15 to 35 °C per km | USGS, Nathenson and Guffanti |
| Eastern United States, average | 25 °C per km | USGS, Nathenson and Guffanti |
| Western United States, average | 34 °C per km | USGS, Nathenson and Guffanti |
| World median heat flow (59 mW/m²), at the surface | about 24 °C per km | Zemanium [MODEL] on IHFC data |
| Region around Milford, Utah (92 mW/m²) | about 37 °C per km | Zemanium [MODEL] on IHFC data |
| Region around Tirana, Albania (31 mW/m²) | about 12 °C per km | Zemanium [MODEL] on IHFC data |

02 / Formula

## How the geothermal gradient is calculated.

Heat flows up through rock by conduction. The gradient is the heat flow divided by the rock's thermal conductivity:

`gradient (°C per km) = heat flow (mW/m²) / thermal conductivity (W/m/K)`

At the world's median continental heat flow of 59 milliwatts per square metre and a conductivity of 2.5 W/m/K, the gradient at the surface is 59 / 2.5 = 23.6 °C per kilometre. The USGS derived an average conductivity of 2.5 ± 0.8 W/m/°C for US rock between a few hundred metres and 2 km. Rock that conducts heat poorly, such as thick sediment, steepens the gradient; rock that conducts well, such as granite, flattens it.

The gradient also eases with depth, because part of the surface heat flow is made inside the crust by radioactive decay. Our model takes 1 µW/m³ of that heat in the top 10 km and a surface temperature of 12 °C.

03 / Depth

## How deep do you have to drill to reach a given temperature?

We ran the conduction model on every measured onshore cell of the IHFC Global Heat Flow Database 2024: 51,882 values in 4,515 cells of one degree. The table gives the share of measured continental area where each temperature lies within each depth, and the median depth.

| Temperature | within 5 km | 7 km | 10 km | 12 km | 15 km | median depth |
|---|---|---|---|---|---|---|
| 150 °C | 30% | 63% | 86% | 92% | 97% | 6.1 km |
| 200 °C | 9% | 32% | 65% | 78% | 89% | 8.5 km |
| 250 °C | 3% | 13% | 42% | 58% | 75% | 10.9 km |
| 400 °C | 0.3% | 1.5% | 7.5% | 14% | 30% | 18.5 km |

[MODEL] on measured data · 27 November 2026

![Line chart of the share of measured continental area where 150, 200, 250 and 400 °C lie within drilling depths from 3 to 15 km, with uncertainty bands for rock conductivity](https://zemanium.com/assets/charts/depth-to-temperature-reach.webp)

Bands show rock conductivity from 2.2 to 3.0 W/m/K. The dotted lines mark Fervo's 5.9 km well drilled in 21 days in 2026 and the deepest hole ever drilled, Kola, at 12.26 km. Free to reuse under CC BY 4.0 with credit to Zemanium.

For 200 °C the median depth ranges from 7.4 to 10.3 km across that conductivity band. Unmeasured land is left out, not counted as cold.

04 / Map

## Where the heat is closest to the surface.

![World map of the modelled depth to 200 °C in every measured one-degree cell of continental land; shallow cells in orange cluster in the western United States, central Europe, East Africa and around the Pacific](https://zemanium.com/assets/charts/depth-to-200c-map.webp)

Depth to 200 °C from the median heat flow in each measured one-degree cell, IHFC Global Heat Flow Database 2024. Blank land is unmeasured. [MODEL] on measured data; free to reuse under CC BY 4.0 with credit to Zemanium.

The shallowest heat follows young tectonics and volcanism: the western United States, Iceland, East Africa's rift, Indonesia, New Zealand and the rim of the Pacific, where the EIA notes most major geothermal resources sit. Old continental interiors run cooler. Local hot spots can be far hotter than their region: Cape Station in Utah drills into a local anomaly inside a region whose median heat flow puts 200 °C at 5.3 km.

05 / Variation

## Why the gradient changes from place to place.

- Heat flow from below. Thin, young or stretched crust, rifts and volcanic arcs let more heat through.
- Rock conductivity. The USGS found gradients raised where thick, poorly conducting sediments lie, such as the Atlantic Coastal Plain and basins of the Great Plains.
- Moving water. Hot water rising along faults carries heat upward, which is what makes a conventional hydrothermal field.
- Heat made in the rock. Granite rich in uranium, thorium and potassium adds heat of its own.

06 / Power

## What the gradient means for geothermal power.

A binary power plant can run on water from about 110 °C, and flash plants on 200 °C and hotter, by the national laboratories' cost baseline. On a typical gradient that means drilling several kilometres; on a steep one, far less. Iceland's IDDP-2 well logged 426 °C at about 4.55 km.

Hotter rock yields more electricity per well, so the gradient sets how many wells a plant needs. Enhanced geothermal and superhot rock projects drill deeper to reach that heat in more places. Our guides to [geothermal wells](https://zemanium.com/guides/geothermal-wells), [enhanced geothermal systems](https://zemanium.com/guides/enhanced-geothermal-systems) and [superhot rock](https://zemanium.com/guides/superhot-rock-geothermal) pick up from here, and the [cost guide](https://zemanium.com/guides/geothermal-electricity-cost) shows what depth does to the price.

07 / Questions

## Common questions.

### What is the average geothermal gradient?

About 25 to 30 °C per kilometre in continental crust away from plate boundaries. On the world's median measured heat flow of 59 mW/m² and typical rock, it is about 24 °C per kilometre at the surface.

### How do you calculate the geothermal gradient?

Divide the heat flow by the rock's thermal conductivity. At 59 mW/m² and 2.5 W/m/K, the gradient is 23.6 °C per kilometre. In a borehole, divide the temperature difference between two depths by the distance between them.

### How hot is it 1 km underground?

On a typical gradient of 25 to 30 °C per kilometre and a surface temperature near 12 °C, rock 1 km down is about 37 to 42 °C. In the western United States, with an average gradient of 34 °C per kilometre, it is closer to 46 °C.

### How deep do you need to drill to reach 200 °C?

About 8.5 km at the median of the world's measured continental heat flow, and less than 5 km in 9% of measured land, by our model on the IHFC database. Geothermal regions such as parts of Utah and Nevada reach it far shallower.

### Where is the geothermal gradient highest?

Near plate boundaries, rifts and volcanoes: Iceland, the western United States, East Africa, Indonesia, the Philippines, New Zealand and the Pacific rim. Old continental shields have the lowest gradients.

08 / Sources

## Sources.

1. Global Heat Flow Data Assessment Group and others, [The Global Heat Flow Database: Release 2024](https://doi.org/10.5880/fidgeo.2024.014), version 2026.03, GFZ Data Services, CC BY 4.0.
2. Nathenson and Guffanti, [Geothermal gradients in the conterminous United States](https://www.usgs.gov/publications/geothermal-gradients-conterminous-united-states), Journal of Geophysical Research, 1988, doi:10.1029/JB093iB06p06437.
3. Geological Society of London, [Geothermal gradient and magma generation, teachers' guidance](https://www.geolsoc.org.uk/media/uitj2igl/ks5-geothermal-gradient-teachers-notes.pdf), read 27 November 2026.
4. US Energy Information Administration, [Where geothermal energy is found](https://www.eia.gov/energyexplained/geothermal/where-geothermal-energy-is-found.php), read 27 November 2026.
5. National Laboratory of the Rockies, [Annual Technology Baseline 2025: geothermal](https://atb.nlr.gov/electricity/2025/2023/geothermal), read 27 November 2026 (binary and flash temperature ranges).
6. Friðleifsson and others, IDDP-2 at Reykjanes, Proceedings World Geothermal Congress 2020+1, paper 31002.
7. Zemanium, depth-to-temperature model on the IHFC database: conduction with k = 2.5 W/m/K (2.2 to 3.0), 1 µW/m³ of radiogenic heat in the top 10 km, surface 12 °C; registered and time-stamped before the run, 27 November 2026. [MODEL].

Text, tables and figures on this page are licensed [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). Cite as: Toni Zemani, "The geothermal gradient: how much hotter the Earth gets with depth", Zemanium, 27 November 2026. [All open models, records and drawings ](https://zemanium.com/open/)

---
Source: https://zemanium.com/guides/geothermal-gradient
Publisher: Zemanium (https://zemanium.com/). Contact: toni@zemanium.com
Licence: text and figures CC BY 4.0 (https://creativecommons.org/licenses/by/4.0/); code MIT.
