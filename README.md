# CoreBuild — Website

**Organize. Automate. Save Time.**

The official website for **CoreBuild**, a business-infrastructure service from **SHIFT合同会社**
for Japanese small and medium-sized companies. CoreBuild organizes how a company works,
automates repetitive work, and gives owners a clear view of the business — accounts and
domain, folder structure, spreadsheets, website, dashboards, workflow automations, and
AI connected to all of it. Sold as a build plus an ongoing monthly plan.

- **`index.html`** — the whole page in one file. All CSS, JS and SVG are inline; the only
  external request is the Google Fonts stylesheet (Zen Old Mincho / Zen Kaku Gothic New).
  Offline it falls back to Hiragino / Yu Mincho and still renders completely, so it stays
  safe to open in a client meeting with no wifi.
- **Bilingual.** Japanese by default with an English toggle; both languages ship in the
  HTML, so there is no translation request at runtime.
- **Japanese line breaking** is handled at runtime with `Intl.Segmenter`, so Japanese text
  wraps at word and phrase boundaries instead of mid-word.
- Reveal animations are progressive enhancement: the page is fully visible without
  JavaScript. `?static` disables reveal gating (print / capture / old tablets);
  `?only=<section-id>` renders a single section.
- **`og.png`** — the 1200×630 social share card, generated from HTML rather than hand-drawn.

**Open before launch:** the contact route is still a placeholder (`お問い合わせ：準備中`)
and the CTAs have nowhere to go. It needs a real destination — an address, a form, or a
LINE公式アカウント — before this is sent to leads.

Internal strategy, specifications and pricing rationale live in the private CLAUDE HUB and
are intentionally **not** part of this repo. The `.gitignore` here excludes `*.md` by
default (`!README.md` is the sole exception) so internal notes cannot be committed by
accident — do not weaken that rule.
