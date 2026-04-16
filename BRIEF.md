# Prime Produce, Inc. — Design Brief

## Brand Synopsis

Prime Produce, Inc. is a privately held Dallas produce brokerage incorporated August 19, 1999 by Rick Harkinson (President/Owner) and Marc J. Nelson (Partner). The company trades **deciduous fruits, melons, stone fruits, and bell peppers** across the United States and Mexico, operating out of 9550 Forest Lane, Suite 510, Dallas, TX 75243. They hold **PACA license #20000096** and are listed in the USDA AMS National Shippers Contact List (ID 21200GJ5H).

Twenty-six years in, the business is quiet by design — two principals on one phone line, repeat counterparties, no storefront, no marketing layer. The Blue Book Services 2016 "Hat's Off To Dallas" market feature is the company's most significant third-party validation.

**The gap we're filling:** They have no website, no digital presence, no claimed social. This mockup is the first canonical web version of the brand — designed to speak credibly to three audiences simultaneously: customer accounts (wholesale buyers), growers/shippers (domestic + Mexico), and transporters (reefer carriers).

---

## Design Decisions

### Direction A — The Ledger
- **Mood:** Editorial, heritage-driven. A 26-year trade publication finally has a website.
- **Fonts:** Fraunces (display serif, variable) + Source Serif 4 (body) + JetBrains Mono (data/tabular)
- **Colors:** `#F1EDE4` cream paper · `#1E4A2D` forest green (ink) · `#C64034` apple red (accent) · `#2A2A28` warm black
- **Layout:** Magazine grid, asymmetric, generous whitespace, numbered sections (§ 01–§ 07), ruled hairlines, drop caps, double-rule dividers, a ledger-style credentials strip in the masthead (`Vol. XXVI · Est. 1999 · Dallas, TX · PACA No. 20000096 · USDA AMS 21200GJ5H`)
- **Signature element:** The commodity list rendered as a ledger — large serif commodity name, dotted leader line, monospace category label right-aligned. Looks like an entry in an old trade almanac.
- **Trends used:** Experimental editorial typography, heritage-meets-modern type pairing, kinetic serif/italic contrast, tabular data as design.

### Direction B — The Packing House
- **Mood:** Confident, contemporary, warm. Small broker that shows up like a major operation, without theatre.
- **Fonts:** Instrument Serif (display, high-contrast editorial) + Manrope (body geometric sans) + JetBrains Mono (data)
- **Colors:** `#1E4A2D` forest green (dominant, hero + sections) · `#F1EDE4` cream (text on green, content bg) · `#C64034` apple red (accent) · `#E8DDC7` warm beige (tertiary)
- **Layout:** Full-bleed hero image with gradient overlay, alternating green/cream/beige bands, bento-style audience cards ("Three doors. Same handshake."), pill-style commodity chip shelf, sticky-column "Desk" section with oversize pull quote.
- **Signature element:** A horizontal commodity marquee in the hero-adjacent band — the 11 commodities scroll endlessly in large italic serif against the deep green field, broken by apple-red bullets. Reads like an old produce-terminal availability board.
- **Trends used:** Full-bleed kinetic hero + overlay type, bento audience cards, horizontal marquee ticker, color-field sectioning, mixed-script typography (serif display + geometric sans).

---

## Content Inventory

### Images used (all local in `images/`)
- **`hero.jpg`** — Real photograph: fruit spread (cantaloupe, honeydew, apples, grapes, stone fruit, cherries, kiwi, apricots, orange) on wood table with Dallas skyline including Reunion Tower. Source: provided by Zack. Quality: excellent.
- **`logo.png`** — Prime Produce, Inc. wordmark with red apple + green leaf icon, forest-green serif type, transparent background. Source: provided by Zack. Quality: excellent.
- **`blue-book.png`** — Blue Book Services "bluebook / Since 1901" horizontal logo, 1760×484, transparent. Source: scraped from bluebookservices.com.

### Key copy / content
- **Tagline (approved via Zack's calendar):** *Fresh. Reliable. On spec, on time since 1999.*
- **Company identity data:** Est. 1999 · PACA 20000096 · USDA AMS 21200GJ5H · SIC 5148 · TX SOS 0154720800 · PMG Co. ID 176366
- **Commodity list (11):** Apples, Grapes, Pears, Cantaloupe, Honeydew, Apricots, Cherries, Nectarines, Peaches, Plums, Bell Peppers
- **Marc Nelson quote** (pull-quote, both directions): *"Supply from Mexico, the East Coast, and Chile continues to move — weather patterns shift, but the obligation to deliver on spec does not."* — Blue Book Services, "Hat's Off To Dallas," 2016
- **Principals:** Rick Harkinson (President & Owner, since 1999) + Marc J. Nelson (Partner, since 1999)
- **Contact:** (214) 221-4554 · Fax 214-221-1886 · primeproduce@hotmail.com · 9550 Forest Lane, Suite 510, Dallas, TX 75243

### Links preserved
- `tel:+12142214554` — clickable phone (primary conversion)
- `mailto:primeproduce@hotmail.com` — clickable email
- Sectional anchors: #top, #trade / #desk, #commodities, #serve / #who, #principals, #contact, #credentials

---

## Image Generation Prompts

**None used.** Zack elected to skip generated product imagery — B2B broker credibility requires authenticity, and AI-generated produce photography would erode trust. No auto-generation was performed during this build.

If Rick ever wants to add generated atmosphere for a future expansion (e.g., an "Our Process" page or a DFW logistics section), prompts would go here. For now: all imagery on the site is real and already in the `images/` folder.

---

## Suggested Next Mockups

Ordered by highest value to Rick's business:

1. **Principals page** — full-length professional bios for Rick and Marc with photography, career histories, industry experience, and the Blue Book 2016 feature excerpt. Biggest credibility lift.
2. **Mexico & Import Sourcing page** — if Prime Mexican Produce, Inc. is an active sister entity, this is a differentiator. Map of sourcing regions, seasonality calendar, PACA cross-border framing.
3. **Harvest Calendar / Seasonal Availability** — interactive 12-month grid showing which commodities are available from which sourcing regions and months. High utility for buyers.
4. **Careers / Working with Prime** — short page for would-be carriers, growers, and operators describing the three "doors" (buyer / grower / transporter) in more operational detail.
5. **Blue Book 2016 feature reprint** — a dedicated press page archiving the full Blue Book article with period context. Single best standalone credibility asset.

---

## Production Notes

To ship this as a live client site (not a mockup), a Claude Code Opus high-effort session would:

1. Port whichever direction Rick picks to a CMS or static generator (Astro + Markdown, or simple static Vite build) so copy is editable without developer help.
2. Add a proper `primeproduce.com` DNS + SSL setup (Bloomberg already associates the domain with them — Rick needs to confirm he owns it).
3. Replace the Hotmail address with a professional `@primeproduce.com` mailbox (Google Workspace or similar — ~$6/mo per user).
4. Add a lightweight contact form (Formspree, Netlify Forms) alongside the phone CTA for after-hours lead capture.
5. Set up Google Business Profile + consistent NAP (Name/Address/Phone) across D&B, Manta, Yelp, Google so search surfaces the new site authoritatively.
6. Add JSON-LD schema for LocalBusiness + Organization to help Google surface hours, address, and the 26-year tenure in rich results.
7. Bring Blue Book feature, PACA verification, and any additional credentials into a structured "Credentials" page with linked sources — this is how B2B trust scales online.

---

## Build Timing
| Phase | Duration |
|---|---|
| Step 1: READ (research ingestion + synthesis) | ~2m |
| Step 2: DIRECTION (two creative briefs) | ~2m |
| Step 3: BUILD (two mockups + selector) | ~12m |
| Step 4: VERIFY (rendering + ACCURACY.md) | ~3m |
| Step 5: BRIEF (this file) | ~2m |
| Step 6: PUBLISH (GitHub + Pages) | TBD |
| Step 7: DELIVER | TBD |
| **Total: Prompt to Live Link** | **TBD** |

*No image generation time — zero AI imagery used this build.*
