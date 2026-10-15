# Light gun hardware comparison data

Dated, sourced comparison data for modern light gun hardware — the guns that work on a flat-panel TV, a projector or a PC, and the ready-made arcade cabinets that ship with guns already in them.

Every price carries the date it was read and the shop it was read from. Where a manufacturer's claim and an independent measurement disagree, both numbers are kept instead of one being picked.

## What is in here

| File | What it is |
|---|---|
| `data/light-gun-hardware-comparison.csv` | One row per gun: tracking method, tracking rate, latency figure, price, what you have to add, and the worst known limitation |
| `data/arcade-machine-comparison.csv` | One row per ready-made light gun arcade cabinet or kit: screen, gun included, games, whether it runs a PC or a TV, listed price, known limitation |
| `data/sinden-price-list.csv` | The Sinden shop's own price list, item by item |
| `data/sources.md` | Where each class of figure came from, and what is a maker claim versus an independent measurement |

## Conventions

- `checked` is the date the figure was read from the source, **not** the date the source was published.
- Prices are kept in the currency the shop itself lists. SGD, EUR and USD are labelled so they are not compared as if they were the same money.
- Latency figures are a mix of manufacturer claims and independent polling tests. The `latency_figure` column says which is which. **They do not measure the same thing** and should not be ranked against each other.
- A blank cell means the source did not publish that figure. It does not mean zero.

## Read this before you use the numbers

- Latency has not been measured head-to-head by an independent party across all four gun families. Any "X is faster than Y" claim rests on figures that count different parts of the chain.
- Recoil is not comparable across vendors — one is a solenoid slide, another a rumble motor, another a spring.
- Cabinet specifications that buyers care about most (weight, power draw, warranty) are largely not published by the sellers, so they are absent here rather than guessed.

## Provenance

Per-row provenance is in `data/sources.md`. The narrative version of this data — with the places where the sources contradict each other written out — is at <https://lightgungame.com/light-gun-for-pc/>.

## Contributing

Corrections are welcome, especially with a link to the page you read and the date. If a price has changed, a dated screenshot or the shop URL is enough.

## License

Data: CC BY 4.0 — see `LICENSE`.
