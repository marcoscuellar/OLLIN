# Ollin

**Human + AI operating systems.** Ollin is the parent brand for a family of Human + AI software products — software that doesn't just store your work, it *moves it forward*.

> *Ollin* — Nahuatl (Mexica) for **movement / momentum**; a day-sign in the Mexica calendar. Pronounced **/ˈol.lin/ — "OHL-leen."**

## This repo

| File | What it is |
|---|---|
| [`index.html`](./index.html) | The parent landing page — a single self-contained HTML file (stacked-reveal scroll, product index, App-Store-style expand cards, color-cycling guide preview). |
| [`vercel.json`](./vercel.json) | Vercel static-hosting config (clean URLs + basic security headers). No build step. |
| [`OLLIN_BRIEF.md`](./OLLIN_BRIEF.md) | Brand & build brief — every decision made so far (positioning, naming, visual identity, palette, page structure, open TODOs). Read it before editing the site. |

## Running it

No build step. Open `index.html` directly in a browser, or serve the folder:

```bash
python3 -m http.server 8000
# then visit http://localhost:8000
```

### Deploying to Vercel

Import the repo in the Vercel dashboard (Framework Preset: **Other**; leave the
build command and output directory empty — it's static HTML). The included
`vercel.json` handles clean URLs and headers; `index.html` is served at `/`.
Every push to the connected branch auto-deploys, and each branch gets its own
preview URL.

### Custom domain (OllinOS.com)

1. In the Vercel project: **Settings → Domains** → add `ollinos.com` **and**
   `www.ollinos.com`. Pick one as primary and let Vercel redirect the other.
2. At the registrar where OllinOS.com is registered, apply the DNS records
   **exactly as Vercel displays them** (its IPs change, so don't hardcode).
   Either point the nameservers to Vercel's (`ns1.vercel-dns.com` /
   `ns2.vercel-dns.com`), or keep your DNS and add the shown A record for the
   apex (`@`) plus a CNAME for `www` → `cname.vercel-dns.com`.
3. Vercel auto-issues SSL once DNS resolves. The "Invalid Configuration"
   warning clears itself when the records propagate.

### Before pointing a live domain at it

- **Set the waitlist endpoint.** Paste a form-service URL (e.g. Formspree)
  into `const NOTIFY_ENDPOINT = ""` near the bottom of `index.html`. While it's
  blank, the "Notify me" form previews the flow but **stores nothing** — real
  signups are dropped. Each submission POSTs `{ email, product, source }`.
- **Fonts are loaded externally** from Google Fonts (Poppins + Inter). Fine as
  is; self-host them if you want zero third-party requests on the primary
  domain.

## The product family

Everything under the parent reads **"Ollin : ___"**.

| Product | One-liner |
|---|---|
| **Ollin : Sales** | The prospecting revenue engine — signal to sent. |
| **Ollin : Vamos** | The tracker — keeps everything moving. |
| **Ollin : Hire** | AI-matched recruiting ("OHMatrix"). |
| **Ollin : MiCasa** | The memory/context layer — the home that holds what's in motion. |
| **Ollin : Constant** | Accountability coach — keeps follow-through on track. |
| **Ollin : TuCasa** | Job board — roles direct to job seekers. |
| **Ollin : Muul** | Content growth — turn what you know into content. |
| **Ollin : Pixchui** | Cybersecurity watcher (monitoring). |
| **Ollin : Nel** | Testing buddy ("Nel" = truth in MX slang). |

## Design principles

- **Monochrome parent, colorful children** — never color the parent chrome; accent color comes from each sub-brand.
- **Respectful homage** — Mexica/Nahuatl heritage carried into the modern AI age. Prefer "Mexica" over "Aztec"; keep every cultural claim accurate. No gold.
- **Type** — Poppins (display/wordmark), Inter (body/UI).
- **The guide** — one gender-neutral AI companion ("Ask your Tío / Tía…") across every product; no cross-tool memory claims.

See [`OLLIN_BRIEF.md`](./OLLIN_BRIEF.md) §7 for open decisions still to be made.

---

© 2026 Ollin Systems · *Ollin* (Nahuatl) — movement
