# HSN — Human Scale Numbers

*Also available in Polish: [README](README_PL.md)*

A small set of round numbers that cover the whole range of everyday measurements — and fit together so you can scale anything without recalculating.

Instead of "a bit more", you use the next value up. Instead of multiplying by 1.6, you shift every value by the same number of steps. The numbers are designed to be memorable, and the steps are designed to be meaningful.

HSN works wherever you measure, experiment, or scale: cooking, training, finances, time, 3D modelling, game design, and more.

## The sequence

| Step | Value |
|------|-------|
| 0 | 1 |
| 1 | 1.25 |
| 2 | 1.6 |
| 3 | 2 |
| 4 | 2.5 |
| 5 | 3.2 |
| 6 | 4 |
| 7 | 5 |
| 8 | 6.4 |
| 9 | 8 |
| 10 | 10 |

Then continues: 12.5, 16, 20, 25, 32, 40, 50, 64, 80, 100 …

## How to remember the values

The sequence is easy to memorize once you notice it consists of three simple interleaved doubling series:

- **1 — 2 — 4 — 8** (×2 each time)
- **1.25 — 2.5 — 5 — 10** (×2 each time)
- **1.6 — 3.2 — 6.4** (×2 each time, also recognizable as 16 — 32 — 64)

Each series doubles at every step; the three series are interleaved to form the full HSN sequence.

## Scaling without recalculating

Because the sequence is geometric, common multiplications become simple step shifts:

| Operation | Steps |
|-----------|-------|
| ×2 (or ÷2) | +3 (or −3) |
| ×3 (or ÷3) | +5 (or −5) — approximate |
| ×10 (or ÷10) | +10 (or −10) |

To double any quantity, shift 3 steps up. To scale down by a third, shift 5 steps down. The same logic applies across domains:

- **Cooking** — scale a recipe for one person or a whole family
- **Training** — progress from 3.2 to 4 to 5 km
- **Finances** — set pocket money that grows meaningfully with age
- **Time** — choose brewing or cooking durations from the time variant
- **3D modelling** — pick dimensions that relate to each other consistently
- **Game design** — build a numeric scale for mechanics (e.g. a power meter)

## Time variant

For time, the sequence is adapted to hours and minutes:

| Step | Value |
|------|-------|
| 0 | 1:00 |
| 1 | 1:15 |
| 2 | 1:36 |
| 3 | 2:00 |
| 4 | 2:30 |
| 5 | 3:12 |
| 6 | 4:00 |
| 7 | 5:00 |
| 8 | 6:24 |
| 9 | 8:00 |
| 10 | 10:00 |
| 11 | 12:30 |
| 12 | 16:00 |
| 13 | 20:00 |
| 14 | 25:00 |
| 15 | 32:00 |
| 16 | 40:00 |
| 17 | 50:00 |
| 18 | 1:00:00 |

Then continues in hours, with 1 day replacing the "25 h" step.

Just as the main sequence consists of three interleaved doubling series, so does the time variant:

- **1:00 — 2:00 — 4:00 — 8:00** (×2 each time)
- **1:15 — 2:30 — 5:00 — 10:00** (×2 each time)
- **1:36 — 3:12 — 6:24** (×2 each time, i.e. 1:30+0:06, 3:00+0:12, 6:00+0:24)

## Example: waffle recipe

The recipe was developed by iterative experimentation using HSN values, then scaled up by 2 steps (≈ ×1.6) to serve a larger family — without recalculating any proportions:

| Ingredient | Amount |
|------------|--------|
| Eggs | 3 |
| Milk | 500 ml |
| Wheat flour | 400 g |
| Baking powder | 1.6 tsp |
| Rapeseed oil | 100 ml |

Milk (500 ml) and flour (400 g) sit precisely on HSN values. Eggs come in whole numbers — rounded to the nearest integer. Baking powder at 1.6 tsp is an HSN value; in practice 1.5 tsp works equally well — a reminder that HSN is a starting point, not a constraint.

See also: [Kitchen measuring tools specification](tools.md)

## For the curious

HSN is a human-oriented adaptation of the R10 Renard series (ISO 3, 1952) and is structurally similar to the E12 series used in electronics. Those systems were designed for manufacturing tolerances and inventory standardization. HSN is optimized for everyday human use: values are rounded to be memorable rather than mathematically exact, and the time variant has no equivalent in the Renard or E series.

The underlying step is 2^(1/3) ≈ 10^(1/10) — roughly 26% between adjacent values. The 1/3-stop ISO film speed sequence (…25, 32, 40, 50, 64, 80, 100…) uses the same step and is a well-known domain-specific instance of the same idea.

## License

CC0 — public domain. No attribution required, though appreciated.
