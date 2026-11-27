Guide · [Toni Zemani](https://zemanium.com/about#toni-zemani) · 24 November 2026

# Is geothermal energy renewable? What the field records show.

Yes. Geothermal energy is renewable because the Earth keeps producing heat inside it, as the US Energy Information Administration puts it. A single reservoir can still cool when a plant draws heat faster than the rock refills it, and Nevada's public well records show how fast that happens, field by field.

Field temperatures and plant output are measured and operator-reported to the Nevada Division of Minerals. Flow-weighted means are computed by Zemanium from that record.

01 / Answer

## Is geothermal energy renewable or nonrenewable?

Geothermal energy is renewable. The heat comes from the Earth's interior, which keeps producing it, and power plants send the used water back underground. The EIA classes it as a renewable source on that basis.

The heat in one reservoir refills slowly, over decades to centuries. So a field can be renewable as a resource while a given well pair cools during its working life. Operators manage that with spacing, injection and new wells.

02 / Mechanism

## How does geothermal energy work?

1. Wells reach hot water or hot rock deep underground.
2. Hot water or steam rises to the surface and drives a turbine, directly or through a second fluid in a binary plant.
3. The cooled water goes back down an injection well and heats up again in the rock.

Because nothing burns and the loop runs in any weather, a geothermal plant delivers power around the clock. [Enhanced geothermal systems](https://zemanium.com/guides/enhanced-geothermal-systems) build the same loop in hot rock that has no natural water or cracks.

03 / Record

## What Nevada's field records show.

Nevada publishes the monthly temperature of every producing geothermal well. Across 18 fields with ten or more years of record and production in 2025, the flow-weighted mean temperature fell by more than 5 °F in 11, stayed within 5 °F in 3 and rose in 4. Statewide geothermal output was 5,044 GWh in 2019 and 5,031 GWh in 2025.

| Field (regulator code) | First year | First-year mean | 2025 mean | Change |
|---|---|---|---|---|
| Blue Mountain (BLU) | 2009 | 368 °F | 281 °F | -87 °F |
| WRS2 (WRS2) | 2015 | 261 °F | 212 °F | -49 °F |
| Jersey Valley (JVP) | 2012 | 331 °F | 292 °F | -38 °F |
| WRS (WRS) | 2013 | 260 °F | 227 °F | -32 °F |
| Brady Hot Springs (BHS) | 2012 | 280 °F | 248 °F | -32 °F |
| McGinness Hills 2 (MGH2) | 2015 | 336 °F | 307 °F | -29 °F |
| McGinness Hills (MGH) | 2012 | 335 °F | 306 °F | -29 °F |
| Tuscarora (TUS) | 2012 | 341 °F | 313 °F | -28 °F |
| Salt Wells (SWL) | 2009 | 276 °F | 248 °F | -28 °F |
| Steamboat (STB) | 2012 | 290 °F | 263 °F | -27 °F |
| Patua (PTA) | 2013 | 303 °F | 293 °F | -10 °F |
| Soda Lake (SDL) | 2012 | 329 °F | 325 °F | -4 °F |
| Dixie Valley (DXV) | 2012 | 330 °F | 330 °F | -1 °F |
| Wabuska (WAB) | 2012 | 209 °F | 209 °F | +0 °F |
| Desert Peak (DPK) | 2012 | 295 °F | 302 °F | +7 °F |
| San Emidio (SEM) | 2012 | 284 °F | 300 °F | +16 °F |
| Stillwater (STW) | 2009 | 270 °F | 297 °F | +27 °F |
| Beowawe (BEO) | 2012 | 274 °F | 324 °F | +50 °F |

A field's mean also moves when operators add or retire wells, so this table shows the produced fluid, not the rock alone. The yearly values for every field are in [one JSON file](https://zemanium.com/data/nevada-field-temperature.json), CC BY 4.0.

The clearest single well-pair record is Fervo's Project Red, which went from a 347 °F plateau in 2024 to 316 °F in July 2026. [See the monthly tracker](https://zemanium.com/fervo-project-red).

04 / Practice

## How operators keep a geothermal field hot.

- **Reinjection.** Sending the used water back keeps reservoir pressure up and returns the fluid for reheating. Most plants reinject, according to the EIA.
- **Well spacing.** Injection wells placed far enough from producers give the water more rock to heat it before it returns.
- **Makeup wells.** When a well cools, operators drill a new one into hotter rock nearby.
- **Even flow.** In enhanced systems, spreading flow across many fractures uses more rock and slows cooling. Our [reservoir explorer](https://zemanium.com/demo/) shows the effect.

05 / Trade-offs

## Geothermal energy pros and cons.

| Pros | Cons |
|---|---|
| Runs day and night in any weather | Good conventional sites are limited to hot regions |
| About 99% less carbon dioxide than fossil plants, per the EIA | Drilling is expensive and dominates the cost |
| Most plants send their water back underground, per the EIA | Single reservoirs can cool over a plant's life |
| Fuel cost is zero | Stimulation can trigger small earthquakes |

Our [cost guide](https://zemanium.com/guides/geothermal-electricity-cost) shows what geothermal electricity costs per megawatt-hour and which inputs move it.

06 / Questions

## Common questions.

### Why is geothermal energy considered renewable?

Because the Earth keeps producing heat in its interior, and power plants return the used water underground to be heated again. The US Energy Information Administration lists geothermal as a renewable energy source.

### Can a geothermal reservoir run out?

A reservoir can cool if heat is drawn out faster than the surrounding rock replaces it. In Nevada's records, 11 of 18 long-running fields produced cooler fluid in 2025 than in their first recorded year, and operators drill makeup wells to hold output.

### Is geothermal energy clean?

Geothermal plants burn no fuel. The EIA reports about 97% less sulfur compounds and about 99% less carbon dioxide than fossil fuel plants, and plants use scrubbers to remove hydrogen sulfide.

### How long does a geothermal power plant last?

Plants commonly run for decades, with wells replaced or added as fields cool. Our cost model assumes a 25-year life for a new plant.

07 / Sources

## Sources.

1. US Energy Information Administration, [Geothermal explained](https://www.eia.gov/energyexplained/geothermal/), read 24 November 2026.
2. US Energy Information Administration, [Geothermal energy and the environment](https://www.eia.gov/energyexplained/geothermal/geothermal-energy-and-the-environment.php), read 24 November 2026.
3. Nevada Division of Minerals, [Geothermal Production and Well Data](https://data-ndom.opendata.arcgis.com/pages/oilgasandgeothermalproduction), workbook of 29 September 2026. Measured, operator-reported.

Text and tables on this page are licensed [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). Cite as: Toni Zemani, "Is geothermal energy renewable? What the field records show", Zemanium, 24 November 2026. [All open models, records and drawings ](https://zemanium.com/open/)

---
Source: https://zemanium.com/guides/is-geothermal-energy-renewable
Publisher: Zemanium (https://zemanium.com/). Contact: toni@zemanium.com
Licence: text and figures CC BY 4.0 (https://creativecommons.org/licenses/by/4.0/); code MIT.
