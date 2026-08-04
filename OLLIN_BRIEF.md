# Ollin — Brand & Build Brief

*A handoff document. Read this top-to-bottom before touching the site. It captures every decision made so far so you can continue without re-litigating them. Deliverable file: `ollin_final.html` (the parent landing page).*

---

## 1. What Ollin is

**Ollin** is the parent company / holding brand for a family of Human + AI software products. Sole owner: Marcos.

- **Name:** *Ollin* — Nahuatl (Mexica) for **movement / momentum**. It is a day-sign in the Mexica calendar. Pronounced **/ˈol.lin/ — "OHL-leen"** (geminate double-L).
- **Positioning:** *Human + AI operating systems.* Ollin Systems is all-encompassing — the umbrella over many products.
- **Brand story:** *"the old welcomes in the new"* — Mexica/Nahuatl heritage carried into the modern AI age. Naming is **respectful homage** (the founder is Mexican). Always prefer **"Mexica"** over "Aztec" in copy.
- **Tagline / mission (locked copy):**
  > Ollin designs human + AI operating systems — software that doesn't just store your work, it **moves it forward**. Spotting where opportunity is forming, turning that into real conversations, tracking the motion, and keeping people and context in sync — **securely**. **One system, many surfaces, all built to create momentum.**

### Naming rule
Everything under the parent reads **"Ollin : ___"**. Sub-names can be plain function words or coined names (non-Aztec allowed).

---

## 2. The product family

**Ollin : Sales** is a suite (the prospecting revenue engine) with four stages:
`Signal → Intelligence → Vamos (tracker) → Redeploy · Ely`.
*(Open decision — see §7 — whether to keep Sales as one bundled suite or unbundle the stages into standalone products.)*

Standalone products:

| Product | One-liner |
|---|---|
| **Ollin : Sales** | The prospecting revenue engine — signal to sent. |
| **Ollin : Vamos** | The tracker — keeps everything moving. *(was "Movement" → "Aligned" → "Vamos"; "vamos" = let's go)* |
| **Ollin : Hire** ("OHMatrix") | AI-matched recruiting. |
| **Ollin : MiCasa** | The memory/context layer — "your home that holds what's in motion." *(renamed from "COS"/Context OS; paired with TuCasa → mi casa / tu casa)* |
| **Ollin : Constant** | Accountability coach — keeps follow-through on track. |
| **Ollin : TuCasa** | Job board — roles direct to job seekers (Ollin is NOT a middleman on these roles). |
| **Ollin : Muul** | Content growth — turn what you know into content. |
| **Ollin : Pixchui** | Cybersecurity **watcher** (monitoring). |
| **Ollin : Nel** | Testing buddy ("Nel" = truth in MX slang). |

### Full card copy (already in `ollin_final.html`)
Each product's expand card shows: **Thesis · The Problem · Capabilities (3–4) · Who it's for**. Copy was extracted from the user's product designs. Products **with** full copy: Sales, Vamos, MiCasa, Constant, TuCasa, Muul, Pixchui. Products **still needing** full copy: **Hire, Nel** (currently show only the one-liner).

---

## 3. Visual identity

- **Parent is monochrome:** black / white / bone only. **Color comes from each sub-brand** (neutral parent, colorful children). This is the core rule — never color the parent chrome.
- **The mark:** a sun-stone-inspired glyph (two orbital arcs + a core "sun"). It **spins very slowly** (~55s per rotation; auto-pauses on `prefers-reduced-motion`). On hover in the hero it scales up and gets a soft bone glow.
- **Type:** **Poppins** (SemiBold/Bold) for the wordmark + display; **Inter** for body/UI.
- **Core dark palette:** background `#08090D`, panel `#13161E`, bone/cream text `#F2EEE6` / `#D8D2C4`, dim `#6E6B78`.
- **No gold.** The founder dislikes gold — do not reintroduce it.

### The Community Palette (product accent colors)
Colors are drawn from Mexica dyes, stone, and flowers — each with a Nahuatl name + meaning (homage). **The Nahuatl names are a respectful *starting* roster; have a native speaker verify before public launch.**

| Product | Color | Hex | Nahuatl / meaning |
|---|---|---|---|
| Sales | cochineal red | `#C0392B` | *Nocheztli* — "blood of the prickly-pear cactus"; the prized dye, 2nd only to silver as Mexico's export |
| Vamos | coral / salmon-pink | `#FB7185` | *spondylus* (spiny-oyster shell) — prized pink-coral shell |
| Hire | jade | `#3EA672` | *Chalchihuitl* — precious greenstone; life, human worth |
| MiCasa | violet | `#8B6FE0` | *Camohpāltic* — memory, the mind, depth |
| Constant | marigold | `#F0871E` | *Cempōhualxōchitl* — the flower that guides (cempasúchil) |
| TuCasa | **CHANGING** (was Nahua blue `#2E7FD6`) | TBD | user wants a new color — leading option: Emerald "Quetzal" `#17A673` |
| Muul | amaranth | `#D24B8C` | *Huauhtli* — the sacred grain-flower; expression, voice |
| Pixchui | yellow | `#F4C542` | *Cōztic* — the watchfire; alertness (fits "watcher") |
| Nel | turquoise | `#2DD4BF` | *Xihuitl* — most sacred/precious stone (already Nel's established color) |

**Fact-check notes (verified):** cochineal was 2nd (not 1st) to silver; "texohtli" is the Nahua term for the blue also called Maya blue; turquoise = precious/sacred (Nel's "truth" comes from the MX slang, not the stone).

---

## 4. The guide (unifying AI companion)

A single Ollin AI guide lives inside every product — a familiar face across the apps.

- **Color changes per product** to match that product's accent (the neutral-parent / colorful-children rule, made literal).
- **NO GENDER.** The ask-bar placeholder shows **both**: *"Ask your Tío / Tía…"* — the user picks their own. Do not default to one gender or use gendered pronouns.
- **Do NOT claim cross-tool memory/learning.** It is not technically true / is a privacy issue. No "learns in one, remembers in all" copy.
- On the **parent landing page** it appears only as an **inline dialogue box preview** (look-only ask bar) that cycles through the product colors — you don't actually chat with it there. The real conversation happens inside each product.
- Reference design language for the in-product version: the user's `nelask.html` (dark surface gradient, aura glow dark-mode only, pill ask bar with mic + arrow send).

---

## 5. Landing page structure (`ollin_final.html`)

A single self-contained HTML file. Stacked-reveal scroll (each panel is `position: sticky; top:0` and the next slides up to reveal it):

1. **Hero** — just the slow-spinning mark + huge white **ollin**. Nothing else. Hover → bone glow blooms, mark scales.
2. **Meaning** — a reverent dictionary moment: *"In the Nahuatl tongue / ollin / /ˈol.lin/ · "OHL-leen" · Nahuatl / noun. movement; momentum. the Mexica day-sign for motion."* Understated, small.
3. **Why Ollin** — the mission copy (§1), lines stagger in editorially (blur + rise).
4. **Everything, one place** — the numbered product index. Each row:
   - hovers → text turns the product's color + a soft **glow in that color blooms behind the row**;
   - clicks → **App Store-style expand** (the card grows from the row's position into a centered, scrollable detail card showing Thesis/Problem/Capabilities/Who, in the product's color), with a "Visit →" button. ✕ / click-away / Esc shrinks it back.
5. **Your guide** — "One companion. Every surface." + the color-cycling inline dialogue box (§4).
6. Footer credits: `© 2026 Ollin Systems · Ollin (Nahuatl) — movement`.

Motion references the user loves: **Linear** (centered, calm, glow), and **motion.dev** examples (text-reveal, footer-reveal, editorial-stagger hero, App-Store card expand).

**Founder name is intentionally OFF the site** — Ollin stands on its own; a founder credit can be added later, quietly, in the footer only.

---

## 6. Domains

Owned: **OllinOS.com**, **ollin.space**, **ollin.app**.
Proposed (not final): ollin.space = parent brand/hub · ollin.app = the individual apps (subdomains like `sales.ollin.app`, since each product is its own standalone app — no central login) · OllinOS.com = canonical .com + email + reinforces the "operating systems" positioning.

---

## 7. Open decisions / TODO

- **TuCasa color** — pick the replacement (leading: Emerald/Quetzal `#17A673`).
- **Sales bundle vs unbundle** — keep Sales as one suite, or split Signal / Intelligence / Vamos / Ely into standalone cards? (User leaned toward separating; needs ~2–3 new community colors if so.)
- **Vámonos** — a travel-companion product appeared in the designs but isn't in the family yet. Decide whether to add it. **Watch the near-collision with "Vamos" (the tracker).**
- **"Coach Bob"** — the Constant design's CTA said "Explore Coach Bob." Confirm whether the coach's persona is named Bob or that was a placeholder.
- **Hire & Nel** — still need full card copy (thesis/problem/capabilities/who).
- **Nahuatl name review** — verify the whole community-palette roster with a native speaker before launch.
- **Assets** — export real logo files (SVG/PNG) + favicon; wire the "Visit →" buttons to each product's destination.
- **Mobile** — stress-test the expand card on short viewports / with keyboard open.

---

## 8. Voice & guardrails

- Warm, confident, understated. Restraint is the brand — the reverence for the Nahuatl root reads *because* it's quiet.
- Homage must stay **accurate** (fact-check any cultural claim) and **respectful** (never costume/decoration).
- Product copy may reference ADHD / neurodivergence as target audiences (that's the user's product positioning) — but never store personal health data about the user.
- Keep the parent monochrome; keep gold out; keep the guide gender-neutral and honest about what it can do.
