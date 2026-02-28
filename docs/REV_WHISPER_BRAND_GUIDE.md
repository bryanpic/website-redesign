# Rev Whisper — Complete Brand Identity Guide

> **Purpose**: This document is the single source of truth for the Rev Whisper brand. It is structured for AI consumption — every value is explicit, every rule is stated, and every specification is machine-parseable. Use this document to generate on-brand copy, design assets, UI components, marketing materials, and product interfaces.

---

## Table of Contents

1. [Brand Overview](#1-brand-overview)
2. [Typography System](#2-typography-system)
3. [Color System](#3-color-system)
4. [Logo System](#4-logo-system)
5. [Icon & Symbol](#5-icon--symbol)
6. [Voice & Tone](#6-voice--tone)
7. [Photography & Imagery](#7-photography--imagery)
8. [Iconography System](#8-iconography-system)
9. [Motion & Animation](#9-motion--animation)
10. [Text Emphasis & Annotation Marks](#10-text-emphasis--annotation-marks)
11. [Data & Product Design](#11-data--product-design)
12. [Brand Applications](#12-brand-applications)
13. [Social Media Strategy](#13-social-media-strategy)
14. [Brand Assets Reference](#14-brand-assets-reference)
15. [Website Implementation Analysis](#15-website-implementation-analysis)

---

## 1. Brand Overview

### 1.1 What Rev Whisper Is

Rev Whisper is an intelligent revenue management platform that optimizes listings, drives pricing strategy, and maximizes returns for short-term rental (STR) owners. The company combines proprietary algorithms with a dedicated tech team to optimize every listing, every night, every market — turning data into dollars while owners focus on their guests.

### 1.2 Brand Manifesto

> "We believe every short-term rental deserves smarter pricing. Not guesswork. Not gut feelings. Revenue driven by algorithms that never sleep."

### 1.3 Brand Story

> "Rev Whisper exists because most short-term rental owners leave revenue on the table. We combine proprietary algorithms with a dedicated tech team to optimize every listing, every night, every market, turning data into dollars while you focus on your guests."

### 1.4 Brand Essence (3 Pillars)

| Pillar | Description |
|--------|-------------|
| **Precision** | Every recommendation is backed by data |
| **Intelligence** | Algorithms that learn and adapt |
| **Results** | Measurable revenue impact |

### 1.5 Brand Pillars (What We Deliver)

| Pillar | Description |
|--------|-------------|
| **Algorithms** | Proprietary pricing engine |
| **Optimization** | Continuous listing improvement |
| **Transparency** | Clear reporting, no black boxes |

### 1.6 Brand Quote

> "The best revenue strategy doesn't feel like a strategy at all. It feels like your listing was always priced exactly right."

### 1.7 Tagline

**"An intelligent revenue management platform that optimizes listings, drives pricing strategy, and maximizes returns for short-term rental owners."**

---

## 2. Typography System

### 2.1 Three-Typeface System

Rev Whisper uses a strict three-typeface system. Each typeface has a defined role and must not be used outside that role.

| Role | Primary Typeface | Web Fallback | Classification | Available Weights |
|------|-----------------|--------------|----------------|-------------------|
| **Headlines** | Tiempos (Kris Sowersby / Klim Type Foundry) | `'Lora', 'Georgia', serif` | Serif | 400 (Regular) |
| **Body** | The Future | `'DM Sans', 'system-ui', 'Helvetica Neue', sans-serif` | Geometric Sans-Serif | 200, 300, 400, 500, 600, 700 |
| **Data Display** | DM Mono (Colophon Foundry) | `'DM Mono', 'SF Mono', 'Fira Code', monospace` | Monospace | 300, 400, 500 |

### 2.2 CSS Font Stack Declarations

```css
--heading: 'Lora', 'Georgia', serif;
--body: 'DM Sans', 'system-ui', 'Helvetica Neue', sans-serif;
--mono: 'DM Mono', 'SF Mono', 'Fira Code', monospace;
```

### 2.3 Type Scale

| Level | Size | Line Height | Typeface | Weight | Usage |
|-------|------|-------------|----------|--------|-------|
| Display | 64px | 1.1 | Tiempos / Lora | 400 | Hero headlines, landing pages |
| H1 | 42px | 1.2 | Tiempos / Lora | 400 | Page titles |
| H2 | 28px | 1.3 | Tiempos / Lora | 400 | Section headings |
| Body | 20px | 1.6 | The Future / DM Sans | 400 | Paragraphs, general content |
| Caption | 14px | 1.5 | The Future / DM Sans | 400 | Supporting text, metadata |
| Label | 13px | 1.4 | The Future / DM Sans | 500 | UI labels, form fields, buttons |

### 2.4 Pairing Rules

- **Core pairing**: Tiempos headlines + The Future body. This is the default combination for all layouts.
- **DM Mono is restricted**: Use ONLY for numeric data, chart labels, KPI metrics, and data tables. Never use DM Mono for body copy, headings, or general UI text.
- **Two-typeface maximum per view**: No single screen should show more than two typefaces (excluding DM Mono in data contexts where it appears alongside the core pair).
- **Data typography rule**: "Lora names the metric. DM Mono renders the number. DM Sans handles everything else."

### 2.5 Weight Usage Guidelines

- Headlines always use weight 400 (Regular) — never bold serif headings
- Body copy uses weight 400 for paragraphs, 500 for labels and buttons
- DM Mono uses 400 for data, 300 for secondary data, 500 for emphasized metrics

---

## 3. Color System

### 3.1 Primary Palette

These four colors constitute the core brand palette. All designs must be achievable with only these four colors.

| Name | Hex | RGB | Role | Usage |
|------|-----|-----|------|-------|
| **Dune** | `#32302F` | `rgb(50, 48, 47)` | Primary brand color | Headlines, body text, navigation, icons. Warm near-black. **Never use pure `#000000`** |
| **Fern** | `#4A6741` | `rgb(74, 103, 65)` | Brand accent | "Rev" in wordmark, key CTAs, selective emphasis. **Use sparingly** |
| **White** | `#FFFFFF` | `rgb(255, 255, 255)` | Primary background | Generous white space is a **defining** brand feature |
| **Stone** | `#E0DCDA` | `rgb(224, 220, 218)` | Structural | Dividers, borders, rule lines, subtle backgrounds |

### 3.2 Extended Palette

These colors appear in the master CSS but are secondary to the core four.

| Name | Hex | RGB | Role |
|------|-----|-----|------|
| **Terracotta** | `#8B4A3E` | `rgb(139, 74, 62)` | Extended accent, warm tones |
| **Gold** | `#9B7B3A` | `rgb(155, 123, 58)` | Extended accent, premium/achievement contexts |
| **Background Subtle** | `#F8F7F6` | `rgb(248, 247, 246)` | Alternate section backgrounds |

### 3.3 Chart Color Palette

For data visualizations, use this sequential palette:

| Token | Hex | Usage |
|-------|-----|-------|
| `--chart-1` | `#32302F` | Primary data series |
| `--chart-2` | `#4A6741` | Secondary data series |
| `--chart-3` | `#8B7D6B` | Tertiary data series |
| `--chart-4` | `#A69882` | Fourth data series |
| `--chart-5` | `#6B7F6B` | Fifth data series |
| `--chart-6` | `#C4BDB6` | Sixth data series |

### 3.4 Color Distribution

This is the target ratio for any given layout or screen:

| Color | Percentage |
|-------|-----------|
| White | **70%** |
| Dune | 15% |
| Fern | 10% |
| Stone | 5% |

### 3.5 WCAG Accessibility Compliance

| Combination | Contrast Ratio | WCAG Level |
|-------------|---------------|------------|
| Dune on White | **12.7:1** | AAA |
| Fern on White | **6.4:1** | AA |

### 3.6 Color Philosophy

> The palette is intentionally restrained. Fern is the only true "color" — everything else is neutral. This restraint is what makes Fern powerful when it appears.

### 3.7 CSS Variables (Complete)

```css
:root {
  --dark: #32302F;
  --white: #FFFFFF;
  --light: #E0DCDA;
  --green: #4A6741;
  --terracotta: #8B4A3E;
  --gold: #9B7B3A;
  --bg-subtle: #F8F7F6;
  --dot-color: rgba(50, 48, 47, 0.07);
  --chart-1: #32302F;
  --chart-2: #4A6741;
  --chart-3: #8B7D6B;
  --chart-4: #A69882;
  --chart-5: #6B7F6B;
  --chart-6: #C4BDB6;
}
```

---

## 4. Logo System

### 4.1 Full Lockup Anatomy

The logo consists of three elements arranged horizontally:

1. **Icon**: Speech bubble containing an algorithmic waveform (left)
2. **"Rev"**: Set in Lora Regular, colored Fern (`#4A6741`)
3. **"Whisper"**: Set in Lora Regular, colored Dune (`#32302F`)

The icon sits to the left of the two-tone wordmark. "Rev" is always Fern, "Whisper" is always Dune in the primary variant.

### 4.2 Logo Variants

| Variant | Icon Color | "Rev" Color | "Whisper" Color | Background |
|---------|-----------|-------------|-----------------|------------|
| **Primary** | Dune `#32302F` | Fern `#4A6741` | Dune `#32302F` | White |
| **Monochrome Dune** | Dune | Dune | Dune | White or light backgrounds |
| **Reversed on Dark** | White `#FFFFFF` | White | White | Dune `#32302F` |
| **Reversed on Fern** | White `#FFFFFF` | White | White | Fern `#4A6741` |

### 4.3 Clear Space

**Minimum clear space** = the height of the icon, applied on all four sides of the entire lockup. No other element may enter this zone.

### 4.4 Background Usage Rules

- **White/light backgrounds**: Use Primary or Monochrome Dune variant
- **Dark/Dune backgrounds**: Use Reversed (all white) variant
- **Fern backgrounds**: Use Reversed (all white) variant
- **Never** place the logo on busy imagery without sufficient contrast
- **Never** distort, rotate, add drop shadows, add outlines, or apply any effects to the logo

---

## 5. Icon & Symbol

### 5.1 Brand Icon Description

A speech bubble containing an algorithmic waveform. The speech bubble represents communication and consultation. The interior waveform represents algorithmic data patterns and pricing signals.

### 5.2 SVG Source

```svg
<svg viewBox="0 0 48 48" fill="none" xmlns="http://www.w3.org/2000/svg">
  <path d="M6 20C6 12 12 6 22 6H26C36 6 42 12 42 20C42 28 36 34 26 34H20L12 40V34C8.5 32 6 27 6 20Z"
        stroke="#32302F" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round"/>
  <path d="M15 21C15 21 17 14 19.5 14C22 14 22 28 24.5 28C27 28 27 16 29 16C31 16 32 22 33 22"
        stroke="#32302F" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
</svg>
```

### 5.3 Construction

- **Grid**: 48px x 48px
- **Outer path**: Speech bubble with tail at bottom-left
- **Inner path**: Continuous waveform with 4 peaks/valleys, representing data signals

### 5.4 Icon Variants

| Variant | Stroke Color | Background |
|---------|-------------|------------|
| **Primary** | Dune `#32302F` | White |
| **Monochrome Dune** | Dune `#32302F` | Light backgrounds |
| **Reversed on Dark** | White `#FFFFFF` | Dune `#32302F` |
| **Reversed on Fern** | White `#FFFFFF` | Fern `#4A6741` |

### 5.5 Usage Rules

- **Minimum size**: 32px
- **Clear space**: Height of the icon on all sides
- Never modify the waveform pattern
- Never fill the speech bubble (stroke only)
- Never animate the waveform in the static icon (see Motion section for interaction states)

---

## 6. Voice & Tone

### 6.1 Three Voice Traits

| Trait | Description | Principle |
|-------|-------------|-----------|
| **Confident & Direct** | We state things plainly. No hedging, no qualifiers. If the data says it, we say it. | Assertive without arrogance |
| **Technical & Precise** | "12% revenue increase" over "significant growth." Specificity builds trust. | Numbers over adjectives |
| **Calm & Understated** | We never oversell. Quiet confidence is our signature. Let the numbers speak. | Restraint is strength |

### 6.2 This / Not This Examples

**Example 1 — Reporting Results**:
- **This**: "Your listings earned $12,830 this month. Occupancy is 8% above market average. Here's what's driving performance."
- **Not This**: "Amazing news!! Your listings are absolutely CRUSHING it this month!"

**Example 2 — Making a Recommendation**:
- **This**: "We recommend a 3-night minimum for the upcoming festival weekend. Based on historical data, this could increase your revenue by 15%."
- **Not This**: "Hey there! We think you might want to maybe try increasing your minimum stay?"

### 6.3 Words to Avoid

| Category | Banned Words/Phrases |
|----------|---------------------|
| **Hype Language** | Revolutionary, Game-changing, Disruptive, Crushing it, 10x your revenue, Unlock your potential |
| **Weak/Passive** | We try to, We hope, Might help, A little bit better, We think maybe, Potentially |
| **Overly Casual** | Hey!, Awesome, Super cool, No brainer, Let's gooo, !!! (multiple exclamation marks) |

### 6.4 Product UI Copy Patterns

| Context | Pattern | Example |
|---------|---------|---------|
| **Error Messages** | State what failed + what to do. Under 20 words. No blame. | "We couldn't update pricing for Seaside Villa. Check your Airbnb connection in Settings." |
| **Empty States** | State the current state + single next step. | "No properties connected yet. Add your first listing to start optimizing revenue." |
| **Tooltips** | Define the term + calculation method. | "ADR: Average Daily Rate. Total revenue divided by number of booked nights." |
| **Notifications** | State what happened + specific details. | "Rate adjusted. Seaside Villa increased to $289/night based on weekend demand data." |

### 6.5 Tone Rules

**DO:**
- Lead with data and specifics
- Use active voice and short declarative sentences
- Let the reader draw their own conclusions
- Be helpful and clear without patronizing
- Write at the level of a smart, busy professional

**DON'T:**
- No exclamation marks in product copy
- Don't make promises the data can't support
- No slang, jargon, or startup speak
- Don't apologize unnecessarily (no "Oops!", no "Sorry!")
- Don't use all caps for emphasis
- No "oops" or "uh oh" in error states
- No emoji in product interfaces
- Don't blame the user for errors

### 6.6 Writing Formula

**Two sentences maximum** for any system message:
1. State what happened
2. State what to do about it

---

## 7. Photography & Imagery

### 7.1 Photography Style

Rev Whisper uses AI-optimized property photography showing before/after transformations. This is a core part of the service offering — showcasing how listings look after professional staging and editing.

### 7.2 Photography Guidelines

**DO:**
- Natural light, wide composed shots
- Muted warm color treatment (aligned with the Dune/Stone palette warmth)
- Architectural details and curated staging
- Wide-angle hero shots showing full rooms
- Clean, aspirational interiors

**DON'T:**
- No oversaturated or HDR photography
- No people's faces (privacy and universality)
- No generic stock photos
- No filters outside the brand palette tones
- No cluttered compositions
- No screenshots with test/placeholder data

### 7.3 Product Screenshot Specifications

| Property | Value |
|----------|-------|
| Dimensions | 1440 x 900 |
| Resolution | Retina 2x minimum |
| Format | PNG (no lossy compression) |
| Border | 1px Stone (`#E0DCDA`) |
| Border radius | 8px |
| Shadow | `--shadow-md` (subtle box-shadow) |

---

## 8. Iconography System

### 8.1 Icon Specifications

| Property | Value |
|----------|-------|
| Grid | 24px x 24px |
| Live area | 20px x 20px (2px padding all sides) |
| Stroke width | 2px |
| Line caps | Round |
| Line joins | Round |
| Fill | None (stroke only, always) |
| Default color | Dune `#32302F` |

### 8.2 General UI Icons (48 icons)

`Home` `Dollar Sign` `Activity` `Calendar` `Settings` `Users` `Search` `Bell` `Mail` `MapPin` `Star` `Heart` `BarChart2` `TrendingUp` `Globe` `Lock` `Layers` `Grid` `Clock` `Shield` `Check` `AlertTriangle` `ExternalLink` `Briefcase` `Zap` `Eye` `Filter` `ArrowUpRight` `ArrowDownRight` `Download` `Upload` `Plus` `Minus` `ChevronDown` `ChevronRight` `MoreHorizontal` `X` `Key` `Camera` `Award` `Wifi` `Coffee` `Target` `Archive` `Clipboard` `MessageCircle` `ThumbsUp` `RefreshCw`

### 8.3 Data & Analytics Icons (20 icons)

`PieChart` `Database` `Server` `Cpu` `BarChart` `Activity2` `Sliders` `GitBranch` `Repeat` `Percent` `Hash` `Maximize2` `Minimize2` `ToggleLeft` `Terminal` `Code` `Crosshair` `Compass` `Anchor` `Radio`

### 8.4 Icon Usage Rules

- All icons are inline SVG — never use icon fonts or raster images
- Default rendering: Dune (`#32302F`) stroke on White background
- Icons may be rendered in White on dark backgrounds
- Never fill icons — they are stroke-only
- Maintain the 2px stroke width at all sizes
- Scale proportionally from the 24px base

---

## 9. Motion & Animation

### 9.1 Three Principles

| Principle | Description |
|-----------|-------------|
| **Purposeful** | Nothing moves for decoration. Every animation communicates a state change, provides feedback, or guides attention. |
| **Subtle** | Animations are felt more than seen. If a user notices the animation itself, it's too much. |
| **Consistent** | Same easing curve and duration range across the entire product. |

### 9.2 Duration Scale

| Type | Duration | Examples |
|------|----------|----------|
| Micro-interactions | **150ms** | Toggles, checkboxes, button hover states |
| Element transitions | **250ms** | Cards opening, panels sliding, tooltips appearing |
| Page transitions | **400ms** | Route changes, full-screen transitions |
| **Maximum allowed** | **500ms** | Never exceed this for any animation |

### 9.3 Easing Curves

| Context | Curve | CSS |
|---------|-------|-----|
| Primary (default) | Ease-out | `cubic-bezier(0.25, 0.1, 0.25, 1.0)` |
| Elements entering viewport | Ease-out | Same as above |
| Elements leaving viewport | Ease-in | Reverse of above |
| In-place transforms | Ease-in-out | Symmetric curve |
| **Banned** | Linear | Never use `linear` easing |

### 9.4 CSS Variables

```css
--ease-out: cubic-bezier(0.16, 1, 0.3, 1);
--transition-lift: transform 0.25s var(--ease-out), box-shadow 0.25s var(--ease-out);
```

### 9.5 Standard Entrance Animation

Elements entering the viewport use a combined fade + translate:

```css
/* Start state */
opacity: 0;
transform: translateY(8px);

/* End state */
opacity: 1;
transform: translateY(0);
```

### 9.6 Hover States

- **Duration**: 150ms
- **Buttons**: Darken background-color on hover
- **Cards**: Border color shift on hover
- **No scaling** — never scale elements on hover
- **No bouncing** — never use bounce or spring animations

### 9.7 Motion Rules

**DO:**
- Fade + translate for viewport entry
- Animate `background-color` on hover
- Consistent durations across the product
- Respect `prefers-reduced-motion` media query
- Test at 2x speed to ensure subtlety

**DON'T:**
- No bounce, elastic, or spring easing
- No layout property animations (width, height, top, left — use transform instead)
- No infinite loops or repeating animations
- No motion for purely promotional content
- Never exceed 500ms

---

## 10. Text Emphasis & Annotation Marks

### 10.1 Design Intent

> "Emphasis marks introduce a controlled moment of human texture into an otherwise minimal system. They signal importance, celebrate achievements, and draw the eye — but only when earned."

### 10.2 Three Approved Marks

| Mark | Shape | Usage |
|------|-------|-------|
| **Circle** | Hand-drawn circle enclosing the target element | Primary mark. Draws the eye to a single data point, metric, or key phrase. |
| **Underline** | Hand-drawn underline beneath text | Subtler than circle. Used for quieter emphasis on a single word or short phrase. |
| **Star** | Small hand-drawn star at top-right of element | Reserved **exclusively** for achievement/milestone emphasis. |

**The system is closed** — no other mark types may be invented.

### 10.3 Consistency Specifications

| Property | Value |
|----------|-------|
| Stroke weight | **1.8px** |
| Color | **Fern `#4A6741` ONLY** — no exceptions, no other colors |
| Clearance | 8px minimum around the mark |
| Line caps | Round |
| Rotation | 1–3 degrees maximum (subtle imperfection) |
| Scale | Proportional — circles match enclosed text, underlines match word width, stars fixed at 12–16px |

### 10.4 Hierarchy Rules

| Text Level | Marks Allowed? | Notes |
|------------|---------------|-------|
| Display / H1 | Yes | One technique per heading |
| H2 / Subhead | Yes | Circles around data points preferred |
| Data / Metrics | Yes | Circle = primary, Star = milestones only |
| **Body Copy** | **NO** | Off-limits. Never apply marks to body text. |
| **Labels / Captions** | **NO** | Off-limits. Never apply marks to UI chrome. |

### 10.5 Restraint Rules

1. **One mark per view**: A single screen or card section gets at most one emphasis mark
2. **One word or metric per mark**: Circles enclose one thing. Underlines span one phrase (three words maximum).
3. **Earn the mark**: If the element already has visual weight (large type, color, isolation), a mark is redundant. Only add marks to elements that need the boost.
4. **Never animate emphasis marks**

---

## 11. Data & Product Design

### 11.1 Design Philosophy

| Principle | Description |
|-----------|-------------|
| **Data First** | Every screen starts with the question "What does the owner need to know right now?" |
| **Progressive Disclosure** | Show the headline metric immediately. Details on demand. |
| **Calm Precision** | Dashboards should feel like a well-organized briefing, not a stock trading floor. |

### 11.2 Chart Types & Specifications

All charts use Fern (`#4A6741`) as the primary color at varying opacities. All numeric labels use DM Mono. All gridlines are 0.5px Stone (`#E0DCDA`), dashed.

| Chart Type | Description | Key Spec |
|------------|-------------|----------|
| **Sparkline** | Compact trend line for KPI cards | Fern stroke with gradient fill fading to white. Pulsing endpoint dot. No axis labels. |
| **Bar Chart** | Standard vertical bars | 15% opacity inactive, 100% Fern active/selected. DM Mono value labels above bars. |
| **Line Chart** | Time-series trends | 2px Fern stroke. 25% opacity Fern for comparison lines. Vertical crosshair at current point. |
| **Area Chart** | Cumulative/trend data | Fern stroke with gradient fill below. Percentage delta label at endpoint. |
| **Donut Chart** | Composition data | Single-hue Fern ring at descending opacities. White center with large DM Mono metric. Max 4 segments. |
| **Stacked Bar** | Proportion data | Three Fern opacity layers: 100%, 40%, 12%. |
| **Horizontal Bar** | Ranking data | Fern bars with Stone track backgrounds. Pill-shaped (full border-radius). Descending opacity per rank. |
| **Radial Progress** | Single-metric progress | Fern arc on 8% opacity Stone track. Round linecaps. DM Mono center metric. |
| **Scatter Plot** | Correlation data | Fern dots with opacity encoding density. Dashed trend line. Variable radius for third dimension. |

### 11.3 Chart Rendering Specs

```
Stroke width:    2px
Line caps:       Round
Gridlines:       0.5px, Stone (#E0DCDA), dashed
Numeric labels:  DM Mono
Primary color:   Fern (#4A6741) at varying opacities
```

### 11.4 Product Copy in Data Contexts

**DO:**
- State what happened, then what to do (2 sentences max)
- Use specific property names and numbers
- Keep error messages under 20 words
- Lead with the data point in tooltips

**DON'T:**
- No "oops" or "uh oh"
- No exclamation marks
- No vague phrases ("something went wrong")
- No emoji or casual tone
- Don't blame the user

---

## 12. Brand Applications

### 12.1 Business Card

- **Front**: Logo lockup, name, title, contact information
- **Back**: Icon/symbol centered
- **Paper stock**: Uncoated, warm white
- **Typography**: Lora for name, DM Sans for all other details

### 12.2 Letterhead

- Logo lockup positioned top-left
- Contact information at bottom
- Body text in DM Sans

### 12.3 Email Signature

- Logo lockup (small)
- Name (Lora), title (DM Sans)
- Contact line (DM Sans)
- Fern accent line separator

### 12.4 Social Templates

Platform-specific templates for Instagram, LinkedIn, and X/Twitter using the full brand color system, typography, and layout rules.

### 12.5 Mobile App Screens

Dashboard and listing detail views applying the brand system in a mobile context — same colors, typography, and data visualization patterns scaled for small screens.

---

## 13. Social Media Strategy

### 13.1 Platform Specifications

| Platform | Feed Size | Stories/Vertical Size |
|----------|----------|----------------------|
| Instagram | 1080 x 1080 | 1080 x 1920 |
| LinkedIn | 1200 x 627 (single), 1080 x 1080 (carousel) | — |
| X / Twitter | 1200 x 675 (single), 800 x 418 (in-stream) | — |
| Reddit / FB Groups | 1200 x 628 (link), 1080 x 1080 (image) | — |

### 13.2 Four Content Pillars

| Pillar | Description |
|--------|-------------|
| **Educational** | Industry insights, market analysis, pricing tips |
| **Product** | Features, data showcases, algorithm explanations |
| **Client Results** | Case studies, revenue wins, before/after |
| **Brand Personality** | Behind the scenes, team, culture |

### 13.3 Caption Guidelines

- Confident, data-forward tone
- Lead with the insight, not the setup
- No hype language — matches Voice & Tone section exactly
- Short sentences, active voice
- Hashtags: mix broad reach STR tags with niche community tags

### 13.4 50-Day Content Calendar (4 Phases)

| Phase | Days | Focus |
|-------|------|-------|
| **Foundation** | 1–6 | Origin story, positioning, founder narrative, market context |
| **Pain Points** | 7–15 | Market saturation, amenity arms race, pricing signals, platform mastery |
| **Deep Cuts** | 16–35 | Technical deep dives, pricing algorithms, data visualizations, before/after case studies |
| **Authority** | 36–50 | Thought leadership, client testimonials, revenue showcases, community engagement |

### 13.5 Four Video Series

| Series | Format | Length | Concept |
|--------|--------|--------|---------|
| **The OTA Whisperer** | Alex audits real listings live | 60–90s Reels / 5–10min YouTube | Primary series. 8 episodes outlined. |
| **Data Drop** | Quick market data insights | 30–45s Reels / 2–3min YouTube | Weekly series. 4 episodes outlined. |
| **The $0 Fix** | Free optimization quick wins | Under 60s | Educational. 5 episodes outlined. |
| **Say It Out Loud** | Direct-to-camera industry truths | Under 30s | Engagement/hot takes. 6 episodes outlined. |

### 13.6 Instagram Highlights Structure

| Highlight | Content |
|-----------|---------|
| Who We Are | Company story, mission, team |
| How It Works | Product walkthrough, process |
| The Whisperer | Best clips from video series |
| Results | Revenue wins, case studies |
| Tips | Quick optimization tips |
| FAQ | Common questions answered |

---

## 14. Brand Assets Reference

### 14.1 Available Asset Formats

| Asset | Formats |
|-------|---------|
| Primary Logo Lockup | SVG, PNG, EPS |
| Reversed Logo Lockup | SVG, PNG, EPS |
| Icon / Symbol (standalone) | SVG, PNG, ICO |
| Wordmark Only | SVG, PNG, EPS |
| Lora (headline font) | Google Fonts, OTF, TTF |
| DM Sans (body font) | Google Fonts, OTF, TTF |
| Color Palette | ASE, CLR, PDF |
| Presentation Template | PPTX, Keynote, Google Slides |
| Icon Library | SVG, Icon Font |
| Email Signature | HTML, PNG |

### 14.2 File Usage Rules

**DO:**
- Use SVG for all digital applications
- Use EPS for print production
- Use PNG only when vector formats are not supported
- Export PNG at 2x resolution minimum
- Reference this guide before creating new brand materials

**DON'T:**
- Don't retrace or redraw assets manually
- Don't convert between formats without source files
- Don't use low-resolution assets for print
- Don't distribute brand assets without permissions
- Don't modify colors or proportions of any assets

---

## 15. Website Implementation Analysis

This section documents how the live Rev Whisper website (`/Users/bryan/Coding/website-redesign`) implements the brand system, including alignment with the guidelines and any implementation-specific patterns.

### 15.1 Architecture

- **Stack**: Pure static HTML/CSS/JS — no framework, no build system
- **Deployment**: Vercel with `cleanUrls: true` for extension-free URLs
- **Styling**: All CSS is inline within `<style>` blocks in each HTML file (no external stylesheets)
- **Pages**: `index.html` (landing), `checkout.html` (pricing), `checkout-form.html` (enrollment form), `get-started.html` (lead capture form), `success-a.html` (dark success page), `success-b.html` (light success page)

### 15.2 CSS Variable System (Website)

The website uses slightly different variable names but maps to the same brand values:

```css
:root {
  /* Core brand colors */
  --black: #32302F;          /* = Brand "Dune" */
  --accent: #4A6741;         /* = Brand "Fern" */
  --green: #4A6741;          /* Alias for Fern */
  --accent-light: #dce6d8;   /* Light Fern tint (not in brand guide) */
  --green-bg: #dce6d8;       /* Alias for light Fern tint */

  /* Gray scale */
  --g50: #faf9f8;            /* Lightest gray */
  --g100: #f3f1ef;
  --g200: #e8e4e1;           /* Close to brand "Stone" #E0DCDA */
  --g300: #d5d0cc;
  --g400: #b8b2ab;
  --g500: #948d85;
  --g600: #706a63;
  --g700: #48433f;

  /* Semantic colors */
  --red: #B85252;
  --warn: #9A3F3F;
  --terra: #8B4A3E;          /* = Brand "Terracotta" */
  --gold: #9B7B3A;           /* = Brand "Gold" */

  /* Typography */
  --font-heading: 'Lora', Georgia, serif;      /* Matches brand */
  --font-body: 'DM Sans', system-ui, sans-serif; /* Matches brand */

  /* Layout */
  --radius: 8px;             /* = Brand --radius-md */
  --radius-sm: 6px;          /* = Brand --radius-sm */

  /* Shadows (warm-tinted) */
  --sh-sm: 0 1px 2px rgba(50,48,47,.04), 0 1px 3px rgba(50,48,47,.06);
  --sh: 0 2px 4px rgba(50,48,47,.03), 0 4px 12px rgba(50,48,47,.06);
  --sh-lg: 0 4px 8px rgba(50,48,47,.04), 0 8px 24px rgba(50,48,47,.08);

  /* Animation */
  --ease-out-expo: cubic-bezier(.16,1,.3,1);
  --ease-spring: cubic-bezier(.25,.1,.25,1.4);
}
```

### 15.3 Typography Implementation

- **Headings**: Lora loaded via Google Fonts, weights 400–700
- **Body**: DM Sans loaded via Google Fonts, weights 200–700
- **Hero H1**: `clamp(52px, 8vw, 96px)` — fluid sizing, larger than brand spec Display (64px) at max
- **Section headings**: `clamp(30px, 4vw, 44px)` — fluid sizing around brand H1/H2 range
- **Body text**: 17px–20px range depending on context
- **Letter spacing**: `-0.02em` on headings (tight tracking for elegant feel)

### 15.4 Layout System

| Property | Value |
|----------|-------|
| Container max-width | 1100px (index) / 1120px (checkout) |
| Container padding | `0 28px` (index) / `0 24px` (checkout) |
| Section padding | `100px 0` desktop, `72px 0` mobile |
| Grid system | CSS Grid with responsive collapse |
| Mobile breakpoint | 768px (index/checkout), 640px (forms) |

### 15.5 Component Patterns

**Navigation**: Fixed top bar with `backdrop-filter: blur(12px)` transparency effect, Lora wordmark with "Rev" in Fern and "Whisper" in Dune.

**Buttons (6 variants)**:
1. Primary: Fern background, white text
2. Secondary: Dune background, white text
3. Ghost: Transparent with Dune border
4. Small: Reduced padding variant
5. CTA Arrow: Primary with animated right arrow
6. Disabled: Reduced opacity

**Cards (5 types)**: Feature cards, pricing cards, testimonial cards, metric cards, FAQ accordion items. All use `--radius: 8px`, `--sh` shadow, and lift animation on hover.

**Form Fields**: Full-width inputs with Stone borders, Fern focus ring (`box-shadow: 0 0 0 3px rgba(74,103,65,.13)`), smooth label animations.

**FAQ Accordion**: Chevron rotation animation, smooth max-height transition, Dune text.

### 15.6 Animation Implementation

- **Scroll reveal**: IntersectionObserver-based with staggered delays (`.d1`, `.d2`, `.d3` classes adding 80ms, 160ms, 240ms delays)
- **Entrance**: `opacity: 0` + `translateY(18px)` → `opacity: 1` + `translateY(0)` with 0.7s duration
- **Form steps**: Exit-up / enter-from-below transitions between multi-step form pages
- **Hover lifts**: Cards translate Y -2px with shadow increase on hover
- **Easing**: `cubic-bezier(.16,1,.3,1)` as primary easing (matches brand `--ease-out`)

### 15.7 Brand Alignment Notes

| Area | Alignment |
|------|-----------|
| **Colors** | Exact match — Dune, Fern, Stone, Terracotta, Gold all present |
| **Typography** | Lora + DM Sans matches. DM Mono not yet used on website (no data displays yet) |
| **Spacing** | White-space-forward approach matches 70% white distribution target |
| **Animations** | Subtlety matches brand guidelines. Uses ease-out curves. Respects < 500ms rule. |
| **Voice/Tone** | Website copy is confident, data-forward, no hype language. Matches guidelines. |
| **Photography** | Property images used on site match warm, natural-light style. No faces, no stock. |
| **Logo** | Two-tone wordmark (Fern "Rev" + Dune "Whisper") correctly implemented in nav. |

### 15.8 Shadow System (Design Tokens)

```css
/* Three-tier shadow system — warm-tinted with Dune RGBA base */
--shadow-sm: 0 1px 2px rgba(50, 48, 47, 0.04), 0 1px 3px rgba(50, 48, 47, 0.06);
--shadow-md: 0 2px 4px rgba(50, 48, 47, 0.03), 0 4px 12px rgba(50, 48, 47, 0.06);
--shadow-lg: 0 4px 8px rgba(50, 48, 47, 0.04), 0 8px 24px rgba(50, 48, 47, 0.08);
--shadow-xl: 0 8px 16px rgba(50, 48, 47, 0.05), 0 16px 48px rgba(50, 48, 47, 0.1);
```

### 15.9 Border Radius System

```css
--radius-sm: 6px;    /* Small elements: badges, tags, small buttons */
--radius-md: 8px;    /* Default: cards, inputs, containers */
--radius-lg: 12px;   /* Large containers, modals */
--radius-xl: 16px;   /* Hero elements, large feature cards */
```

---

## Quick Reference Card

For rapid AI consumption, here are the most critical brand values in one place:

```
COLORS
  Primary text:     #32302F  (Dune — warm near-black, NEVER use #000000)
  Brand accent:     #4A6741  (Fern — use sparingly)
  Background:       #FFFFFF  (White — 70% of any layout)
  Borders/dividers: #E0DCDA  (Stone)
  Extended:         #8B4A3E  (Terracotta), #9B7B3A (Gold)

FONTS
  Headlines:  Lora (serif), weight 400, fallback Georgia
  Body:       DM Sans (sans-serif), weight 400/500, fallback system-ui
  Data:       DM Mono (monospace), weight 400, fallback SF Mono

VOICE
  Confident, not arrogant
  Specific, not vague ("12% increase" not "significant growth")
  Calm, not hype (no !!, no ALL CAPS, no emoji)
  2 sentences max for any system message

LOGO
  "Rev" = Fern (#4A6741) + "Whisper" = Dune (#32302F)
  Icon = speech bubble with algorithmic waveform
  Clear space = icon height on all sides
  Minimum icon size = 32px

ANIMATION
  Micro: 150ms  |  Element: 250ms  |  Page: 400ms  |  Max: 500ms
  Easing: cubic-bezier(0.16, 1, 0.3, 1)
  Entrance: opacity 0→1 + translateY(8px→0)
  NO bounce, NO spring, NO infinite loops, NO linear

EMPHASIS MARKS
  Only 3 types: Circle, Underline, Star
  Only in Fern (#4A6741), 1.8px stroke
  One mark per view, one word per mark
  Never on body copy
```
