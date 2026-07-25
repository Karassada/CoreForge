# OSBS — ミセログ（仮称）Landing Page

Product landing page for **SHIFT GK's** data-collection automation service for
Japanese small hospitality businesses (restaurants, cafes, bars, izakaya, clubs):
staff send their usual end-of-day sales report to LINE → AI reads it → sheets,
phone dashboard, searchable history and LINE confirmations update within the minute.
Sold as setup + monthly operation.

- **`index.html`** — the whole page in one file. All CSS, JS and SVG are inline; the
  only external request is the Google Fonts stylesheet (Zen Old Mincho / Zen Kaku
  Gothic New). Offline it falls back to Hiragino / Yu Mincho and still renders
  completely, so it stays safe to open in a client meeting with no wifi.
- Reveal animations are progressive enhancement: the page is fully visible without
  JavaScript. `?static` disables reveal gating (print / capture / old tablets);
  `?only=<section-id>` renders a single section.
- Product name is a working title (ミセログ / MISELOG, 仮称) pending final naming.

**Open before launch:** the contact route is still a placeholder (`お問い合わせ：準備中`)
and the booking CTA has nowhere to go. It needs a real destination — a booking link,
a form, or a LINE公式アカウント — before this is sent to leads.

Internal strategy, spec, and pricing rationale live in the private CLAUDE HUB and are
intentionally **not** part of this repo.
