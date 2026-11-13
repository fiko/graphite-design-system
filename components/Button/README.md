The pill-shaped action control, in four variants and two sizes.

**You provide:** a `<button>` or `<a>` with class `gr-btn` plus one variant (`gr-btn--primary`, `--secondary`, `--ghost`, `--danger`), an optional size (`gr-btn--sm`), and a label. Icon-only buttons add `gr-btn--icon` and need an `aria-label`. Add `gr-btn--block` for full width.

- Use one `primary` button per view; everything else is `secondary` or `ghost`.
- Labels are sentence case and start with a verb: "New email", "Upgrade plan".
- Icons are 16px, before the label, coloured by `currentColor`.
- Use `danger` only for destructive actions, and always with a label that names the action.
- Do not change the radius; buttons are always `radius-full`.
