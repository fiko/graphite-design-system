A square checkbox with a small radius, filled with `primary` when checked.

**You provide:** `<label class="gr-check">` wrapping a native `<input type="checkbox">` and a `<span>` label. Add `gr-check--done` to strike through a completed task.

- Use for selecting rows and for to-do items.
- Keep the native input so keyboard and screen readers work.
- A checkbox without visible text needs an `aria-label`.
- For a single on/off setting that applies immediately, prefer a switch pattern instead.
