# NerdMDs — DESIGN.md

**Aesthetic Family:** Pocket Protector
**One-line:** Clinical authority meets technical fluency. Nerdy in the self-aware, credentialed sense. Navy and ivory professionalism with a typographic wink.
**Surface:** nerdmds.com, advisory proposals, pitch deck templates, LinkedIn company presence, podcast episode art, client-facing PDFs
**Principals:** Adam Carewe, MD and Dale Gold, MD — double-board certified physician executives

> **Version status:** v1.0 codifies the current brand state. The live nerdmds.com is a WordPress-base site and is targeted for a full redesign using a modern aesthetic from this repo. This DESIGN.md establishes the brand identity as structured tokens so the redesign preserves voice and positioning while upgrading visual execution.

---

## 1. Brand Identity

NerdMDs is a physician executive advisory practice. Not a generic consulting shop. Not a health-tech promoter. A credentialed bridge between enterprise-scale healthcare operations and early-stage startup execution, built by clinicians who have done both.

**Tagline (locked):** Letting doctors be doctors.
**Positioning one-liner:** Most health-tech advisors come from one world. We come from both.
**Headline framing:** The NerdMDs Difference.

**The two-world bridge (core positioning device):**

```
ENTERPRISE HEALTHCARE               EARLY-STAGE EXECUTION
Kaiser Permanente CMIO              Startup advisory and build
Clinical informatics at scale       Health-tech venture counsel
EHR implementation                  Go-to-market pressure testing
Frontline clinical care             Board-level strategy
```

The brand is the `=` sign in the middle. Credible on both sides. Rare as a matter of credentialing, not just claim.

**Who we work with:** providers, health systems, payers, investors, startups — anyone who needs guidance "grounded in clinical reality, not just market maps."

**What we do (service architecture):**

```
ADVISORY & CONSULTATION        Fractional CMIO, board counsel, strategic engagements
15-MINUTE PITCH                Fast-calibration intake; credentialed feedback on a pitch
LINKEDIN ANALYSIS              Clinician-facing analysis tooling
APPEARANCES                    Speaking, podcasting, panels
PODCAST                        Efficiency Unlocked | Nerd Tested. MD Approved.
```

**Brand temperament:** approachable authority. We're not ivory tower. We're NerdMDs — the physicians who also read the docs, run the experiments, and ship the builds. Self-aware. Technically fluent. Credentialed.

**Signature phrases (protect these):**
- Letting doctors be doctors
- Nerd Tested. MD Approved.
- The NerdMDs Difference
- Two-world bridge
- Credentialed feedback

---

## 2. Color Tokens

Navy-led consulting palette with an ivory clinical background. One structural accent (Graph Paper Blue) for nerdy-technical notes. Clinical Red reserved for medical cross motifs and urgent CTAs only.

### Primitives

```
Ivory              #F6F4EE   Primary background (clinical cleanliness)
Paper              #FFFFFF   Elevated surfaces, service cards
Bone               #EEECE4   Secondary fills, sidebars
Rule               #D8D4C8   Borders, hairlines
Mute               #8B877B   Disabled, tertiary metadata

Slate              #4A5468   Body text, secondary UI
Steel              #2E3A4F   Subheads, emphasis
Navy               #102138   Primary brand color, CTAs, chrome
Ink                #0A1423   Headline text, wordmark

Graph              #3A6BA5   Accent: technical callouts, graph-paper motif, charts
Graph-Pale         #E5EEF7   Accent background tint

Clinical-Red       #B0342B   Medical cross motif, urgent CTAs (reserved)
Terminal-Green     #1F6B43   Terminal/code accents, success states (reserved)
```

### Rules

- **Navy is the default primary.** Ivory is the default background. This pairing is the brand.
- **Graph is a structural accent, not decorative.** Use for callouts, inline notes, chart elements, and subtle differentiation within long documents.
- **Clinical-Red is reserved.** Medical cross, urgent-action CTAs, and nothing else. Never use for chrome or navigation.
- **Terminal-Green is reserved.** Code blocks, terminal references, success states, "it works" moments. Never as decoration.
- **Never use pure black or pure white for text.** Use Ink and Paper.
- **Body text is always Slate.** Headlines always Ink or Navy. Metadata always Mute.
- **Contrast floor:** Slate on Ivory = 6.8:1. Navy on Ivory = 13.1:1. Keep Mute for non-essential text only.

---

## 3. Typography

IBM Plex family across the board. The family carries technical-intellectual credibility (originated at IBM for enterprise tech) without being stuffy. Serif for display gravitas. Sans for body legibility. Mono for code, frameworks, and credential strips.

### Typefaces

- **Display & Headlines:** IBM Plex Serif — weights 500, 600, 700
- **Body & UI:** IBM Plex Sans — weights 400, 500, 600
- **Code, Mono, Credentials:** IBM Plex Mono — weights 400, 500

Web fallback stacks:
```
Serif:  "IBM Plex Serif", Georgia, "Times New Roman", serif
Sans:   "IBM Plex Sans", system-ui, -apple-system, sans-serif
Mono:   "IBM Plex Mono", ui-monospace, Menlo, monospace
```

### Scale

```
TOKEN              FONT              WEIGHT     SIZE     LINE HEIGHT     USAGE
────────────────────────────────────────────────────────────────────────────────
Hero               Plex Serif        700        56       64              Landing hero
Display Large      Plex Serif        600        40       48              Page titles
Display Medium     Plex Serif        600        32       40              Section opens
Display Small      Plex Serif        500        24       32              Subsection headers
Title Large        Plex Sans         600        20       28              Service card titles
Title Medium       Plex Sans         600        17       24              UI headers
Body Large         Plex Sans         400        18       28              Long-form body
Body Medium        Plex Sans         400        16       26              Standard body, web
Body Small         Plex Sans         400        14       22              Metadata, footnotes
Label              Plex Sans         600        12       16              Overline, section markers (UPPERCASE, +1 tracking)
Caption            Plex Sans         500        13       18              Captions, attribution
Mono Label         Plex Mono         500        12       18              Credential strips, "MD" suffixes, tags
Mono Body          Plex Mono         400        14       22              Code, frameworks, service names
```

### Rules

- Plex Serif for display only. Plex Sans for body. Plex Mono for code and credentials.
- Credential suffixes ("MD", "MS", "MHI") render in Plex Mono at 0.85em to create visual differentiation. Example: "Adam Carewe, `MD`" where `MD` is monospaced and slightly smaller.
- Overlines (Label token) are the only allowed uppercase in sans. Plus 1pt letter tracking.
- Service names ("Advisory", "15-Minute Pitch", "LinkedIn Analysis") render in Plex Mono when isolated as structural elements (sidebar, service index).
- Minimum text size anywhere: 12pt. No exceptions.
- Never use Serif for body text. The reading flow is always Sans.

---

## 4. Spacing & Layout

### Scale (4pt base grid)

```
4     Inline element gaps
8     Tight padding
12    Icon-label gaps
16    Standard card padding
24    Paragraph spacing, service card separation
32    Section breaks within a page
48    Major section breaks, hero padding
64    Landing-page section breaks
96    Hero vertical padding on desktop
```

### Layout Rules

- **Reading surfaces:** Max content width 720px. Left-aligned. Never centered body copy.
- **Landing / web:** Max container 1200px. Side padding 16pt mobile, 48pt desktop.
- **Service grid:** 3-column on desktop, 2-column on tablet, stacked on mobile. Cards are equal height.
- **Credential strip device:** Horizontal row of credentials/logos/client names, equal spacing, Plex Mono styling. Used in footer and "About" sections.
- **Grid paper motif (optional subtle accent):** Background grid pattern using Graph-Pale hairlines at 32pt spacing for section dividers or hero blocks. Use sparingly. Never behind body text.
- **Body paragraphs:** 24pt spacing. No first-line indentation. No justified text.

---

## 5. Components

### Page Hero

```
[Label overline in Graph, 12pt, +1 tracking: e.g. "ADVISORY & CONSULTATION"]
[Display Large headline in Ink, Plex Serif 600]
[Subtitle in Slate, Body Large, 2 lines max]
[Primary CTA in Navy, secondary link in Graph]
```

### Service Card

The primary content container on the site. Three or more service cards arranged in a grid.

```
Background:     Paper
Border:         1pt Rule, all sides
Corner radius:  8px (sharper than Rewski's 12 — signals precision)
Padding:        24pt all sides
Spacing:        24pt between cards

Structure:
  [Icon or numeral in Graph, 24pt]
  [Title in Ink, Title Large Plex Sans]
  [Mono tag in Graph: service code or duration, e.g. "15 MIN" or "ADVISORY"]
  [Body Medium description in Slate, 3–4 lines]
  [Tertiary link in Navy, "Learn more →" or "Book a session →"]
```

Hover state: 1pt border becomes 2pt Navy. Background stays Paper.

### Credential Strip

A horizontal band of credentials, affiliations, or client logos. The credibility-at-a-glance device.

```
Background:     Ivory (or Bone on dark-section contrast)
Padding:        32pt vertical
Layout:         Horizontal flex, equal spacing, centered
Content:        Plex Mono in Slate, all caps, 14pt
Separators:     Vertical Rule bars, 1pt, 16pt tall
Items:          "KAISER PERMANENTE  |  EPIC CERTIFIED  |  BOARD CERTIFIED IN CLINICAL INFORMATICS  |  PHYSICIAN BUILDER PROGRAM"
```

Use in: About page, footer context bar, proposal cover sheets.

### Byline Block

How principals are introduced. Preserves credential gravitas without over-formatting.

```
[Avatar, 48px circular, Rule 1pt border]
[Name in Ink, Title Large: "Adam Carewe"]
[Credential line in Slate, Plex Mono 13pt: "MD · Clinical Informatics · MS (Nutrition)"]
[Role line in Slate, Body Small: "Co-founder, NerdMDs · Clinical Product Lead, General Medicine"]
```

### Pull Quote

```
Background:     Bone
Border:         4px left border in Navy
Padding:        24pt
Quote:          Plex Serif 500, Display Small, Ink
Attribution:    Body Small in Slate, Plex Mono, prefix with "—"
```

### Framework / Data Callout

```
Background:     Graph-Pale
Border:         1pt Graph on all sides, 6px corner radius
Padding:        20pt
Label:          Plex Mono 12pt Graph, all caps: "FRAMEWORK" or "DATA POINT"
Content:        Plex Serif 500 in Ink, 18pt
```

Use for: numerical claims ("13 years at Kaiser"), framework statements, supporting facts.

### CTA Button

```
Primary:
  Background:    Navy
  Text:          Ivory, Plex Sans 600, 14pt
  Corner radius: 6px (sharper than Rewski; signals professional precision)
  Padding:       14pt vertical, 28pt horizontal
  Hover:         Ink background

Secondary:
  Background:    Ivory
  Text:          Navy, Plex Sans 600
  Border:        2px Navy
  Corner radius: 6px

Destructive / Clinical:
  Background:    Clinical-Red
  Text:          Ivory
  Reserved for:  urgent clinical-context CTAs only
```

Button labels use verbs + object: "Book a 15-Minute Pitch," "Download the Advisory Brief," "Contact NerdMDs."

### Navigation

- **Top nav:** Ivory background, 1pt Rule bottom border, Plex Sans 500 in Slate, 15pt. Active state: Navy underline, 2px.
- **Footer:** Ink background, Ivory text. Credential strip, contact line, social icons (Plex Mono footer).

---

## 6. Motion & Interaction

Restrained. Consulting brands don't animate. Signal credibility through stillness and precision.

### Allowed

- Hover state on links: Slate → Navy, 150ms ease-out
- Hover on CTAs: background color transition, 150ms ease-out
- Hover on service cards: border thickness 1pt → 2pt Navy, 150ms ease-out
- Fade-in for section reveals on scroll: 400ms ease-out, subtle, desktop only
- Image lazy-load: 200ms fade

### Forbidden

- Parallax
- Scroll-jacking
- Auto-play video or GIFs
- Animated gradients
- Bouncing, sliding, or rotating elements
- Any animation longer than 400ms
- Cursor effects or hover gimmicks

Respect `prefers-reduced-motion`. Replace all animation with instant state changes.

---

## 7. Iconography

Lucide icon set. 1.5px stroke weight. Navy color default, Graph color for technical/data contexts.

### Sizing

```
CONTEXT              SIZE     STROKE    COLOR
──────────────────────────────────────────────────
Inline UI            18px     1.5px     Slate / Navy active
Service card         24px     1.5px     Graph
Section header       24px     1.5px     Navy
Empty state          48px     1.5px     Mute
Hero                 64px     2px       Navy (sparingly)
```

### Key assignments

```
Advisory / consulting        briefcase
15-Minute Pitch              timer
LinkedIn Analysis            bar-chart-2
Podcast                      mic
Appearances                  mic-2
Videos                       play-circle
Contact                      mail
Download                     download
External link                arrow-up-right
Check / validated            check-circle
```

### Rules

- No emoji in headlines, body, or UI. No exceptions.
- No clip-art medical icons. No stethoscope-shaped dividers. No RX logo motifs.
- The medical cross symbol, if used at all, appears only in the logo lockup. Never decoratively.
- Prefer typographic marks over icons when the marker is structural ("→" instead of arrow icon).

---

## 8. Tone & Voice

### Core rules

- **Credentialed.** Every claim is backed by experience. "We led clinical informatics at the largest integrated health system in the United States" is the voice — specific, verifiable, not boastful.
- **Dual-fluent.** Speak clinical and technical in the same paragraph without translation friction.
- **Plainspoken.** No jargon for jargon's sake. If a VP of a health system and a seed-stage founder both read it, both understand it, both feel respected.
- **Forward-leaning.** Every page ends with a clear next action.
- **Self-aware nerdy.** We're NerdMDs. Lean into it lightly. Don't overdo it.

### Voice attributes

- Credible but not arrogant
- Technical but not gatekeeping
- Professional but not sterile
- Warm but not casual
- Confident but not braggadocious

### Banned constructions

- Em-dashes (use periods, colons, or commas)
- Hedging: "could be," "might be," "we think," "potentially"
- Filler: "at the end of the day," "moving the needle," "in today's landscape"
- Consulting-deck jargon: "synergy," "bandwidth," "holistic approach," "white-glove"
- Over-hype: "revolutionary," "transformative," "game-changing"
- Stock credibility phrases: "trusted by," "industry-leading," "world-class" (unless literally true and specific)

### Required patterns

- **Specific credentials, always.** "Double-board certified" with both specialties named.
- **Specific institutions, always.** "Kaiser Permanente" not "a large integrated health system."
- **Specific durations.** "13 years" not "over a decade."
- **One CTA per page.** Pages don't ask for three things. They ask for one.

### Naming conventions

```
Company name              "NerdMDs" (one word, mixed case, no period)
Legal entity              "NerdMDs LLC"
Domain                    nerdmds.com
Principals                "Adam Carewe, MD" and "Dale Gold, MD" (credential in Plex Mono)
Tagline                   "Letting doctors be doctors" (always lowercase, quoted)
Podcast                   "Efficiency Unlocked | Nerd Tested. MD Approved."
Service names (locked)    "Advisory", "15-Minute Pitch", "LinkedIn Analysis", "Appearances"
Never                     "NERD-MDS", "nerd MDs", "Nerd MDs", "nerdmds.com" in body prose (use "NerdMDs")
```

---

## 9. Example Screens & Surfaces

### Home / Advisory Landing

```
HERO
  Ivory background
  Label overline in Graph: "PHYSICIAN EXECUTIVE ADVISORY"
  Display Large headline in Ink: "Letting doctors be doctors."
  Subtitle in Slate, Body Large: "Most health-tech advisors come from one world. We come from both."
  Primary CTA (Navy): "Book a 15-Minute Pitch"
  Secondary link (Graph): "Read the advisory brief →"

SECTION — The Two-World Bridge
  Full-width split block. Ivory background, Bone divider.
  Left: "ENTERPRISE HEALTHCARE" credential strip
  Right: "EARLY-STAGE EXECUTION" credential strip
  Centered: Display Medium in Ink — "We live in the gap where projects fail."

SECTION — The NerdMDs Difference
  Three service cards side by side on desktop
  "ADVISORY" · "15-MINUTE PITCH" · "LINKEDIN ANALYSIS"

SECTION — Principals
  Two byline blocks side by side
  Adam Carewe, MD and Dale Gold, MD
  Each with credential strip and one-sentence bio

SECTION — Recent Work / Appearances
  Credential strip of client names or appearance venues (if public)
  Link to full Appearances page

SECTION — CTA Band
  Navy background, Ivory type
  "Not sure where to start?"
  Primary CTA (Ivory button, Navy text): "Book a 15-Minute Pitch"

FOOTER
  Ink background, Ivory type
  Credential strip (certifications, board memberships)
  Contact: info@nerdmds.com
  Plex Mono social links
```

### Service Detail Page (e.g., Advisory)

Ivory background, 720px content column. Breadcrumb in Mute, Plex Mono. Page hero. Three-part structure: "What it is" / "Who it's for" / "How it works." Each section opens with a Display Small header in Serif, body in Sans. Ends with a single CTA and a Pull Quote from a past client (if permissioned).

### 15-Minute Pitch Page

More conversational. Still the Pocket Protector aesthetic. Explains the format, the credentialed feedback, what to prepare. Booking CTA prominent. Framework callout block: "WHAT YOU GET" in Graph-Pale, three bullet points in Plex Serif 500.

### Proposal / Advisory Brief PDF (Cover Page)

```
Ivory background, full bleed
Credential strip across the top in Plex Mono
Centered block:
  "ADVISORY BRIEF" overline in Graph, Plex Mono
  Client name in Display Large Plex Serif
  Date and engagement scope in Plex Mono, Slate
Footer strip with "NerdMDs LLC · info@nerdmds.com"
Subtle Graph grid paper motif in background at 10% opacity
```

### Podcast Episode Art (Efficiency Unlocked)

```
1280 × 1280
Ink background
Label overline in Graph, Plex Mono: "EFFICIENCY UNLOCKED · EP #NN"
Hero headline in Ivory, Plex Serif 700, max 6 words
Subtitle in Mute, Plex Sans 500, one line
Bottom-right: "NERD TESTED. MD APPROVED." in Plex Mono, Graph
```

---

## Do / Don't

**Do:**
- Navy and Ivory as the default pairing.
- IBM Plex Serif for display, Sans for body, Mono for credentials and code.
- Credential strips as the structural credibility device.
- Specific credentials, institutions, and durations.
- One CTA per page.
- Sharper corner radii (6–8px) than the editorial brands — signals precision.

**Don't:**
- Use Clinical-Red for anything other than reserved medical/urgent contexts.
- Use Graph as a decorative accent. It's structural.
- Use em-dashes, stock credibility phrases, or consulting-deck jargon.
- Use any typeface other than IBM Plex across the system.
- Use emoji. Ever. Not in social, not in UI, not in anything.
- Describe ourselves as "revolutionary" or "trusted." Let the credential strip do that work.

---

## 10. Migration Notes (for the upcoming redesign)

This document codifies NerdMDs v1.0 as brand identity. The current nerdmds.com runs on WordPress with standard template chrome. The redesign will migrate to a modern stack (likely Next.js or Astro) and adopt one of the DESIGN.md aesthetic families from this repo.

**What transfers unchanged to v2:**
- Tagline, positioning, signature phrases
- Service architecture and service names
- Voice rules and banned constructions
- Credential strip as a structural device
- Two-world bridge as the core positioning visual

**What may evolve in v2:**
- Exact hex values (Navy/Ivory will stay directionally, but sampled from the new logo treatment)
- Typography (IBM Plex is strong; swap only if the chosen aesthetic family requires)
- Corner radii and spacing scale
- Hero treatments and motion allowances
- Grid paper motif (may be retired or amplified depending on direction)

**The redesign should not break:**
- The clinical authority signal
- The dual-fluent voice
- The "Letting doctors be doctors" tagline
- The credential-forward information architecture

---

*Aesthetic Family: Pocket Protector*
*Source: nerdmds.com · Adam Carewe, MD + Dale Gold, MD · "Letting doctors be doctors"*
*Version 1.0 — Current-state brand codification, designed to evolve into a modern redesign*
