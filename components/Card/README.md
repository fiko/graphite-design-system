A rounded surface panel that groups related content.

**You provide:** a `<section class="gr-card">` with an optional `gr-card__head` (title plus a small icon button), any content, and an optional `gr-card__foot`. Nest `gr-card gr-card--inner` for items inside a card. `gr-progress` is a pill progress bar for use inside cards.

- Cards sit on `canvas` with `radius-lg`; inner cards use `surface-sunken` with `radius-md`.
- Never nest more than one level.
- Use `gr-card__kicker`, `gr-card__value` and `gr-card__text` for a stat or event.
- Padding is always `space-4` (outer) or `space-3` (inner).
