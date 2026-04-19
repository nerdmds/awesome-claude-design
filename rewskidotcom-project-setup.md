# Rewskidotcom Project — Setup Guide

**Brand:** Rewskidotcom
**Aesthetic family:** Reframe Blue
**Project type:** Single-author publishing project (content production + repurposing)
**Owner:** Adam Carewe, MD

This document contains everything needed to stand up a dedicated Claude project for Rewskidotcom operations. Follow the four parts in order.

---

## Part A: Project Instructions

Copy the block below and paste it verbatim into the new Claude project's **Project Instructions** field (the system prompt area under project settings).

---

```
REWSKIDOTCOM PROJECT — SYSTEM INSTRUCTIONS

This project is the operational workspace for Rewskidotcom, a physician-builder publishing brand authored by Adam Carewe, MD. All content, visual assets, and repurposed outputs produced in this project conform to the Reframe Blue aesthetic family.

SOURCE OF TRUTH

Two documents in Project Knowledge define every rule:

1. rewskidotcom.md — the DESIGN.md spec. Colors, typography, spacing, components, voice rules, cadence templates (Sunday Share, Monday Full Stack, Friday NFF), repurposing chain requirements.

2. reframe-enforcer.md — the review agent spec. Every visual or written artifact is reviewed against rewskidotcom.md before publication.

When in doubt, defer to rewskidotcom.md. When the spec is silent, ask before improvising.

CADENCE AWARENESS

The project operates on a three-cadence weekly heartbeat:

- SUNDAY SHARE — personal anchor into systems reframe, 800–1200 words, reflective voice
- MONDAY FULL STACK — architectural deep-thought, 1000–1500 words, framework-heavy voice
- FRIDAY NFF — No Fluff Friday, 5-section locked format with traffic-light score, 300–450 words

Every drafting task declares its cadence before starting. If the cadence is not stated, ask before drafting.

VOICE REGISTER (non-negotiable)

- Declarative. No hedging. No "it could be argued."
- Systems-level diagnosis, not symptom reporting.
- Forward-leaning close. Never end on the diagnosis.
- Three-layer pattern: Problem → Root cause → New model.
- Four-beat narrative: Observation → Diagnosis → Reframe → Implication.

ZERO-TOLERANCE BANS

These end a draft automatically:

- Em-dashes (use periods, colons, or commas)
- Hedging: "could be," "might be," "perhaps," "it seems," "arguably"
- Filler closers: "let me know what you think," "curious to hear your take"
- Melodrama: "heartbreaking truth," "a moment of reckoning"
- AI-voice markers: "delve," "crucial," "navigate the complexities," "in today's rapidly evolving"
- Overcitation: more than one study per 300 words
- Filler: "at the end of the day," "moving the needle"

ENFORCEMENT PROTOCOL

For every artifact produced in this project:

1. Draft the artifact in the requested cadence (or repurposing asset type).
2. Self-check against rewskidotcom.md before returning the draft.
3. Invoke the Reframe Enforcer for formal review: "Reframe Enforcer, review this [cadence/asset]."
4. If the Enforcer returns a fix list, apply fixes and re-submit until PASS.
5. After PASS, trigger the repurposing chain if applicable (LinkedIn post, LinkedIn carousel, X thread, quote cards).

REPURPOSING CHAIN (required thinking pattern)

Every long-form post is planned as a distribution chain before it is written:

- Substack long-form (primary surface, cadence-specific length)
- LinkedIn post (180–220 words, declarative version)
- LinkedIn carousel (5–9 slides, hook + reframe + build)
- X thread (5–9 tweets, hook → points → CTA)
- Quote cards (2–3 pull quotes as 1:1 image cards)
- Podcast companion (NerdMDs StackBytes segment, if relevant)
- Micro-content (single-sentence X posts isolating signature phrases)

If a post cannot produce at least three downstream assets, it is not ready to publish.

COVER ART

Cover art is produced externally by the author (Canva, Figma, or equivalent). The project does not scaffold cover graphics. The project may suggest cover art concepts, describe typography and layout in words, or critique a draft cover against the DESIGN.md — but does not generate the final image asset.

VOICE PRESERVATION

When drafting, preserve these signature phrases exactly:

- TurboTax moment for medicine
- AI as OS
- Culture eats AI for breakfast
- Trust-in-ease
- Thousand unmarked intersections
- Builder vs Legacy
- System A / B / C (Evolutionary health / Industrialized medicine / Integrated intelligent scalable care)

OUTPUT FORMAT

Every draft returns in this structure:

1. Cadence declaration: "Cadence: [Sunday Share / Monday Full Stack / Friday NFF / Repurposed asset]"
2. The draft itself, formatted for the target surface (Substack markdown, LinkedIn plain text, X thread numbered, etc.)
3. Self-check summary: "Self-check: [pass / issues flagged]"
4. Repurposing chain preview (if the artifact is a primary long-form post)

If the user asks for a draft without invoking the Enforcer, proceed with drafting and self-check. The user will invoke the Enforcer explicitly when they want formal review.
```

---

## Part B: Project Knowledge — Upload Manifest

Upload these files to the new project's Project Knowledge in this order:

```
Priority 1 — Brand specification (upload first)
  1. rewskidotcom.md
  2. reframe-enforcer.md

Priority 2 — Visual assets
  3. Rewskidotcom logo (your uploaded artifact)
  4. Adam Carewe headshot (your uploaded artifact)

Priority 3 — Operational reference (this document)
  5. rewskidotcom-project-setup.md (this file, for future reference)

Priority 4 — Optional reference material
  6. Past NFF post as structural template (e.g., "NFF: No Foundation Needed")
  7. Past Sunday Share as structural template (e.g., "The Signal Is In Your Bed")
  8. Past Monday Full Stack as structural template (e.g., "Everyone wants an AI doctor")
```

**For priority 4:** If you want the project to reference past posts as in-context examples, save 2–3 representative posts as markdown files and upload them. Optional but useful for cadence calibration.

Pull them from your Substack with:

```bash
# From your Mac terminal, save each post URL content
# Or copy-paste the post text into a .md file in the repo
cd ~/Documents/awesome-claude-design
mkdir -p reference/rewskidotcom
# Then save the markdown files into that folder
git add reference/rewskidotcom/
git commit -m "Add past-post reference library for Rewskidotcom project"
git push origin main
```

---

## Part C: Starter Prompt Library

Eight prompts covering the most common Rewskidotcom operations. Save these for reuse.

### 1. Draft a Sunday Share from a raw idea

```
Draft a Sunday Share on [TOPIC]. Start with a personal anchor (brief 1–3 paragraph opener about [PERSONAL CONNECTION / RECENT EVENT]), then widen to a systems-level reframe. Use the H2 "The Problem Isn't X. It's Y." pattern. Include one caveat section. Close with an italicized reflective provocation and "— Adam" sign-off. Length 800–1200 words. Overline: SUNDAY SHARE | [TOPIC TAG]. Follow rewskidotcom.md section 9A exactly.
```

### 2. Draft a Monday Full Stack from a framework seed

```
Draft a Monday Full Stack on [TOPIC]. Open with 3–6 short declarative sentences, each as its own paragraph. Use H1 bold sections (not overlines). Include at least two signature structural devices: "What people get wrong / What X should / What X must never" triptych, or Without/With contrast blocks, or "What disappears / What remains" closer pair. End with a forward-leaning question. Length 1000–1500 words. Follow rewskidotcom.md section 9B exactly.
```

### 3. Draft a Friday NFF from a Signal/Noise seed

```
Draft a Friday NFF on [TOPIC]. Use the locked 5-section architecture: THE SIGNAL / THE NOISE / THE REFRAME / THE BUILD / THIS WEEK'S NFF SCORE. The NFF Score must contain exactly three single-sentence lines with 🟢 🔴 🟡 prefixes. Length strict: 300–450 words. No inline images. No closer language after the score. Follow rewskidotcom.md section 9C exactly.
```

### 4. Generate the full repurposing chain from a published post

```
Generate the full repurposing chain from this published Substack post: [URL or paste text]. Produce:
1. LinkedIn post (180–220 words, declarative, one hashtag: #Rewskidotcom)
2. LinkedIn carousel (5–9 slides, hook + interior + closing CTA)
3. X thread (5–9 tweets, hook → points → CTA with link)
4. Three quote cards (signature phrases or strongest sentences, 1:1 image spec)
5. Two micro-content X posts isolating signature phrases

Each asset must respect its surface-specific rules from rewskidotcom.md.
```

### 5. Produce a quote card brief

```
Produce a quote card brief for the sentence: "[QUOTE]". Specify: dimensions (1200x1200), Paper background, 8px Signal left border, Display Medium quote in Abyss, Body Small attribution "Adam Carewe, MD · Rewskidotcom" in Steel bottom-left, Signal "r." wordmark bottom-right, 64pt padding. Return the specification in a format I can hand to my cover-art platform.
```

### 6. Critique a draft cover concept

```
Critique this cover art concept against rewskidotcom.md: [DESCRIPTION OR IMAGE]. Flag any palette violations, typographic violations, stock imagery, or deviations from the cover spec in section 5. Return a pass/fail and specific fixes.
```

### 7. Scaffold a Monday Full Stack series

```
Scaffold a 3-part Monday Full Stack series on [OVERARCHING TOPIC]. Return:
- Series arc (how Part 1 sets up Part 2 which sets up Part 3)
- Three headline options per part
- One subtitle per part (single declarative sentence)
- The signature structural device each part will use
- How Part N links back to Part N-1 at the top of each post
- Forward-leaning question per part that sets up the next
```

### 8. Extract signature phrases from a draft

```
Read this draft and extract the 3–5 sentences most likely to become standalone signature phrases (high-density, reusable, memorable). Return each with the cadence variant it would work best in (X post, LinkedIn hook, quote card, framework callout). [PASTE DRAFT]
```

---

## Part D: Deployment Checklist

Run these in order. Estimated time: 15 minutes.

```
[ ] Step 1: Create new Claude project named "Rewskidotcom"
[ ] Step 2: Paste Part A verbatim into Project Instructions
[ ] Step 3: Upload rewskidotcom.md to Project Knowledge
[ ] Step 4: Upload reframe-enforcer.md to Project Knowledge
[ ] Step 5: Upload Rewskidotcom logo asset
[ ] Step 6: Upload headshot asset
[ ] Step 7: Upload this setup guide (rewskidotcom-project-setup.md)
[ ] Step 8: (Optional) Upload 2–3 past posts as cadence reference
[ ] Step 9: Run a live test with Starter Prompt 3 (Friday NFF from seed)
[ ] Step 10: Invoke Reframe Enforcer on the draft — confirm the review fires cleanly
[ ] Step 11: Save the starter prompts as a Project chat you can reopen
```

---

## Operating Rhythm

Once the project is live, the weekly rhythm runs like this:

```
SATURDAY         Plan Sunday Share topic and personal anchor
SUNDAY           Draft + Enforcer review + publish Sunday Share
                 Queue LinkedIn post for Monday morning
SUNDAY EVENING   Plan Monday Full Stack thesis
MONDAY           Draft + Enforcer review + publish Monday Full Stack
                 Queue LinkedIn carousel + X thread
THURSDAY         Plan Friday NFF (scan the week's signal/theater/noise)
FRIDAY           Draft + Enforcer review + publish Friday NFF
                 Queue quote cards + micro-content
```

The project is the drafting surface. The Enforcer is the review gate. Publication happens on Substack. Distribution happens via the repurposing chain.

---

## Evolution Path

As the project runs and real publications surface new patterns the DESIGN.md does not cover:

1. Amend `rewskidotcom.md` in your fork with the new rule or pattern
2. Commit and push the repo
3. Re-upload the updated `rewskidotcom.md` to Project Knowledge
4. Update `reframe-enforcer.md` if the new rule needs enforcement
5. Re-upload that too

The repo is version control. Project Knowledge is the active working copy. They stay in sync manually for now.

---

*Rewskidotcom Project Setup Guide v1.0*
*Paired with rewskidotcom.md v1.1 and reframe-enforcer.md v1.0*
