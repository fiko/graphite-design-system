An inline status message in one of four tones, with matching badges and tags.

**You provide:** a `<div class="gr-alert">` with one tone (`gr-alert--info`, `--success`, `--warning`, `--danger`), a `gr-alert__dot`, and text that starts with a `<strong>` word naming the status. Use `role="alert"` for errors and `role="status"` otherwise.

- The alert sits on the tone's `*-soft` ground; the leading word carries the tone colour, the message stays `ink`.
- Always start with the status word ("Error:", "Warning:") so meaning never depends on colour.
- `gr-badge--*` is a solid pill for a status that must stand out; `gr-tag--*` is the quiet version for tables and lists.
- One alert per context. Do not stack more than two.
