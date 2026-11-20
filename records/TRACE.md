# ROOM TRACE — every number in the room, record → label → caveat

`company/room/` · 3 October 2026 · the room's trace under the same standing
laws as `company/CLAIM-TRACE.md` (S1–S8, restated below). A number in
`company/room/content.py` that cannot be placed here makes the build fail
(`tools/build-room.py` refuses untraced numbers). Chart data values are read
from the cited `qa/` records at build time by the same build and carry their
provenance in the chart captions (S8 treatment).

---

## 1. Standing laws (S1–S8, from company/CLAIM-TRACE.md)

| # | Law | In the room |
|---|---|---|
| S1 | Fractions of a box are never probabilities | §01 stat cards, MC box chart footnote, §06 readbox |
| S2 | Contract box = fixed-price EPC + long-tenor debt; assumed, not a guarantee | §01 body |
| S3 | Every $/kW quote states scope: installed vs equipment, gross vs net | §04 P-E3 rows, §08 risk 5 |
| S4 | Ladder rows are different project definitions — never additive; spec and real-cost are two series | §00 chart, §01 chart caption |
| S5 | Label vocabulary: measured · verified · vendor-stated · model · simulated · inference · assumption · proposed · TBD | every number below |
| S6 | Zero measured duty hours, said in every materials set | §00 stats, §13 |
| S7 | The reinforced run reproduces R5 = $29.80 to 1e-9 before re-pricing | §01 body |
| S8 | Structural numbers are identifiers (sections, claims, records, contracts), not claims | §6 register below |

## 2. Economics rows

| Quote in the room | Source (+ key) | Label | Caveat |
|---|---|---|---|
| `$61.65` spec target row | `qa/thirty-mwh-audit-2026-09-14.json` → `coupled_cases.target.lcoe_usd_mwh` = 61.64919219348134 | model | audited arithmetic on assumed inputs |
| `$47.46` / `$34.06` spec rows (300 °C $25m $1,800 / $25m $1,000) | same → `hotter_fixed_flow_sensitivities` (300, 25, 1800) = 47.46; (300, 25, 1000) = 34.06 | model | different project definitions (S4) |
| `$29.80` spec row (320 °C $15m $1,000) | same → (320, 15, 1000) = 29.80 | model | R5 spec row |
| "reproduces the audited $29.80 row exactly — to nine decimal places" | `qa/ladder-reinforced-2026-10-02.json` → `transcription_gate` (29.801515451011966, matches to 1e-9) | model + SIMULATED | S7 |
| `$30.44` R5P nominal | `qa/ladder-reinforced-2026-10-02.json` → `R5P_320c_allowance_realphysics.declared_box.nominal_lcoe_usd_mwh` | SIMULATED | allowance case at real physics |
| `$45.72` R5C nominal · "holds $30 in 0% of both boxes" | same → `R5C_320c_combined_realcost` nominal = 45.719…; `frac_le_30` = 0.0 both boxes | SIMULATED | 0% rows stay visible (S6 doctrine) |
| `$37.19` R6S nominal · "$45 band across 77–99.9%" | same → `R6S_500c_today_cost` nominal = 37.186…; `frac_le_45` declared = 0.77045 (77.0%), contract = 0.9994 (99.9%) | SIMULATED | box fractions, never probabilities (S1) |
| `$31.11` R6T nominal | same → `R6T_500c_e3_target` nominal = 31.113… | SIMULATED | at the E3 target cost class |
| `$24.58` R6D nominal · "holds $30 in 80% of the declared box and 99.9% of the contract box" | same → `R6D_500c_design_2458` nominal = 24.580…; `frac_le_30` = 0.8 / 0.999 | SIMULATED | design spec, not a forecast (S2) |
| "about $970 per gross-kW" (R6D solved surface) | same → `design_rule.solved_surface_usd_per_gross_kw` = 969.7 | SIMULATED / assumption | installed scope, gross basis (S3) |
| "≤$1,400/gross-kW" (P-E3-02) | `inventions/RED-TEAM.md` frozen-prediction register P-E3-02 | proposed (frozen prediction) | judged by scope-matched RFQ offers |
| "±$130/gross-kW" (escalation sensitivity) | `inventions/RED-TEAM.md` open item 5 (±0.15 on ×1.60 moves anchors ~±$130/kW) | assumption | RFQ price basis is the measurement |
| `×1.60` 2007→2025 USD escalation · `±0.15` | `inventions/RED-TEAM.md` open item 5 | assumption | unquoted basis |

## 3. Deliverability, hydraulics (VP1, this session)

| Quote | Source (+ key) | Label | Caveat |
|---|---|---|---|
| `294 kg/s` (declared superhot flow) · `~50 kg/s` IDDP-class | `qa/ladder-reinforced-2026-10-02.json` → `limits[1]`; W1B-018 class measured deliverability | assumption vs measured | red-team open item 1 |
| `100 kg/s` (R6S band threshold) | `qa/room-virtual-deliverability-2026-10-03.json` → `survival_summary.R6S_500c_today_cost.holds_45_at_100kg_s_audited` | SIMULATED | nominal under audited hydraulics |
| `$46.28` R6S at 50 kg/s · `$40.20` R6T · `$33.67` R6D | same → `red_team_open_items.1_deliverability.cells` (charged q3 nominal) | SIMULATED | pumping charged, q3 law declared |
| `29.14 MW` 7 in pump · `0.67 MW` 12 in pump · `43`× swing | `qa/geophires-crosscheck-2026-10-02.json` → `e_swing_term` (29.14 / 0.67 / 43.49) | SIMULATED (GEOPHIRES-X) | external cross-check, never design authority |
| "12.7% of gross" (7 in at 294) · "0.3% of gross" (12 in) | `qa/room-virtual-deliverability-2026-10-03.json` → `red_team_open_items.2_completion_hydraulics.cells.pump_share_of_gross_*` | SIMULATED | pump electricity kept separate from recovered output (house rule) |

## 4. Duty, mechanics, machines

| Quote | Source | Label | Caveat |
|---|---|---|---|
| `100` cycles `500 ↔ 150` °C · `30 MPa` · `500 h` hold | `next-stage/build/e7-assembly/duty_spec.json` (cycles, temperatures_c, pressure_mpa, hold_hours) | proposed (frozen before fabrication) | DC-4 duty |
| checkpoints `1, 10, 25, 50, 75, 100` · destructive at `50`/`100` | same → `checkpoints` | proposed | leak + stroke at every checkpoint |
| `25 K/min` bounding quench · `0.1 K` margin (E4 worst corner) | same → `rates.bounding_quench_k_per_min`; `inventions/MAP.md` E4 row | proposed / SIMULATED | bounded, not measured |
| `552 MPa` L-80 · `862 MPa` TN125SS · `931 MPa` quench stress | `next-stage/REFERENCE-CASE.md §4`; `next-stage/build/e7-assembly/stackup.py` (190 GPa, 14e-6/K, ΔT 350 K) | verified (API 5CT) / assumed / [MODEL] | screening arithmetic, not FEA |
| `25.8` mm per 10 m vs `2.5–3` mm band · strain `2.58e-3` | `qa/room-virtual-stroke-envelope-2026-10-03.json` → `frozen_point` (25.758 mm/10 m, strain 0.002576) | SIMULATED ([MODEL]) | the campaign verifies which reading the hardware needs (VP6) |
| `56 mm` full travel · `54–138 µm` window class | `hardware/shiftlatch-demo/geometry-check.json` (travelMm 56); `inventions/RED-TEAM.md` P-E1-01 | measured (geometry) / SIMULATED (prediction) | mechanism demonstrator |
| `+60/−20 mm` collar travel · `220 mm` OD · `800 mm` housing | `hardware/thermoslip-cassette/design.json` (positiveTravel 60, negativeTravel 20, outerOd 220, housingLength 800) | assumed (geometry) | seal interface UNRESOLVED_SUPPLIER_CARTRIDGE |
| kit sizes `219.1 × 300` · `273 × 300` · `245 × 120` · `80 × 30 × 8` · `320 × 320 × 20` mm · clearance `1.0` mm | `next-stage/build/e7-assembly/design.json` (duty_spec.json specimen.parts) | assumed (envelope) | CONCEPT_SPECIMEN_GEOMETRY_ONLY |
| `±5 °C` through `500 h` at `450 °C` (DC-1 keystone) | `next-stage/build/q-platform/duty_classes.json` DC-1; `inventions/RED-TEAM.md` P-E0-01 | proposed (frozen prediction) | bench confirms or kills |
| safe-state deadlines `30/5/30/10 s` | `next-stage/build/e9-loop/task_set.json` → `safe_state_times` | proposed (frozen) | verdict rides on these values (VP3) |
| `250/300/320 °C` seal cycle classes | `inventions/RED-TEAM.md` P-E5-01 | SIMULATED (prediction) | cycled-seal bench judges it |
| duty classes `250/300/374` °C · `374` °C class ceiling | `inventions/MAP.md` G4 (250 → 300 → 374 °C duty classes) | model / proposed | requirements with gates, not built hardware |
| `0.90` stability threshold · `0.90–1.15`× anchor band | `next-stage/build/e8-cost-case/well_cost_case.py` (STABILITY_THRESHOLD); P-E3-01 | proposed / SIMULATED | E8-F1 gate form |
| `6` VP4 variants all INDETERMINATE | `qa/room-virtual-e8-robustness-2026-10-03.json` → `variants` | SIMULATED | declared ranges only; RFQ moves the numbers |
| `12` VP2 scenarios · `9` VP3 scenarios · `15` VP5 cheats | `qa/room-virtual-e7-matrix-2026-10-03.json` · `room-virtual-e9-matrix-2026-10-03.json` · `room-virtual-record-corpus-2026-10-03.json` | SIMULATED | synthetic campaigns, no physical run |

## 5. The case, the market, the programs

| Quote | Source | Label | Caveat |
|---|---|---|---|
| `4,659` m · `176` drilling days · `2,500` m start | `next-stage/REFERENCE-CASE.md §1` (W1B-014) | measured | IDDP-2 |
| `426–427` °C at `340` bar · `535` °C after five-month stimulation | same (W1B-014, W1B-015) | measured | ~600 °C inferred from petrology |
| `2,300–2,400` m damage zone · losses below `3,060` m | same (W1B-015, W1B-014) | measured | one unplanned transient |
| `20`-well base rate (collapse/connection rupture) | `next-stage/REFERENCE-CASE.md §4` (W1B-019) | measured synthesis | the aggregate version of W1B-015 |
| `374.1` °C / `22.06` MPa critical point · ARPA-E `>375` °C / `>22` MPa | `next-stage/REFERENCE-CASE.md §0` (physical constant; W1A-027) | verified | temperature alone decides nothing |
| `350` °C connection-testing wall · `375–400` °C no service | `next-stage/REFERENCE-CASE.md §2` (W1B-021); market scan 2026-09-29 | measured / verified | the certificate gap |
| run order `7 → 6 → 5 → 8 → 9` | `next-stage/HUMAN-QUEUE.md §3` | assumption (plan) | cheapest decisive measurement first |
| `$5–15k` · `$60–180k` · `$200–450k` · `$80–250k` · `$80–150k` · `$320–640` · `$550k–1.0M` | `next-stage/HUMAN-QUEUE.md §2`; `next-stage/downselect.md §4–§7` | assumption | sums of assumed ranges, not a budget quote |
| `11,041,343` US patent · expires `2038` | `qa/invention-series-wave-b.json` (priority 2015-12-18, expiry 2038-03-25) | verified (patent record) | sliding-seal claim blocked; filing halted |
| `126` build tests · `163` engine contracts (`107 + 7 + 49`) · `37` tests (E0 readout) | `qa/next-stage-build-2026-10-02.json` (ran_all 126); `qa/reality-pass-2026-10-02.json` (reconciled_total 163); `company/MASTER-PLAN.md §1` | measured (test counts) | contracts prove software behavior on declared inputs, never hardware qualification |
| `2026-10-02` freeze dates · `2026-10-03` room date | `inventions/RED-TEAM.md` (P-rows 2026-10-02); build date | fact | |

## 6. Identifier register (S8 — structural, not claims)

Section ids `00`–`13` · programs `O-01`–`O-05` · machines `E0`–`E9` · duty
classes `DC-1`–`DC-7` · contracts `A1`–`A11`, `L1`–`L8`, `W1`–`W5`, `C1`–`C10`
· pushes `VP1`–`VP7` · claims `W1B-014`, `W1B-015`, `W1B-018`, `W1B-019`,
`W1B-021`, `W1B-022`, `W1A-026`, `W1A-027`, `W2D-014` · law `R-20`, `R-23` ·
gate ids `E7-F1`–`E7-F6`, `E9-F1`–`E9-F4`, `E8-F1`, `E6-F1`–`E6-F5` ·
predictions `P-E0-01`, `P-E1-01`, `P-E2-01`, `P-E2-02`, `P-E3-01`, `P-E3-02`,
`P-E5-01` · standards `IEEE Std 323` · packages `SL-D01-A`, `TS-M01-A`,
`SP-R01`, `RL-B03` · specs `E7-DC4-DUTY-SPEC-REV0`, `E9-TASKSET-REV0` ·
records `qa/ladder-reinforced-2026-10-02.json`,
`qa/thirty-mwh-audit-2026-09-14.json`, `qa/geophires-crosscheck-2026-10-02.json`,
`qa/next-stage-build-2026-10-02.json`, `qa/reality-pass-2026-10-02.json`,
`qa/room-virtual-deliverability-2026-10-03.json`,
`qa/room-virtual-e7-matrix-2026-10-03.json`,
`qa/room-virtual-e9-matrix-2026-10-03.json`,
`qa/room-virtual-e8-robustness-2026-10-03.json`,
`qa/room-virtual-record-corpus-2026-10-03.json`,
`qa/room-virtual-stroke-envelope-2026-10-03.json`,
`qa/room-virtual-duty-corners-2026-10-03.json` · engines `assembly_gate.py`,
`loop_gate.py`, `well_cost_case.py`, `record_validator.py`, `stackup.py`,
`latch_campaign.py` · drafts `RFQ-TEXT.md`, `ASKS.md` · doc ids `A1`, `D1`–`D5`
· O-01 fixture ids `P-1`–`P-6` · `SSI-1.5` deposit class · deck slide format `16:9` (structural) · mission date
`2035` (DOE $45/MWh target band, `company/comms/PLAN.md §1`).

## 7. Machine token register (build-enforced)

Every numeric token that appears in `company/room/content.py` copy must be in
this file; `tools/build-room.py` fails the build otherwise. Tokens map to the
rows above or to the identifier register in §6.

`0` `1` `2` `3` `4` `5` `6` `7` `8` `9` `01` `02` `03` `04` `05` `06` `07`
`08` `09` `10` `11` `12` `13` `15` `20` `25` `30` `37` `43` `45` `50` `54` `56`
`60` `77` `80` `90` `95` `100` `107` `120` `125` `126` `130` `138` `150` `163`
`176` `180` `200` `245` `250` `273` `294` `300` `320` `323` `340` `350` `375`
`400` `426` `427` `450` `500` `535` `550` `552` `640` `931` `970` `1,400`
`2,300` `2,400` `2,500` `4,659` `11,041,343` `0.1` `0.15` `0.3` `0.67` `0.90`
`1.0` `1.15` `1.5` `1.60` `2.5` `2.58` `12.7` `22.06` `24.58` `25.8` `29.14`
`29.80` `30.44` `31.11` `33.67` `37.19` `374` `374.1` `40.20` `45.72` `46.28` `61.65`
`77.0` `99.9` `219.1` `2007` `2025` `2026` `2038`
