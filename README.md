Graphite is a calm, neutral interface language: a soft grey canvas, white rounded panels, near-black ink and pill-shaped controls, with one plum accent used sparingly. Use it for any product where content, not chrome, should lead.

## Principles

- **Tone before lines.** Separate areas by stepping `canvas` → `surface` → `surface-sunken`. Reach for `border` only for row dividers; reach for shadows only when something floats.
- **Black is the brand.** The primary action is a `primary` pill with `on-primary` text. Use one per view.
- **Colour is information.** `accent` and the tag colours mark categories and the few things that matter. If everything is coloured, nothing is.
- **Round and soft.** Controls are pills (`radius-full`); containers step up from `radius-md` to `radius-xl` as they get larger. Never mix square corners in.
- **Dense but quiet.** Small type, generous radii, even rhythm. Rows are compact; panels breathe.

## Colour

- Page background is `canvas`. Content sits on `surface` panels. Nested cards, hover rows and neutral tags use `surface-sunken`.
- Text is `ink` (primary), `ink-muted` (secondary) and `ink-subtle` (dates, counts). All three pass 4.5:1 on `canvas`, `surface` and `surface-sunken` in both themes.
- `ink-faint` fails contrast on purpose. Use it only for placeholder icons, disabled states and decoration.
- Use `border` for decorative hairlines and `border-strong` for outlines that carry meaning (checkboxes, inputs).
- `accent` is the only brand hue. Use it for links, one highlighted tag and key data. Put `on-accent` on accent fills; pair `accent` text with `accent-soft` grounds.
- Category tags pair `tag-*-bg` with the matching `tag-*-ink`. Neutral tags use `surface-sunken` with `ink-muted`.
- Status colours come in four muted families, mixed to sit beside the plum accent rather than shout: `info` (slate blue), `success` (lagoon, a teal green), `warning` (honey yellow) and `danger` (clay red). Never swap in brighter, saturated versions. Each has a solid colour, an `on-*` colour for text on that fill, and a `*-soft` tinted ground.
- For alerts and status tags, put `info`, `success` or `danger` text on its `*-soft` ground. `warning` is a fill only; for warning text use `warning-ink`.
- Status colours always appear with a word or icon, never as colour alone. They do not replace `primary`: the main action stays black.
- Both themes are complete. Switch with `data-theme="light"` or `data-theme="dark"` on the root; never hard-code a hex value.

## Typography

- One family: Geist (`--font-sans`), loaded from Google Fonts in weights 400, 500 and 600. Geist Mono (`--font-mono`) for code and IDs.
- Default text is `body` (14/20). Use `body-strong` for emphasis and button labels, `caption` for metadata, `label` for tags.
- Headers inside panels use `subheading`; sections use `heading`; pages use `title`. Reserve `display` for one hero line per page.
- Emphasise with weight (500, 600), never with colour or italics. Never go above 600.
- Sentence case everywhere, including buttons and headings. No all-caps.

## Spacing and layout

- Everything sits on a 4px grid: `space-1` to `space-12`.
- Panels pad `space-4`; rows pad `space-3` block and `space-4` inline; panels sit `space-2` to `space-5` apart on the canvas.
- Typical app layout: a 240px sidebar directly on `canvas`, a fluid main column of `surface` panels, and an optional 280px to 320px side rail of cards.
- Wrap a full app in a shell with `radius-xl` when it floats on a backdrop.

## Shape and elevation

- `radius-full`: buttons, inputs, icon buttons, avatars. `radius-sm`: checkboxes and tags. `radius-md`: nav items and nested cards. `radius-lg`: panels. `radius-xl`: shell and dialogs.
- A nested element always has a smaller radius than its container.
- Resting panels take `shadow-sm` or none. Popovers take `shadow-md`, dialogs `shadow-lg`. Never stack shadows.

## States

- Hover: step the ground one tone (`surface` → `surface-sunken`); primary buttons drop to 88% opacity.
- Selected: nav items become `surface` with `shadow-sm` and `ink` text; checked controls fill with `primary`.
- Focus: a 2px solid `focus` ring with 2px offset on every interactive element.
- Disabled: 45% opacity, no pointer events.
- Motion is brief and functional: 120ms to 160ms ease-out on colour and opacity only.

## Iconography

- Use the Graphite icon set in the Icons asset group: 71 outline icons on a 24px grid with a 1.5px stroke and round caps. Never mix in another icon library.
- Inline the SVG with `stroke="currentColor"` and class `gr-icon` so it takes `ink` or `ink-muted` from its parent; `assets/Icons/icons.json` holds the inline markup for every icon.
- Size icons at 16px in nav items, rows and buttons, and 20px (`gr-icon--lg`) in icon buttons and toolbars.
- Never use emoji as icons. `star-filled` is the only filled icon, for the starred state.
- If an icon is missing, draw it on the same grid and stroke rather than borrowing one.

## Voice

- Short, plain and specific. Labels are verbs or nouns: "New email", "Upgrade plan", "View all 35 tasks".
- Speak to the person as "you". No exclamation marks, no jargon.
- Numbers are exact and compact: "1 of 4", "12 May, 13:50", "16.7 GB".

## Using the components

- Load `components/bundle.css` after the tokens; every class is prefixed `gr-` and reads only tokens.
- The components are plain HTML and CSS, so they work in Laravel Blade, Liquid, Next.js or any other stack. Copy the markup from each component's preview.


---

## Consuming this system (generated — do not edit)

Every path named below is under `project/` in this design system: read `project/api/tokens.md`, not `api/tokens.md`.

8 components are documented without a runnable `components/bundle.js`: read each component’s card, and its README where it has one (`components/<Comp>/README.md`), and build to those guidelines. Tokens: the values are on `api/tokens.md`; a Slides deck or Design canvas also takes `tokens.json` by file path. On a Design canvas, also copy `tokens.css` to `project/ds/<folder>/tokens.css` in the call that installs this system, and link it in each artboard that uses this system, right after the `support.js` line and before the system’s other stylesheets: `<link rel="stylesheet" href="ds/<folder>/tokens.css">` (with one `../` in front for each folder the artboard is in).

**Read, per thing:** a component’s props, parts and examples: `api/components/<Comp>.md`; token values: `api/tokens.md`; stored assets and their paths: `api/assets/<Group>.md`. After this README, fetch the cards and fonts you need in ONE message as parallel calls — none depends on another.

**Two rules.** Before you use a thing — a component, a token group, an icon, an asset — read its card from the index below; a value you did not read from a card is a guess. `tokens.json`, `manifest.json` and `design-system.json` are sources for tools: hand them over. `components/<Comp>/README.md` and `assets/<Group>/README.md` are the long-form second read a card links to; `SKILL.md` and `artifact-type/` beside them are authoring guidance, not needed to consume the system.

## Index (generated — do not edit)

**Tokens**

- `api/tokens.md` — Every token: surface, text, fill, border, palette, type, spacing, radius, shadow. (13.0k)

**Icons and assets**

- `api/assets/Icons.md` — 70 files, by asset id. (7.2k)

**Components** (`api/components/<Comp>.md`, 8)

- **Feedback**: `Alert` — An inline status message in one of four tones, with matching badges and tags
- **Actions**: `Button` — The pill-shaped action control, in four variants and two sizes
- **Data display**: `Card` — A rounded surface panel that groups related content · `ListRow` — A compact row for lists and tables, inside a rounded list container · `Tag` — A small label that categorises an item
- **Forms**: `Checkbox` — A square checkbox with a small radius, filled with primary when checked · `Input` — A pill-shaped text field, with an optional leading icon, label and hint
- **Navigation**: `NavItem` — A sidebar navigation row with icon, label and optional count
