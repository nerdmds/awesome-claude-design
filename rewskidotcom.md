# Rewskidotcom — DESIGN.md

**Aesthetic Family:** Reframe Blue
**One-line:** Editorial builder voice. Monochromatic blue. High-signal density. Publication-feel, not blog-feel.
**Surface:** Substack, LinkedIn, X, carousel slides, quote cards, podcast show art, future Rewskidotcom.com landing
**Author:** Adam Carewe, MD — physician-executive, clinical informaticist, healthcare AI consultant

---

## 1. Brand Identity

Rewskidotcom is the publishing surface of a physician-builder reframing healthcare. Not healthcare reporting. Not AI hype analysis. A declarative reframe layer where clinical intuition, informatics expertise, and systems thinking compress into short, high-signal essays a reader finishes with a different mental model than they started with.

**Tagline (long):** Physician futurist, podcast host, technology, thought leadership, and radical dad reviews.
**Tagline (short):** Systems thinking from a clinician-builder.
**Positioning statement:** Not legacy medicine. Not Silicon Valley translation. A third thing: a physician who builds.

**Brand frame (load-bearing):** Builder vs Legacy. Every piece of content lives on one side or the other of that contrast. Explicit when relevant, implicit always.

**Macro framework:** System A / B / C
- **System A** — Evolutionary health (ancestral-fit, pre-industrial)
- **System B** — Industrialized medicine (what most healthcare is now)
- **System C** — Integrated intelligent scalable care (what we're building)

**Signature phrases (use and protect):**
- TurboTax moment for medicine
- AI as OS
- Culture eats AI for breakfast
- Trust-in-ease
- Thousand unmarked intersections
- Builder vs Legacy
- System A / B / C

### Weekly Cadence (the publishing heartbeat)

Three Substack posts per week. Each has a distinct format, voice register, and length. The cadence is the rhythm that earns the reader's trust.

```
SUNDAY SHARE       Personal anchor into systems reframe          ~800–1200 words
MONDAY FULL STACK  Architectural deep-thought                    ~1000–1500 words
FRIDAY NFF         No Fluff Friday, 5-section locked format      300–450 words
```

**Supporting cadences:**
- **NerdMDs StackBytes** — podcast companion micro-essays paired with audio
- **TechDadCO** — product reviews, family-facing tech evaluations (separate sub-publication on the Substack)

---

## 2. Color Tokens

Monochromatic blue. One palette, nine steps, no secondary hues. The only accent is a traffic-light trio reserved exclusively for the NFF Score (Signal / Theater / Noise).

### Primitives (Blue scale)

```
Paper              #F5F8FC   Primary background, Substack body surface
Surface            #FFFFFF   Elevated cards, quote card background
Mist               #E6EDF5   Secondary fills, section dividers background
Rule               #CBD8E8   Borders, hairlines
Mute               #94ADCD   Disabled, tertiary metadata
Steel              #5D7FAE   Secondary body text, captions
Signal             #2E5B8F   Primary brand blue, links, accent chrome
Deep               #1F4577   Subheads, emphasis
Inkwell            #13335C   Headline text
Abyss              #0A1F3D   Display text, hero headlines, wordmark
```

### NFF Score Accents (reserved, never decorative)

```
NFF-Signal         #1F7A4D   🟢 Real signal in the noise
NFF-Theater        #B7342B   🔴 Performative, pitch-deck theater
NFF-Noise          #C89418   🟡 Loud but empty, commentary that adds nothing
```

### Rules

- **Blue only for brand chrome.** No purple, teal, or secondary accent hues anywhere.
- **Signal / Theater / Noise are reserved.** Use exclusively in NFF Scores. Never as decorative accents in headers, buttons, or dividers.
- **Body text is always Inkwell or Steel.** Headlines always Abyss or Inkwell. Metadata always Mute.
- **Never use pure black (`#000000`) or pure white (`#FFFFFF`) for text.** Use Abyss and Paper.
- **High contrast is the point.** Default pairings: Abyss on Paper (14.2:1) or Paper on Signal (4.8:1).

---

## 3. Typography

Two typefaces. Nothing else.

### Typefaces

- **Display and Headlines:** Montserrat. Geometric, confident, modern. Weights 600, 700, 800.
- **Body and UI:** Inter. High-legibility at small sizes. Weights 400, 500, 600.

Web fallback stack: `system-ui, -apple-system, Segoe UI, Roboto, sans-serif`.

### Scale

```
TOKEN              FONT         WEIGHT     SIZE     LINE HEIGHT     USAGE
─────────────────────────────────────────────────────────────────────────────
Hero               Montserrat   800        56       64              Landing hero, cover
Display Large      Montserrat   700        40       48              Substack post titles
Display Medium     Montserrat   700        32       40              Section opens, H1 in Monday posts
Display Small      Montserrat   600        24       32              H2 section headers
Title Large        Inter        600        20       28              Card titles
Title Medium       Inter        600        17       24              UI headers
Body Large         Inter        400        18       28              Substack body copy
Body Medium        Inter        400        16       26              Standard body, LinkedIn, web
Body Small         Inter        400        14       22              Metadata, footer
Label              Inter        600        12       16              Overline, section markers (UPPERCASE, +1 tracking)
Caption            Inter        500        13       18              Image captions, pull quotes attribution
Mono               ui-monospace 500        14       22              Frameworks, code, signature phrases when isolated
```

### Rules

- Montserrat for display only. Inter for everything else. Never mix mid-sentence.
- Body copy is always Body Large (18px) on reading surfaces. Body Medium (16px) on UI.
- Overlines (Label token) are the only allowed uppercase. Plus 1pt letter tracking.
- Signature phrases like "Builder vs Legacy" or "System A / B / C" render in Mono when isolated as a framework callout. Inline in body they stay sans.
- Minimum text size anywhere: 12pt. No exceptions.

---

## 4. Spacing & Layout

### Scale (4pt base grid)

```
4     Inline element gaps
8     Tight padding, related element spacing
12    Icon-label gaps
16    Standard card padding, tight section spacing
24    Card-to-card spacing, body paragraph spacing
32    Section breaks within an article
48    Major section breaks, hero padding
64    Landing-page section breaks
96    Hero vertical padding on desktop
```

### Layout Rules

- **Reading surfaces (Substack, blog):** Max content width 680px. Left-aligned. Never centered body copy.
- **Landing and web surfaces:** Max container 1200px. 16-unit horizontal padding on mobile, 48 on desktop.
- **Split-screen device:** The core visual motif. 50/50 two-column blocks for Builder vs Legacy, Old vs New, Noise vs Signal. Hard divider line in Rule, 1px. Left column is always "before/legacy." Right column is always "after/builder."
- **Single column below 768px.** Split-screen blocks stack vertically with the "legacy" side on top, "builder" side below.
- **Body paragraphs:** 24px spacing. No first-line indentation. No justified text.
- **Pull quotes:** Full-bleed on desktop (extend past reading column), 4px left border in Signal, Display Small font.

---

## 5. Components

### Post Hero (Substack, LinkedIn Newsletter, Web)

```
[Optional Label overline in Steel, 12pt, +1 tracking]
[Display Large headline in Abyss, left-aligned, max 3 lines]
[Subtitle in Deep, Display Small, single declarative sentence]
[Author line: Adam Carewe, MD · date, Body Small in Mute]
```

**Rules:**
- Headline is always declarative. Never interrogative unless the question is the thesis.
- Subtitle delivers the thesis in one sentence. Reader can close the tab after reading the subtitle and still have the take.
- No excerpt or dek beyond the subtitle.

### Cover Image (Substack post art, podcast episode art)

```
Format:     1280 × 1280 square (Substack, podcast); 1200 × 628 (LinkedIn share)
Palette:    Abyss background, Signal or Paper typography
Type:       Hero token, Montserrat 800, max 6 words
Layout:     Bottom-left or centered, generous negative space
Imagery:    Never stock photos. Either typography-only or minimal geometric abstraction.
Wordmark:   Optional "rewskidotcom" in Mono, Paper, bottom-right corner, small
```

**Never:** stock photography, AI-generated people, clip-art, generic tech imagery (glowing brains, circuit boards, hand-shake-through-screen).

### Quote Card (repurpose from any post to X, LinkedIn, Instagram)

```
Dimensions:     1200 × 1200 square
Background:     Paper
Border:         8px Signal on left edge only
Quote:          Display Medium in Abyss, max 4 lines, left-aligned
Attribution:    Body Small in Steel, bottom-left: "Adam Carewe, MD · Rewskidotcom"
Wordmark:       Small Signal "r." mark, bottom-right
Padding:        64px all sides
```

### Carousel Slide (LinkedIn, Instagram)

```
Dimensions:     1080 × 1350 portrait (LinkedIn carousel standard)
Slide 1 (Hook):
  - Abyss background
  - Hero token headline in Paper, 4-6 words, bold declarative
  - Tiny Mute "1 / N" counter, top-right
Interior slides:
  - Paper background
  - Display Medium headline in Abyss, top
  - Body Large supporting prose in Inkwell, max 40 words
  - Steel "N / total" counter, top-right
Closing slide:
  - Signal background
  - Paper typography
  - One CTA verb + link (e.g. "Read the full reframe at rewskidotcom.substack.com")
```

Minimum 5 slides. Maximum 9. Every carousel ends with a CTA slide.

### Split-Screen Contrast Block (web, landing, carousel)

The load-bearing visual device of the brand.

```
Layout:      50/50 two-column on desktop, stacked on mobile
Divider:     1px Rule, vertical on desktop, horizontal on mobile
Left (Legacy):
  - Mist background
  - Label overline: "LEGACY" or "BEFORE" in Steel
  - Display Small headline in Inkwell
  - Body Medium description in Steel, 2–3 lines
Right (Builder):
  - Paper background
  - Label overline: "BUILDER" or "AFTER" in Signal
  - Display Small headline in Abyss
  - Body Medium description in Inkwell, 2–3 lines
```

Use for: System A/B, System B/C, Legacy/Builder, Old Workflow/New Workflow, Noise/Signal.

### Framework Callout

For isolating signature phrases as structural elements.

```
Background:     Mist
Border:         1px Rule, all sides, 8px corner radius
Padding:        24px
Content:        Mono token, 14px, Inkwell, bold
Prefix:         Small Signal dot, 6px diameter, left of text
```

Example:

```
● Builder vs Legacy
● System A → System B → System C
● Distribution ate the model.
```

### CTA Button (web, Substack button blocks)

```
Primary:
  Background:    Signal
  Text:          Paper, Label token
  Corner radius: 8px
  Padding:       16px vertical, 32px horizontal
  Hover:         Deep background
Secondary:
  Background:    Paper
  Text:          Signal, Label token
  Border:        2px Signal
  Corner radius: 8px
```

Button labels are verbs plus object: "Read the Reframe," "Subscribe to Rewskidotcom," "Get the Build."

---

## 6. Motion & Interaction

Minimal. Editorial publications don't animate. Animation signals status change only, never decoration.

### Allowed

- Hover state on links: Signal to Deep, 150ms ease-out
- Hover on CTA buttons: background color transition, 150ms ease-out
- Carousel advance: hard cut, no transition animation
- Image lazy-load: 200ms fade in
- Split-screen reveal on scroll: 400ms ease-out, subtle (optional, desktop only)

### Forbidden

- Parallax scrolling
- Scroll-jacking
- Auto-playing video
- Animated gradients
- Bouncing emoji
- Anything that says "we hired a motion designer"

Respect `prefers-reduced-motion`. Replace all animation with instant state changes.

---

## 7. Iconography

Minimal. Lucide or Feather icon set. 1.5px stroke weight. Never filled unless active state requires it.

### Sizing

```
CONTEXT              SIZE     STROKE    COLOR
──────────────────────────────────────────────────
Inline UI            18px     1.5px     Steel / Signal active
Section header       24px     1.5px     Signal
Empty state          48px     1.5px     Mute
Hero                 64px     2px       Signal (sparingly)
```

### NFF Score Marks (exception)

Native emoji traffic lights: 🟢 🔴 🟡. These are the only emoji allowed anywhere in the brand system. They are structural, not decorative.

### Rules

- No emoji in headlines, body copy, or UI labels. Exception: NFF Score traffic lights.
- No flags, no clip-art medical icons, no stethoscope silhouettes.
- Prefer typographic marks over icons when possible (e.g., "→" arrow glyph instead of an arrow icon).

---

## 8. Tone & Voice

### Core rules

- **Declarative.** Never hedge. Never "it could be argued." State the thing.
- **Systems-level.** Diagnose the system, not the symptom. Workflow, incentive, architecture, distribution, not vibes.
- **Forward-leaning.** End on the build move. Never end on the diagnosis.
- **Three-layer pattern:** Problem → Root cause → New model. Never stop at the complaint.
- **Four-beat narrative:** Observation → System-level diagnosis → Strategic reframing → Future-oriented implication.

### Voice attributes

- Clinician-credible but not clinician-dense
- Technologist-literate but not technologist-captured
- Confident but not cocky
- Opinionated but not preachy

### Voice register by cadence

The three weekly cadences occupy distinct voice registers. The DESIGN.md preserves them separately.

```
SUNDAY SHARE       Reflective, first-person, essay-pace. Opens personal, resolves systemic.
                   Uses "I" and "we" freely. Sign-off: "— Adam"

MONDAY FULL STACK  Architectural, confident, framework-heavy. Short sentences as paragraphs.
                   Uses lists and contrast blocks. Opens with a provocation.

FRIDAY NFF         Compressed, scoring-mindset. 300–450 words max.
                   No throat-clearing. Every sentence is load-bearing.
```

### Banned constructions

- Em-dashes (use periods, colons, or commas)
- Hedging phrases: "could be," "might be," "perhaps," "it seems"
- Filler closers: "let me know what you think," "curious to hear your take," "hope this helps"
- Melodrama: "the heartbreaking truth is," "we owe it to our patients"
- Overcitation: more than one study reference per 300 words signals insecurity
- AI-generated voice markers: "delve," "crucial," "in today's rapidly evolving landscape"

### Required closers (pattern library)

- **Sunday Share:** italicized reflective provocation + `— Adam` sign-off
- **Monday Full Stack:** forward-leaning question that invites engagement without begging for it
- **Friday NFF:** none. The traffic-light score IS the closer.

Never: "Let me know your thoughts."

### Naming conventions

```
Author byline             "Adam Carewe, MD"
Publication name          "Rewskidotcom" (one word, lowercase in URLs, title case in prose)
Domain                    rewskidotcom.substack.com (redirect target: rewskidotcom.com)
Podcast                   "Efficiency Unlocked | Nerd Tested. MD Approved."
Consulting practice       "NerdMDs Consulting"
Podcast companion         "NerdMDs StackBytes"
Product reviews           "TechDadCO"
Weekly formats            "Sunday Share", "Monday Full Stack", "No Fluff Friday" or "NFF"
AI posture                "Builder" (not "AI enthusiast," not "AI skeptic")
```

---

## 9. Cadence Templates

Three locked templates. Each is a signed contract between reader and publication. Deviation breaks the rhythm.

### 9A. Sunday Share — personal anchor into systems reframe

**Purpose:** Build relational equity. Start personal, end systemic. The Sunday reader wants to spend time, not scan.

**Length:** 800–1200 words
**Publish:** Sunday evening

**Overline format:**
```
SUNDAY SHARE | [TOPIC TAG]
```

Examples: `SUNDAY SHARE | SLEEP + HEALTHCARE`, `SUNDAY SHARE | MATCH DAY + INFORMATICS`, `SUNDAY SHARE | BUILDING`.

**Structural pattern:**

```
[Overline: SUNDAY SHARE | TOPIC]
[Display Large headline, declarative, personal-adjacent]
[Subtitle, the thesis in one sentence]

[Opening hook, 1–3 short paragraphs]
  Personal anchor. A thing that happened. A product that broke. A moment remembered.
  Transition sentence that widens from personal to relevant-to-reader.

[H2 section 1]
  The "Problem Isn't X. It's Y." pattern works well here.
  2–4 paragraphs that reframe the personal anchor into a systemic observation.

[H2 section 2]
  Architectural reframe. The builder's diagnosis.
  What the system is actually doing, not what it claims.

[H2 section 3]
  The white space. What nobody has built yet.
  Where the reader should look.

[Optional H2: caveat or nuance section]
  "One Caveat Worth Naming" or equivalent. Shows intellectual honesty.

[Italicized closing reflection, 1–2 paragraphs]
  Forward-leaning. Connects back to the opening personal anchor.

— Adam

[Italicized related-posts pointer line]
  "If this resonated, [link to series]. For the [angle] take, [link]."
```

**Visual rules:**
- Cover image: typography or minimal abstraction in Abyss and Signal
- One or two inline images allowed (lifestyle, product, memory-anchored). Never stock.
- Caption in Caption token, Steel, italic.
- Horizontal rule (`---`) between major section transitions.
- Links to prior posts in Signal, underlined on hover only.

**Headline pattern examples (live from publication):**
- "The Signal Is In Your Bed. The Care Pathway Isn't."
- "The Match That Made Me"

**Subtitle pattern:** One declarative sentence that delivers the thesis. Example: "Eight Sleep just raised $50M and is chasing FDA clearance for sleep apnea detection. That's the easy part. Here's what still needs to be built."

---

### 9B. Monday Full Stack — architectural deep-thought

**Purpose:** Establish intellectual authority. Deep reframe. Architecturally confident.

**Length:** 1000–1500 words
**Publish:** Monday morning

**Structural pattern:**

```
[Display Large headline, short, declarative, often a provocation]
[Subtitle, same as or echoes the headline]

[Opening, 3–6 short sentences, each as its own paragraph]
  A common question or assumption.
  The wrong framing.
  The real framing.
  (Short, punchy, each sentence is load-bearing.)

[Optional: Part N framing, linking prior posts in a series]

[H1 section: "What people get wrong about X"]
  The mistaken mental model.
  Use bullet lists with parallel structure.

[H1 section: "What X should actually do"]
  The correct model. Bullets. Frameworks. Architecture language.

[H1 section: "What X must never do"]
  Constraints and rails. Structured list.

[H1 section: "How [thing] changes with [builder model]"]
  Before/after contrast. Use the Without/With pattern:

  Without agents, the day begins behind:
    - inbox churn
    - refill clarifications
    - scheduling noise

  With agents, the day begins ahead:
    - every patient pre-summarized
    - labs digested
    - red flags surfaced

[H1 section: "What disappears" / "What remains"]
  Two parallel lists. What the builder model kills. What only humans keep.

[Closing, 3–5 short sentences, each as its own paragraph]
  One-line summary of the argument.
  A forward-leaning question that invites engagement.
```

**Visual rules:**
- H1 sections render as bold Display Medium in Abyss (not overlines)
- Heavy use of bulleted lists with parallel structure. 3–7 items per list is the sweet spot.
- No em-dashes. Use periods or colons.
- Whitespace is a design element. Short paragraphs. Don't fear short lines.
- Horizontal rules (`---`) between H1 sections.

**Signature structural devices:**
- "X is not Y. It is Z." — the core reframe sentence pattern
- Without/With contrast blocks (see above)
- What X should / must never — paired constraint lists
- Zero-click / One-click task taxonomy
- What disappears / What remains — final contrast pair

**Headline pattern examples (live from publication):**
- "Everyone wants an AI doctor. Almost no one is building the right kind."
- "How Much of Medicine Is Actually an Algorithm?"
- "Concierge medicine is incredible. Unless..."

---

### 9C. Friday NFF — No Fluff Friday (compressed score)

**Purpose:** Weekly scan of Signal, Theater, Noise. Reader gets the build move in under 3 minutes.

**Length:** 300–450 words. Strict.
**Publish:** Friday morning

**Structural pattern (locked, non-negotiable):**

```
[Display Large headline]
[Subtitle, the thesis in one declarative sentence]

[Section overline in Label token, Signal color: "THE SIGNAL"]
  2–3 short paragraphs. What's real. The thing the reader might have missed.

[Section overline: "THE NOISE"]
  2–3 short paragraphs. The dominant but shallow narrative.

[Section overline: "THE REFRAME"]
  2–4 short paragraphs. The builder's reframe. System-level diagnosis.

[Section overline: "THE BUILD"]
  2–3 short paragraphs. What to do with this. The actionable next move.

[Section overline: "THIS WEEK'S NFF SCORE"]
  🟢 Signal — [one declarative sentence]
  🔴 Theater — [one declarative sentence]
  🟡 Noise — [one declarative sentence]
```

**Visual rules:**
- Section labels render as Label token overlines in Signal color, small dot bullet before
- NFF Score uses native emoji traffic lights as the only allowed emoji
- No inline images except the cover
- No links except the standard Substack subscribe CTA at top and bottom
- No "Let me know what you think" or similar. The Score IS the closer.

**Cover image override:** NFF covers should feel like a weekly edition. Consider a small `NFF #NN` or date stamp in Mono, Paper, bottom-right corner of the cover.

**Headline pattern examples (live from publication):**
- "NFF: No Foundation Needed"

---

## 10. Example Screens & Surfaces

### Substack Post Page (any cadence)

Paper background. Content column 680px, left-aligned. Hero up top (Label overline → Display Large headline → Display Small subtitle → author line). Body in Body Large, paragraphs 24 apart. Horizontal rules between major transitions. Signal CTA button at bottom ("Subscribe").

### LinkedIn Post (text only)

No carousel, pure post. 180–220 words. Opens with a declarative hook (1 line). Three body paragraphs. Closes with the build move. Signature phrases isolated on their own lines for scannability. No hashtags except one at the end: `#Rewskidotcom`.

### X / Thread

5–9 tweets. Tweet 1 is the hook (the subtitle of the Substack post, adapted). Tweets 2 through N are one point each. Last tweet is the CTA plus link to Substack. No emoji except NFF traffic lights if scoring. No threads about threads.

### Landing (future rewskidotcom.com)

```
HERO
  Abyss background, full viewport height
  Label overline "REWSKIDOTCOM" in Signal, top-center
  Hero headline in Paper: "Systems thinking from a clinician-builder."
  Signal CTA "Read the reframe"
  Subtle scroll indicator at bottom

SECTION 1 — The weekly cadence
  Paper background, Mist dividers
  Three columns side by side on desktop, stacked on mobile:
    SUNDAY SHARE       "Personal anchor. Systemic reframe."
    MONDAY FULL STACK  "Architectural deep-thought."
    FRIDAY NFF         "Signal. Theater. Noise. Scored."
  Each column: Label overline, Display Small title, Body Medium description, Signal tertiary link

SECTION 2 — Split-screen Builder vs Legacy
  Full-width split-screen contrast block
  "LEGACY: The way healthcare talks about AI."
  "BUILDER: The way healthcare should build with AI."

SECTION 3 — Latest from each cadence
  Mist background
  Three most recent posts, one per cadence, as cards
  Each card: cover image (Abyss), Display Small title, Body Medium subtitle, date in Mute

SECTION 4 — Frameworks (framework callouts row)
  Paper background
  Three framework callouts side by side:
    ● Builder vs Legacy
    ● System A / B / C
    ● Trust-in-ease

SECTION 5 — Subscribe
  Signal background, Paper typography
  "Three posts a week. No fluff."
  Email input + Signal CTA

FOOTER
  Abyss, minimal, Mono wordmark, social links
```

### Podcast Episode Art (StackBytes)

```
1280 × 1280
Abyss background
Label overline in Signal: "NERDMDS STACKBYTES · #NN"
Hero headline in Paper, Montserrat 800, max 6 words
Small Mute line below: "with Adam Carewe, MD"
Wordmark "r." in Signal, bottom-right
```

---

## Do / Don't

**Do:**
- Monochromatic blue. One palette, nine steps, no exceptions.
- Montserrat for display, Inter for body. Nothing else.
- Declarative headlines. The subtitle delivers the thesis.
- Split-screen Builder vs Legacy as the load-bearing visual device.
- NFF Score traffic lights as the only emoji.
- Preserve the cadence voice register: Sunday reflective, Monday architectural, Friday compressed.
- End every post on the build move, not the diagnosis.

**Don't:**
- Secondary accent colors beyond the NFF traffic lights.
- Stock photography. Glowing brains. Hands shaking through screens.
- Em-dashes. Hedging. Filler closers.
- Emoji outside the NFF Score.
- Melodrama. Overcitation. AI-voice markers.
- Question-headline hooks unless the question is the thesis.
- Drift between cadence voices. Monday is not Sunday. Friday is not Monday.

---

## Repurposing Chain (required thinking pattern)

Every long-form post must be planned as a distribution chain before it's written:

```
Substack long-form    →    Primary surface, length by cadence
LinkedIn post         →    180–220 words, declarative version
LinkedIn carousel     →    5–9 slides, hook + reframe + build
X thread              →    5–9 tweets, hook → points → CTA
Quote cards           →    2–3 pull quotes as 1:1 image cards
Podcast companion     →    NerdMDs StackBytes episode or segment
Micro-content         →    Single-sentence X posts isolating signature phrases
```

If a post can't produce at least three of these downstream assets, it's not ready to publish.

---

*Aesthetic Family: Reframe Blue*
*Source: rewskidotcom.substack.com · Builder vs Legacy · System A / B / C*
*Version 1.1 — Cadence templates codified from live Sunday Share, Monday Full Stack, and Friday NFF posts*
