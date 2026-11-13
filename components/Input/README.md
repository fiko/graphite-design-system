A pill-shaped text field, with an optional leading icon, label and hint.

**You provide:** a `<label class="gr-input">` wrapping an `<input>` and an optional 16px icon. For a labelled field, wrap it in `gr-field` with `gr-field__label` and `gr-field__hint`.

- Default inputs take a `border-strong` outline so they read on any surface.
- Use `gr-input--quiet` (no outline, `shadow-sm`) only for search on `canvas`.
- Mark errors with `gr-input--error`, `aria-invalid="true"` and a hint in `gr-field__hint--error` that starts with the word "Error".
- Placeholders are examples, not labels. Every input needs a visible label or an `aria-label`.
