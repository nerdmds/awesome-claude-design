# NerdMDs Project — Setup Guide

**Brand:** NerdMDs
**Aesthetic family:** Pocket Protector
**Project type:** Advisory and consulting operations workspace
**Principals:** Adam Carewe, MD + Dale Gold, MD

This document contains everything needed to stand up a dedicated Claude project for NerdMDs advisory operations. Follow the four parts in order.

---

## Pitch Site Reconciliation (read first)

The live **pitch.nerdmds.com** (Vercel subdomain) represents a more modern execution than the current nerdmds.com WordPress base. Inspection revealed:

**What pitch.nerdmds.com does well (preserve these as v2 directional cues):**

- Credential stats bar: "50 States Licensed · 15+ Years at Kaiser · C-Suite Leadership · 100% No-Fluff Policy"
- Numbered process cards (01, 02, 03) for "Three steps. Zero friction."
- Hero copy that hits specific credentials fast: "A 50-state licensed physician. 15+ years inside Kaiser Permanente. Chief Medical Information Officer."
- Tagline placement in footer: "Letting doctors be doctors."
- Clear single CTA: "Book & Pay Now — $100"
- Quote attribution format: "— Adam, NerdMDs Founder"

**What pitch.nerdmds.com does that conflicts with the strict Pocket Protector DESIGN.md:**

- Uses emoji as section icons (🩺 💬 📝)
- Uses em-dash in attribution ("— Adam")
- Uses en-dash in pricing ("Book & Pay Now — $100")

**Reconciliation decision you need to make:**

Option 1 — **Tighten pitch site to match DESIGN.md**
Replace emoji icons with Lucide SF-symbol-style line icons. Replace em-dashes with colons or commas. Cleaner, more disciplined.

Option 2 — **Amend DESIGN.md to add a "Pitch Surface Exception"**
Allow emoji icons in numbered process cards and stats bars (structural, not decorative). Allow em-dash in attribution only (typographic convention for quotes). Documented exception, not silent drift.

Recommendation: **Option 2**. The pitch site's emoji-as-structural-icon usage is not decorative — it is functional iconography in a specific component context. Amending the spec acknowledges real-world product reality and keeps enforcement tight.

If you want to proceed with Option 2, I can produce a `nerdmds.md v1.1` amendment adding the Pitch Surface Exception. Say the word.

---

## Part A: Project Instructions

Copy the block below and paste it verbatim into the new Claude project's **Project Instructions** field.

---

```
NERDMDS PROJECT — SYSTEM INSTRUCTIONS

This project is the operational workspace for NerdMDs, a physician-executive advisory practice founded by Adam Carewe, MD and Dale Gold, MD. All client-facing artifacts, proposals, landing pages, pitch materials, podcast episode assets, and outbound correspondence produced in this project conform to the Pocket Protector aesthetic family.

SOURCE OF TRUTH

Two documents in Project Knowledge define every rule:

1. nerdmds.md — the DESIGN.md spec. Colors (Navy + Ivory palette), typography (IBM Plex Serif/Sans/Mono), spacing, components, voice rules, credential integrity requirements.

2. pocket-protector-enforcer.md — the review agent spec. Every client-facing artifact is reviewed against nerdmds.md before delivery.

LIVE REFERENCE

- nerdmds.com — current WordPress-based site (targeted for redesign)
- pitch.nerdmds.com — modern Vercel-based pitch subdomain (directional cue for v2)

When nerdmds.md and pitch.nerdmds.com conflict, nerdmds.md wins unless an explicit Pitch Surface Exception has been added to the DESIGN.md.

BRAND POSITIONING (non-negotiable)

Tagline: "Letting doctors be doctors" (always lowercase, in quotes when inline)
Positioning: Most health-tech advisors come from one world. We come from both.
Two-world bridge: Enterprise healthcare (Kaiser CMIO, clinical informatics at scale) and early-stage execution (startup advisory, health-tech venture).

The brand is the "=" sign in the middle. Credible on both sides. Rare as a matter of credentialing, not just claim.

VOICE (non-negotiable)

- Credentialed: every claim backed by specific, verifiable experience.
- Dual-fluent: clinical and technical in the same paragraph without translation friction.
- Plainspoken: accessible to VPs of health systems and seed-stage founders alike.
- Forward-leaning: every page or document ends with a clear next action.
- Self-aware nerdy: lean into "NerdMDs" lightly, never overdo it.

ZERO-TOLERANCE BANS

These end a draft automatically:

- Em-dashes in body copy (use periods, colons, or commas). Exception: attribution lines if Pitch Surface Exception applies.
- Hedging: "could be," "might be," "we think," "potentially"
- Consulting-deck jargon: "synergy," "bandwidth," "holistic approach," "white-glove," "thought partner," "value-add"
- Over-hype: "revolutionary," "transformative," "game-changing," "paradigm shift"
- Stock credibility without specifics: "trusted by," "industry-leading," "world-class"
- AI-voice markers: "delve," "crucial," "navigate the complexities," "in today's rapidly evolving"
- Overly casual: emoji-laden prose, "hey there," "fam"
- Overly formal: "we are pleased to announce," "please find attached herewith"

CREDENTIAL INTEGRITY (high-weight)

Every credentialing claim must be specific:

- "Double-board certified in Family Medicine and Clinical Informatics" not "board certified"
- "Kaiser Permanente" not "a large integrated health system"
- "13 years" not "over a decade"
- "Chief Medical Information Officer" not "healthcare technology leader"

First-reference principal attribution always includes credential suffix: "Adam Carewe, MD" or "Dale Gold, MD" — never "Dr. Carewe" alone in first reference.

SERVICE NAMES (locked)

Render exactly:
- Advisory
- 15-Minute Pitch
- LinkedIn Analysis
- Appearances

Never abbreviate ("15MP") or rename ("the pitch service") in client-facing materials.

CTA DISCIPLINE

One primary CTA per page or document. CTA labels are verb + object:
- "Book a 15-Minute Pitch"
- "Download the Advisory Brief"
- "Contact NerdMDs"

Never CTAs phrased as nouns ("Pitch session"), passive ("Be contacted"), or stacked three-deep.

ENFORCEMENT PROTOCOL

For every artifact produced in this project:

1. Draft the artifact per request (proposal, landing copy, email, deck, podcast content).
2. Self-check against nerdmds.md before returning.
3. Invoke the Pocket Protector Enforcer for formal review: "Pocket Protector Enforcer, review this [artifact type]."
4. If the Enforcer returns a fix list, apply fixes and re-submit until PASS.
5. Credential-integrity check is mandatory for any client-facing artifact.

OUTPUT FORMAT

Every draft returns in this structure:

1. Artifact type declaration: "Artifact: [Advisory Brief / Pitch page copy / Outbound email / Podcast episode description / etc.]"
2. The draft itself, formatted for the target surface
3. Self-check summary: "Self-check: [pass / issues flagged]"
4. Credential density note: "Credential density: [appropriate / requires more specifics]"

If the user asks for a draft without invoking the Enforcer, proceed with drafting and self-check. The user will invoke the Enforcer explicitly when they want formal review.
```

---

## Part B: Project Knowledge — Upload Manifest

Upload these files to the new project's Project Knowledge in this order:

```
Priority 1 — Brand specification (upload first)
  1. nerdmds.md
  2. pocket-protector-enforcer.md

Priority 2 — Visual assets
  3. NerdMDs horizontal logo (your uploaded artifact)
  4. NerdMDs square icon (your uploaded artifact)
  5. Adam Carewe headshot (your uploaded artifact)

Priority 3 — Operational reference (this document)
  6. nerdmds-project-setup.md (this file)

Priority 4 — Directional reference
  7. Screenshot or rendered copy of pitch.nerdmds.com (as v2 design cue)
  8. Any existing advisory brief PDF (if available) for voice calibration
  9. Dr. Dale Gold bio or headshot (when available)
```

**For priority 4 item 7**, you can either:
- Take a full-page screenshot of pitch.nerdmds.com and upload as PNG
- Use a browser "save as PDF" and upload
- Have me produce a structured description of the pitch site as a markdown reference file

---

## Part C: Starter Prompt Library

Eight prompts covering the most common NerdMDs operations. Save these for reuse.

### 1. Respond to an inbound 15-Minute Pitch request

```
Draft a response to this inbound 15-Minute Pitch request: [PASTE INQUIRY]. Acknowledge the specific project area they mentioned, surface one clarifying question before booking (if applicable), include the booking link (pitch.nerdmds.com), and close with a single CTA. Keep to 5–8 sentences. Credential-forward without over-hyping. Professional but not sterile.
```

### 2. Draft an Advisory Brief one-pager

```
Draft an Advisory Brief one-pager for a prospective client: [CLIENT NAME, STAGE, FOCUS AREA]. Structure:
- Credential strip at top (Kaiser CMIO, double-board certified, 13 years enterprise + startup builder)
- "The Engagement" — 2–3 sentence summary of what NerdMDs brings to this specific client's situation
- "What We've Done" — three specific precedents with named institutions and durations
- "What We'll Deliver" — bulleted scope specific to their stage
- Single CTA: "Book a 15-Minute Pitch" with pitch.nerdmds.com link
Length: one page. Voice: credentialed, dual-fluent, no consulting-deck jargon. Follow nerdmds.md.
```

### 3. Produce a pitch deck slide sequence

```
Produce a 7-slide pitch deck for [AUDIENCE: prospective client / speaking engagement / investor panel]. Each slide returns as: slide number, headline (Display Medium Plex Serif), body copy (Plex Sans), any credential strip or framework callout content. Colors reference nerdmds.md tokens. Preserve two-world bridge positioning across the arc.
```

### 4. Draft podcast episode description for Efficiency Unlocked

```
Draft a podcast episode description for Efficiency Unlocked, episode #[NN]. Topic: [TOPIC]. Guest: [GUEST NAME, CREDENTIALS]. Structure:
- Episode title (max 8 words, declarative)
- Episode subtitle (single sentence, the thesis)
- 3-paragraph description (the question → the guest's lens → why it matters now)
- 5 timestamped highlights
- Guest bio paragraph
Voice: credentialed, dual-fluent, listenable. Length: 200–300 words total. Include standard CTA to Rewskidotcom and NerdMDs.
```

### 5. Credential-forward outbound email

```
Draft an outbound email to [PROSPECT NAME, ROLE, COMPANY]. Context: [WHY YOU'RE REACHING OUT]. Ask: [SPECIFIC ASK]. Structure:
- Subject line: specific, not cute
- 3–4 short paragraphs, each with a purpose
- One clear ask at the end
- Sign-off with credential line under name
Voice: credentialed without peacocking, respectful of their time, specific about why this outreach makes sense. No "hope this finds you well" or similar filler.
```

### 6. LinkedIn Analysis service landing copy

```
Draft the hero + feature section for a LinkedIn Analysis service page. The service provides [DESCRIBE SERVICE]. Structure:
- Hero overline (Graph Plex Mono): service category
- Hero headline (Display Large Plex Serif): declarative value statement
- Hero subtitle (Slate Body Large): single sentence thesis
- Three feature cards (Graph icon + Plex Sans title + Slate description + "Mono tag" + Navy tertiary link)
- Single primary CTA button
Follow nerdmds.md section 5 component specs. No emoji, no em-dashes. Credential-forward.
```

### 7. Reconcile a pitch.nerdmds.com page against DESIGN.md

```
Review this pitch.nerdmds.com page section against nerdmds.md and flag any drift: [PASTE SECTION OR URL]. Categorize violations by: palette, typography, voice, credential integrity, CTA discipline. For each, quote the offending element and propose the specific fix. If the violation could be solved by amending the DESIGN.md with a Pitch Surface Exception, note that option.
```

### 8. Two-world bridge positioning statement

```
Draft a 150-word "About NerdMDs" positioning statement for [CONTEXT: website, speaker bio, proposal cover, LinkedIn]. Lead with the two-world bridge. Name specific institutions and credentials. No over-hype. No stock credibility phrases. End with a forward-leaning sentence that implies the next action (contact / learn more / book pitch). Pair with a credential strip of 4 items.
```

---

## Part D: Deployment Checklist

Run these in order. Estimated time: 20 minutes.

```
[ ] Step 1: Decide on Pitch Site Reconciliation (Option 1 tighten or Option 2 amend DESIGN.md)
[ ] Step 2: If Option 2, request DESIGN.md v1.1 amendment from Claude with Pitch Surface Exception
[ ] Step 3: Create new Claude project named "NerdMDs"
[ ] Step 4: Paste Part A verbatim into Project Instructions
[ ] Step 5: Upload nerdmds.md (v1.0 or v1.1 per step 2) to Project Knowledge
[ ] Step 6: Upload pocket-protector-enforcer.md to Project Knowledge
[ ] Step 7: Upload NerdMDs horizontal logo
[ ] Step 8: Upload NerdMDs square icon
[ ] Step 9: Upload Adam Carewe headshot
[ ] Step 10: Upload this setup guide (nerdmds-project-setup.md)
[ ] Step 11: (Optional) Upload pitch.nerdmds.com reference (screenshot or structured markdown)
[ ] Step 12: Run a live test with Starter Prompt 1 (Inbound 15-Minute Pitch response)
[ ] Step 13: Invoke Pocket Protector Enforcer on the draft — confirm the review fires cleanly
[ ] Step 14: Save starter prompts as a Project chat for reuse
```

---

## Operating Rhythm

Once the project is live, typical activities run like this:

```
INBOUND CLIENT INQUIRIES       Draft response → Enforcer review → Send
ADVISORY BRIEF PRODUCTION      Draft brief → Enforcer review → Export to PDF
PODCAST PRODUCTION             Draft episode description + bio → Enforcer review → Publish
OUTBOUND OUTREACH              Draft email → Enforcer review → Send from personal email
PITCH SITE REVISIONS           Produce copy → Enforcer review → Deploy via pitch.nerdmds.com
LINKEDIN COMPANY CONTENT       Draft post → Enforcer review → Publish
LANDING PAGE SCAFFOLDS         Produce scaffold → Enforcer review → Hand to Claude Design for visual
```

The project is the drafting and review surface. Production surfaces (pitch.nerdmds.com, Substack, LinkedIn, email) are external. Enforcement happens here; shipping happens there.

---

## Coordination With Other Brand Projects

NerdMDs frequently intersects with the other two brand projects. Cross-brand rules:

**NerdMDs ↔ Rewskidotcom:**
- NerdMDs StackBytes podcast lives in the Rewskidotcom project (editorial surface)
- References to NerdMDs services within Rewskidotcom content follow Reframe Blue voice, not Pocket Protector voice
- When a Rewskidotcom post promotes a NerdMDs engagement, the Reframe Enforcer reviews the post; the Pocket Protector Enforcer reviews any linked collateral

**NerdMDs ↔ Porch.family:**
- Porch is a NerdMDs-authored product but uses the Hearth Structured aesthetic, not Pocket Protector
- When NerdMDs client-facing materials reference Porch as a portfolio example, the Pocket Protector voice applies to the prose; Porch imagery honors its own DESIGN.md
- A NerdMDs case study about Porch reads "We built Porch..." with Pocket Protector voice; screenshots of Porch retain Hearth Structured aesthetic

**When in doubt:** the surface dictates the aesthetic. If the artifact is published under NerdMDs (nerdmds.com, advisory briefs, client decks), Pocket Protector rules. If the artifact is published under another brand, the other brand's rules apply.

---

## Evolution Path

As the project runs and real client engagements surface patterns the DESIGN.md does not cover:

1. Amend `nerdmds.md` in your fork with the new rule
2. Commit and push the repo
3. Re-upload updated `nerdmds.md` to Project Knowledge
4. Update `pocket-protector-enforcer.md` if the new rule needs enforcement
5. Re-upload that too

Specific upcoming amendments anticipated:

- Pitch Surface Exception (if you choose Option 2 in the reconciliation decision)
- Case study template (when you accumulate 3+ shipped engagements worth featuring)
- Dale Gold byline block specification (when Dale's assets are in the system)
- Email signature template for NerdMDs outbound

Each of these can ship as a v1.N amendment when you're ready.

---

*NerdMDs Project Setup Guide v1.0*
*Paired with nerdmds.md v1.0 and pocket-protector-enforcer.md v1.0*
