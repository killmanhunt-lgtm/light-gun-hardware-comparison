# Sources and provenance

## What this repository actually is

This is a **republished, structured copy** of the comparison tables published on `lightgungame.com`. The `checked` dates and the named sellers are as recorded on those pages. I have **not** independently re-read every seller page to re-verify each figure — where a figure is carried over, it is marked as such below.

That distinction matters, so it is stated here rather than buried.

## Per-file provenance

### `data/light-gun-hardware-comparison.csv`

Carried over from the comparison table on `lightgungame.com/light-gun-for-pc/`, which dates its figures **2026-10-13** and names these sources:

| Row | Figure type | Source as recorded on the page |
|---|---|---|
| Sinden Light Gun | price | Sinden's own shop, in SGD |
| Sinden Light Gun | tracking rate, latency | maker's documentation; early hands-on write-ups |
| Gun4IR | price | maker's own price list, in EUR |
| Gun4IR | latency, tracking rate | maker's claim (2–7 ms); one independent polling test (145 Hz = 6.89 ms) |
| Retro Shooter RS3 Reaper | price | `retroshooter.com/shop`, read 2026-10-13, USD |
| Retro Shooter RS3 Reaper | tracking rate | the same independent polling test (860 Hz peak = 1.1 ms) |
| AimTrak | price | `ultimarc.com`, read 2026-10-13, USD |
| AimTrak | tracking rate, latency | not published by the maker |

**The `latency_figure` column mixes two different kinds of number.** A maker's claim and an independent measurement are not the same thing, and in several cases they count different parts of the chain (camera-to-cursor versus processing only). Do not sort this column and treat the result as a ranking.

### `data/arcade-machine-comparison.csv`

Carried over from the table on `lightgungame.com/light-gun-arcade-machine/`, which dates its figures **2026-10-14** and reads each figure from the **seller's own product page**, not from a shopping-results block. Where the two disagreed, the seller's own page was used.

| Row | Source as recorded on the page |
|---|---|
| Dreamcade Vision 29 | `dreamarcades.com/vision29.php` |
| Full Size 2 Player Shooter Arcade Cabinet – Adventure Series | `gameroomsolutions.com` product page |
| HighPeak Retro Arcade Shooter | `highpeakco.com` product page |
| Dual Light Gun Upright Arcade (trackball, 32 in) | `ebay.com` listing |
| Upgrade Arcade Shooter Cabinet | `upgradearcade.com` product page |

Two of the five machines were shown at a **lower** price in a shopping-results block than on the seller's own page (HighPeak: $295.62 vs $450.00; Upgrade Arcade: $1,800.00 vs $2,000.00). This dataset uses the seller's own page in both cases.

### `data/sinden-price-list.csv`

Carried over from the price table on `lightgungame.com/sinden-light-gun-setup/`. Prices are in **SGD**, as listed by the Sinden shop, dated 2026-10-13.

## Known gaps

- Cabinet **weight, dimensions, power draw and warranty** are mostly not published by the sellers, so they are absent rather than estimated.
- **No independent head-to-head latency test** exists across all four gun families. Every "faster than" claim in circulation rests on figures that count different things.
- **Recoil** is not comparable across vendors: one is a solenoid slide, one a rumble motor, one a spring.
- Exchange-rate conversions are **not applied**. Each price stays in the currency its own shop lists, so a USD figure and an SGD figure are not directly comparable as numbers.

## Corrections

If a figure is wrong or out of date, open an issue with the shop URL and the date you read it. A dated screenshot is enough.
