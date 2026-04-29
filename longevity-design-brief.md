# California Center of Longevity Medicine — Homepage Redesign Brief

A first-pass concept for a modern, premium-but-warm homepage in the spirit of Next Health and Parsley Health.

---

## 1. Page Structure

A single, scannable narrative — top to bottom:

1. **Navigation** — sticky, translucent, minimal
2. **Hero** — left-aligned headline + image right
3. **Trust strip** — four short credibility points
4. **Services** — three clean cards
5. **Founder credibility** — Dr. Kurtz section
6. **Patient journey** — three-step process
7. **Final CTA** — closing consultation invite
8. **Footer** — minimal, just enough

---

## 2. Suggested Copy

### Navigation
- **Logo:** California Center of Longevity Medicine
- **Links:** About · Services · Longevity · Functional Medicine · Contact
- **CTA:** Book Consultation

### Hero
- **Eyebrow:** WOODLAND HILLS · LOS ANGELES
- **Headline:** Live Longer. Live Better.
- **Subhead:** A personalized approach to longevity and functional medicine — designed around your biology, your goals, and your life.
- **CTA:** Book a Consultation

*Alternate headlines if you want a softer or more medical tone:*
- "A more personal approach to longevity medicine."
- "Longevity care designed around the whole person."
- "Personalized medicine for a longer, healthier life."

### Trust Strip
- Board-Certified Physicians
- Functional & Longevity Medicine
- Evidence-Based Protocols
- Personalized Care

### Services
- **Eyebrow:** WHAT WE DO
- **Headline:** Modern medicine, built around the individual.
- **Subhead:** Three integrated areas of care — informed by advanced diagnostics and decades of clinical experience.

| Service | Copy |
|---|---|
| Longevity Medicine | Extend your healthspan with proactive, science-based care that addresses aging at its biological roots. |
| Hormone Optimization | Restore balance and vitality through precise, individualized hormone therapy guided by advanced diagnostics. |
| Functional Medicine | Identify and resolve the root causes of chronic symptoms with comprehensive testing and integrative treatment. |

### Dr. Kurtz Section
- **Eyebrow:** MEET YOUR PHYSICIAN
- **Name:** Dr. Allan Kurtz, M.D.
- **Title:** Founder & Medical Director
- **Bio (paragraph 1):** Dr. Kurtz brings more than three decades of clinical practice to the California Center of Longevity Medicine. Board-certified and trained in both conventional and functional approaches, he has built his practice around one principle: care should be precise, evidence-based, and built around the individual.
- **Bio (paragraph 2):** His patients come to him for a level of attention rarely found in modern medicine — physician-led care that listens carefully, investigates thoroughly, and treats the whole person.
- **Pull quote:** "Real longevity care begins with truly knowing the patient."
- **Credential chips:** Board Certified · 30+ Years Practicing · Functional & Longevity Trained

### Patient Journey
- **Eyebrow:** THE PATIENT EXPERIENCE
- **Headline:** A clear path to better health.
- **Subhead:** Every patient relationship begins the same way — with time, listening, and a complete picture of your health.

| Step | Copy |
|---|---|
| 01 — Comprehensive Consultation | We begin with an in-depth conversation about your history, goals, and concerns — the foundation of effective care. |
| 02 — Advanced Testing | Comprehensive lab and biomarker analysis reveals the underlying drivers of your health and aging. |
| 03 — Personalized Care Plan | Your physician designs a clear, evidence-based plan tailored to your biology and lifestyle. |

### Final CTA
- **Headline:** Begin your longevity journey.
- **Subhead:** Schedule a private consultation with Dr. Kurtz and our care team to see what personalized medicine can do for you.
- **Button:** Request a Consultation

---

## 3. Visual Layout Notes

- **Container width:** 1240px max, 32px gutters, generous vertical rhythm (130px between major sections on desktop).
- **Hero:** asymmetric two-column grid (1.1fr / 1fr). Headline reads big and quiet; image sits beside it as an editorial counterweight, not a backdrop. No overlay text on imagery.
- **Trust strip:** thin band, top + bottom hairline border, four equal columns. Small diamond glyph above each label so it reads as branded, not bullet-point list.
- **Services:** three equal cards with hairline borders that lift on hover (subtle shadow + accent border). Numbered eyebrow ("01 — LONGEVITY") to give the grid a magazine quality. Each card ends with a "Learn more →" underline link.
- **Founder section:** flipped to a tinted background (warm beige) so it visually anchors the page mid-scroll. Portrait left, story right, with a left-rule pull quote and a credential row separated by a hairline.
- **Patient journey:** three columns, oversized thin numerals (01 · 02 · 03) as the visual hook. No icons — keeps it clinical, not consumer-app.
- **Final CTA:** dark band (deep ink, not black) for contrast — the only dark surface on the page. White button, single message.
- **Footer:** one row. Resist the urge to add columns of links.

**Imagery direction:** abstract botanical, soft architectural light, or clean clinical interiors. No portraits in the hero. The Dr. Kurtz image should be a real, well-lit editorial portrait — replace the placeholder before launch.

---

## 4. Color Palette

| Token | Hex | Use |
|---|---|---|
| Background | `#FAFAF7` | Page background — warm off-white, not stark |
| Surface | `#FFFFFF` | Cards, trust strip |
| Tint | `#F1EFE8` | Founder section background, subtle banding |
| Ink | `#1A2422` | Headlines, body text, dark CTA section |
| Ink Soft | `#5A6862` | Subheads, captions, footer text |
| Accent | `#4A5D4F` | CTA, links, eyebrows — muted forest green |
| Accent Hover | `#2D3D32` | Pressed/hover state |
| Border | `#E8E5DD` | Hairlines, card borders |

Why these: a warm off-white base feels human (not clinical-cold); the muted forest accent reads as natural, established, and confident without the spa-green or wellness-mint that signals med-spa; the deep ink stays just shy of pure black, which keeps the page feeling soft.

---

## 5. Typography

- **Family:** Montserrat (Google Fonts), with system sans-serif as fallback.
- **Hero headline:** 600 weight, ~76px desktop, line-height 1.05, letter-spacing -0.02em.
- **Section titles:** 600 weight, ~50px desktop, letter-spacing -0.015em.
- **Subheads / body:** 400 weight, 18–19px, line-height 1.6, color Ink Soft.
- **Eyebrows:** 500 weight, 12px, uppercase, letter-spacing 0.22em, color Accent. These are the page's "stitching" — they show up in every section and give the design rhythm.
- **Buttons:** 500 weight, 14px, letter-spacing 0.04em. Square corners (2px radius) feel more clinical than rounded pills.
- **Hierarchy rule:** at most three type sizes on any one screen. If you're reaching for a fourth, you've added a section that doesn't need it.

---

## 6. Building It Quickly

The HTML file is a single self-contained page — no build step, no framework, drops straight into Lovable, v0, or Claude Artifacts.

**To use in Lovable / v0:** paste the HTML into a new project and ask the tool to "convert this static page to a Next.js + Tailwind component, preserving the design tokens." The CSS variables at the top map cleanly to a Tailwind theme.

**To swap imagery:**
- Hero image: replace the Unsplash URL in `.hero-image` with a brand asset (botanical, architectural, or clinical interior).
- Doctor portrait: replace the URL in `.doctor-image` with Dr. Kurtz's actual headshot.

**Quick tweaks worth making before showing the client:**
- Real Dr. Kurtz portrait and verified years-of-practice number.
- Confirm the four trust-strip claims with the practice (board certifications, etc.).
- Add the practice address and phone to the footer.
- Hook the "Book Consultation" button to the existing scheduling system.

**What to leave alone in the first review:**
- The section order. It's deliberately Next Health / Parsley-shaped.
- The single dark band at the end. It's the only place the page raises its voice.
- The lack of testimonials, blog teasers, and "as seen in" logos. Adding them now will dilute the premium read; they belong on a v2 once the foundation is approved.
