# Porch — DESIGN.md

**Aesthetic Family:** Hearth Structured
**One-line:** Apple Reminders meets a warm living room. Structured, glanceable, human.
**Surface:** Native iOS (primary) + web marketing surfaces (landing, docs, brand assets)
**Source of truth for iOS implementation:** `/specs/design-system.md` in the Porch repo. This DESIGN.md is the Claude Design companion for scaffolding web artifacts on-brand.

---

## 1. Brand Identity

Porch is the quiet family operating layer. Not a productivity app, not a surveillance tool. A warm, structured space where a household's reminders, locations, trips, and messages live together.

**North star:** A teenager can use it without instruction. A parent trusts it with their family's location. Neither feels like the target demographic was an afterthought.

**Voice:** Warm, direct, plain. Never cute. Never corporate.
**Tagline pattern:** "The family [noun], quieter." / "Your family, in one place."
**Brand word:** Porch (wordmark ends with a period: `Porch.`)

**Positioning contrasts:**
- Not Life360 (surveillance framing, anxiety-driven)
- Not Apple Reminders (individual, not familial)
- Not a chat app (structure, not conversation)
- Closest cousin: the front porch itself — a shared, warm, visible place everyone in the family knows about

---

## 2. Color Tokens

### Primitives

```
Cream              #FAF7F2   Primary background
Warm               #F2EDE4   Secondary background, card fills
Surface            #FFFFFF   Elevated surfaces, sheets, inputs

Ink                #1A1610   Primary text, headings
Ink-Mid            #4A3F30   Body text
Ink-Light          #8A7A65   Metadata, timestamps
Ink-Faint          #C8BFB0   Placeholder, disabled

Amber              #C8860A   Primary accent (only accent color)
Amber-Light        #E8A020   Hover, pressed states
Amber-Pale         #FDF3E0   Selected background, badges

Green              #2D6A4F   Success, location-active
Green-Pale         #EDF5F0   Success background tint
Red                #C0392B   Destructive, errors
Red-Pale           #FDEAEA   Error background tint
Blue               #2E6B9E   Links, informational
Blue-Pale          #E8F0F7   Informational background tint

Rule               #E2D8CC   Dividers, borders
Rule-Light         #F0EAE0   Subtle dividers within cards
```

### Family Member Rotation (max 6)

Assigned sequentially to family members for calendar and location ID:

```
Amber              #C8860A
Forest             #2D6A4F
Slate Blue         #4A6FA5
Terracotta         #C45D3E
Plum               #7B5EA7
Teal               #3A8A7C
```

### Rules

- Amber is the only accent color. No blue/purple CTAs. Semantic colors (green, red, blue) are reserved for status.
- Never use pure black (`#000000`) or pure white (`#FFFFFF`) for text. Use Ink and Cream.
- Dark mode is not in V1. Structure allows future extension. Lock light mode.

---

## 3. Typography

### Typefaces

- **Body:** SF Pro (iOS) / `system-ui, -apple-system` (web fallback)
- **Display:** Georgia (serif) — brand moments only

### Scale

```
TOKEN              FONT        WEIGHT     SIZE     LINE HEIGHT
───────────────────────────────────────────────────────────────
Display Large      Georgia     Bold       28       34
Display Small      Georgia     Regular    22       28
Title Large        SF Pro      Semibold   20       26
Title Medium       SF Pro      Semibold   17       22
Title Small        SF Pro      Medium     15       20
Body Large         SF Pro      Regular    17       24
Body Medium        SF Pro      Regular    15       22
Body Small         SF Pro      Regular    13       18
Label Large        SF Pro      Semibold   15       20
Label Medium       SF Pro      Medium     13       18
Label Small        SF Pro      Medium     11       14
Caption            SF Pro      Regular    12       16
```

### Rules

- Georgia appears in exactly two places: the `Porch.` wordmark and rare display titles. Nowhere else.
- Body text is always Ink-Mid. Headings are always Ink. Metadata is always Ink-Light.
- No ALL CAPS in user-facing text. Exception: overline labels (Label Small) with +1pt tracking.
- Minimum app text: 11pt. Minimum widget text: 13pt.

---

## 4. Spacing & Layout

### Scale (4pt base grid)

```
2    Hairline adjustments
4    Inline element gaps
8    Related element spacing
12   Icon-label gaps
16   Standard padding, card internal margins
20   Section spacing in scroll views
24   Card-to-card spacing
32   Major section breaks
48   Screen-level top/bottom padding
```

### Rules

- Screen edge padding: 16pt horizontal. No exceptions.
- Card internal padding: 16pt all sides.
- Minimum list item height: 52pt (44pt touch target + 8pt breathing room).
- Single column on phone. Two-column split on tablet.
- All primary screens scroll. Never truncate behind a fixed viewport.

---

## 5. Components

### Buttons

**Primary (CTA):** Amber fill, Surface text (Label Large), 12pt radius, 50pt height, full width. Pressed: Amber-Light + scale 0.98.

**Secondary:** Warm fill, Ink text, 1pt Rule border, same dimensions.

**Tertiary (text):** Transparent, Amber text (Label Medium). Used for inline actions: "See All", "Add", "Edit".

**Destructive:** Secondary structure, Red text.

**Icon Button:** 44pt touch target, 22pt icon. Ink-Mid default, Amber active.

### Cards

Primary content container.

```
Background:     Surface (white)
Corner radius:  16pt
Border:         none
Shadow:         Ink at 4% opacity, 8pt radius, 2pt y-offset
Internal pad:   16pt all sides
Between cards:  24pt
```

**Variants:**
- **Standard:** White + shadow (reminders, messages, trips)
- **Tinted:** Amber-Pale fill, 1pt Rule border, no shadow (featured/AI suggestions)
- **Status:** 4pt left border accent in semantic color (location, geofence triggers)

### Lists

Apple Reminders aesthetic. Left-aligned content, right-aligned metadata. 52pt minimum row, 8pt vertical padding.

**Checkable row (Reminders):**
- Unchecked: open circle, 24pt, Ink-Mid stroke
- Checked: filled Amber circle + white checkmark, title gets strikethrough + Ink-Light color
- Animation: spring fill over 0.3s, checkmark fades in

**Dividers:** Rule-Light, 1pt, inset 52pt from leading edge to align past icon column. Never full-width.

### Inputs

```
Background:     Surface
Border:         1pt Rule (default), 1pt Amber (focused)
Corner radius:  12pt
Height:         48pt single line
Padding:        16pt horizontal, 12pt vertical
Label:          Label Small above, Ink-Light
Error:          Red border, Caption Red message below
```

### Navigation

- **Tab bar:** System default. Cream background, Rule-Light top border. Icons: Ink-Light inactive, Amber active.
- **Nav bar:** System default. Tint Amber. Never custom.

### Badges & Chips

- **Count badge:** Red capsule, white 11pt bold, 18pt min width.
- **Status chip:** Semantic pale fill + matching text color, 8pt radius, 10/4pt padding.
- **Avatar:** Circle, assigned family color, white first initial at 60% of circle diameter. 32pt list, 40pt detail, 24pt inline.

### Empty States

Every empty-possible screen has one.

```
[48pt SF Symbol, Ink-Faint]
Title Medium, Ink
Body Medium, Ink-Light, max 2 lines, centered
[Primary Button]
```

Center vertically. Never show a blank screen.

### Sheets

- Background: Cream
- Drag indicator visible
- Detents: Medium for quick-add flows, Large for detail views and AI chat

---

## 6. Motion & Interaction

### Principles

- Purposeful only. Every animation communicates state change.
- Fast. Default 0.25s, max 0.4s.
- Spring for interactive feedback: `spring(response: 0.3, dampingFraction: 0.7)`.
- Ease for fades: `easeInOut(0.2s)`.

### Specific patterns

```
Reminder checked         Circle spring fill 0.3s + strikethrough sweep 0.2s
Card load                Fade + Y-translate 8pt, staggered 0.05s, max 5 items
Error shake              3x horizontal oscillation, 4pt amplitude, 0.3s total
Message sent             Slide up from bottom, 0.2s ease-out
Location pin update      0.5s position interpolation, never jumps
```

### Rules

- Never animate on first load. Initial display is instant.
- Never block interaction for animation.
- Respect Reduce Motion. Replace with instant state changes.

---

## 7. Iconography

**SF Symbols only.** No custom icon assets in V1.

### Sizing

```
CONTEXT                SIZE   WEIGHT     COLOR
──────────────────────────────────────────────────────
Tab bar                24     Regular    Ink-Light / Amber
List item leading      22     Regular    Ink-Mid
Card header            22     Medium     Amber
Inline action          18     Regular    Amber
Empty state            48     Thin       Ink-Faint
Navigation bar         22     Regular    Amber
```

### Key assignments

```
Reminder unchecked           circle
Reminder checked             checkmark.circle.fill
Add                          plus.circle.fill
Location on                  location.fill
Location off                 location.slash
Trip                         airplane
Hotel                        building.2
Calendar event               calendar.badge.clock
Message                      bubble.left.fill
AI / Ask Porch               sparkles
Screenshot parse             camera.viewfinder
Geofence                     mappin.and.ellipse
Family member                person.circle
```

---

## 8. Tone & Voice

### Rules

- Warm but not cute. "Your family" not "Your fam!" No emoji in UI labels.
- Direct. "Add a reminder" not "Would you like to add a reminder?"
- Plain language. "Share your location with family" not "Enable CoreLocation services."
- Button labels are verbs: Add, Share, Save, Send.
- Error messages help: "Couldn't sync. Check your connection and try again."

### Naming conventions (user-facing)

```
FamilyGroup              "Your Family" or "Family"
FamilyMember             person's first name (never "member")
AI feature               "Ask Porch" (never "Claude" or "AI Assistant")
Geofence                 "Place Alert"
LocationSharingLevel     "Location Sharing"
Premium                  "Porch Premium"
SuperPremium             "Porch Premium Plus"
```

Critical: the AI layer is branded as Ask Porch. The underlying model is invisible to the user.

### Date & time

- Recent: "Just now", "5 min ago", "2 hours ago", "Yesterday"
- Older: "Mon, Apr 13", "Apr 13, 2026"
- Time: "7:00 PM" (12-hour, respects system locale)
- Duration: "2 days", "1 week" — never "48 hours"
- Trip ranges: "Apr 13 – 18" same month, "Apr 28 – May 3" cross-month

---

## 9. Example Screens & Patterns

### Widget (medium, 4x2)

The widget is the product for most family members. Zero learning curve. Checkable from the home screen.

```
┌──────────────────────────────────────┐
│ Porch.              Today, Apr 13    │
│                                      │
│ ○  Pick up dry cleaning              │
│ ○  Soccer practice at 4              │
│ ○  Call dentist                      │
│ ────────────────────────             │
│ 📅 Team dinner · 7:00 PM             │
└──────────────────────────────────────┘
```

### Home (app)

Single scroll. Sections: Today's Reminders, Coming Up, Family (location summary), Ask Porch entry. Each section is a card group. Section headers use Label Small uppercase Ink-Light.

### Empty state (Reminders, fresh account)

```
[circle.badge.plus icon, 48pt, Ink-Faint]
Your first reminder
Add something for yourself or your family.
[Add Reminder — Primary]
```

### Permission pre-prompt (before iOS system dialog)

```
[location.fill, 48pt, Amber]
Why Porch needs this
So your family can see when you've arrived home safely.
[Allow — Primary]
[Not Now — Tertiary]
```

Show before the system dialog. Never nag. If declined, show subtle indicator in settings.

### Marketing landing (web)

- Cream background, full-bleed
- Hero: Georgia Display Large headline on left, Porch widget mockup on right
- Single Amber CTA
- Feature triptych below: three cards (Reminders, Location, Trips), each with SF Symbol, Title Medium, Body Medium, tertiary link
- Footer: Ink-Light on Warm, minimal links

### Ask Porch (AI) surface

Sheet at Large detent. Cream background. Message bubbles:
- User: Amber-Pale fill, Ink text, right-aligned, 16pt radius
- Porch: Surface fill, Ink text, left-aligned, 16pt radius, sparkles icon overlay top-left

Never expose "Claude" or the underlying model. The conversation is with Porch.

---

## Accessibility Floor

Non-negotiable. Every screen:

- Touch targets 44x44pt minimum
- WCAG AA contrast (verified for Ink-Light on Cream at 3.8:1 — use only for non-essential metadata)
- VoiceOver labels on every interactive element, descriptive not generic
- Dynamic Type support, tested at max accessibility size
- Reduce Motion replaces animation with instant transitions
- No color-only status indicators — always pair with text or icon

---

## Do / Don't

**Do:** Cream backgrounds. Amber for one accent color only. Georgia for the wordmark. Card-based layouts. SF Symbols. System navigation. Warm, direct copy.

**Don't:** Dark mode (V1). Custom nav bars. Custom tab bars. Secondary accent colors. Emoji in UI labels. Surveillance framing. "AI Assistant" language. Hex literals outside the token system.

---

*Aesthetic Family: Hearth Structured*
*Source: porch.family · iOS spec `/specs/design-system.md` · Version 1.0*
