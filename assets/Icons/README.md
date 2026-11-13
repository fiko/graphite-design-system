Graphite icons: 71 outline icons drawn for the email product, on a 24px grid with a 1.5px stroke, round caps and round joins.

- **Ink:** the SVG files are single-ink, stroked in `ink` (`#070606`). An `<img>` cannot inherit colour, so for themed UI paste the icon inline with `stroke="currentColor"` and let it take `ink` or `ink-muted` from its parent.
- **Inline source:** `icons.json` maps each icon name to its inner SVG markup, already using `currentColor`. Wrap it in `<svg class="gr-icon" viewBox="0 0 24 24">…</svg>`.
- **Sizes:** 16px in nav items, rows and buttons (`gr-icon`), 20px in icon buttons and toolbars (`gr-icon gr-icon--lg`), 24px for empty states. Never scale below 16px.
- **Mailbox:** inbox, star, star-filled, clock (snoozed), send, send-later, draft, archive, trash, spam, block.
- **Folders and labels:** folder, file, file-text, files, news, flag, briefcase, tag, cloud.
- **Message actions:** compose, pencil, reply, reply-all, forward, paperclip, mail, mail-open, mail-unread, download, upload, link, image, copy, printer.
- **Toolbar and navigation:** search, sliders, filter, pin, calendar, refresh, settings, plus, more, more-vertical, menu, chevrons, check, x, arrow-up-right, checklist, grid.
- **Account and security:** user, users, at, globe, bell, lock, key, shield, eye, eye-off, sun, moon, logout, help, info, sparkle (upgrade).
- `star-filled` is the only filled icon; use it for the starred state only. Icon-only buttons always carry an `aria-label`.
