A compact row for lists and tables, inside a rounded list container.

**You provide:** a `<div class="gr-list">` with an optional `gr-list__head`, then `gr-row` children. Each row can hold a checkbox, a `gr-avatar`, `gr-row__name`, `gr-row__title`, `gr-row__preview`, a tag and `gr-row__date`. Add `gr-row--unread` to emphasise new items.

- Unread rows use `ink` at weight 600 and coloured tags; read rows use `ink-muted` and neutral tags.
- The preview truncates with an ellipsis; never wrap rows to two lines.
- Rows are divided by `border` hairlines and step to `surface-sunken` on hover.
- Below 640px, hide `gr-row__preview` and the tag.
