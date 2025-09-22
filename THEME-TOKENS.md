# Theme‑Tokens & Variablen

## Farben (ausgehend von `$primary: #024878`)
- `$primary-100 … $primary-900` – Tints/Shades per `mix(white|black, $primary, x%)`
- Akzente: `$accent #34c759`, `$warning #ff9f0a`, `$danger #ff3b30`, `$info #0a84ff`

## Typografie
- `$font-family-sans-serif` – System‑Stack (SF Pro, -apple-system, usw.)
- `$headings-font-weight`, `$font-weight-*`

## Radii & Schatten
- `$border-radius*`, `$card-border-radius`, `$btn-border-radius*`, `$input-border-radius`, `$modal-content-border-radius`
- `$box-shadow*` (sm, md, lg)

## Fokus & Glas
- `$focus-ring-color`, `$focus-ring`
- Glas‑Fallbacks: `$glass-bg`, `$glass-border`, `$glass-shadow`
- Mixins: `@mixin focus-ring`, `@mixin glassy($bg, $blur)`, `@mixin ios-pressable`

## CSS‑Variablen (im POST definiert)
- `--brand`, `--brand-100 … 700`  
- `--glass-*`, `--surface`, `--surface-soft`, `--text`, `--muted`

## Hilfsklasse
- `.glass` – sofort einsetzbarer Glascontainer mit Radius & Schatten
