A sidebar navigation row with icon, label and optional count.

**You provide:** an `<a class="gr-nav-item">` with a 16px icon, a label, and an optional `<span class="gr-nav-item__count">`. Group items in `<nav class="gr-nav">` with an optional `gr-nav__title`. Mark the current page with `aria-current="page"`.

- Place the sidebar directly on `canvas`; the selected item lifts to `surface` with `shadow-sm`.
- Exactly one item is current at a time.
- Counts are plain numbers in `ink-subtle`, right aligned. Do not use badges.
- Separate groups by `space-6`.
