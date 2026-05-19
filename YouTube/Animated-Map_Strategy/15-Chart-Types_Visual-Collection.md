## Which YouTube Channels Became Famous Through Each Format

> Each entry includes a live SVG preview, the channels that made the format iconic, production specs, and the key rule.

---

## 1. Horizontal Bar Chart

**Made iconic by:** Wendover Productions, Vox

```
Channel signature: Wendover's "off-screen bar" — the leading bar exits
the right edge of the frame. Most screenshotted moment in the channel's history.
```

**Preview:**

```
  USA    ████████████████████████████████████  85%
  Germany ████████████████████          62%
  Japan   ████████████████              48%
  Brazil  ██████████████                34%
  India   ████████████████████████████████████████████ 120% ←exits frame
```

**Specs:** Bar height 32px · gap 10px · primary `#2563EB` · accent `#F59E0B` one bar only · sort descending always

**The rule:** All bars one color. One accent bar maximum. Never rainbow. The viral trick: let the leading bar exit the frame.

---

## 2. Animated Line Chart

**Made iconic by:** Veritasium, Our World in Data, 3Blue1Brown

```
Channel signature: Our World in Data draws lines left-to-right in sync
with the narrator. The line is never shown complete before the story ends.
```

**Preview:**

```
100% ┤
 75% ┤         ╭──────────────── main trend (#2563EB, 2.5px)
 50% ┤    ╭────╯
 25% ┤╭───╯  - - - - - - - - -  benchmark (#B4B2A9, 1.5px dashed)
  0% ┼────────────────────────▶
     2000        2012        2024
```

**Specs:** Main line `#2563EB` 2.5px · benchmark `#B4B2A9` 1.5px dashed `4 4` · gridlines opacity 0.15 · no Y-axis · accent point circle r=5

**The rule:** One accent point maximum. Line draws in real time with narration — never pre-loaded.

---

## 3. Slope Chart

**Made iconic by:** Vox, Wendover Productions, The Economist

```
Channel signature: Vox uses slope charts for "who won, who lost" stories.
One red line falling, one blue line rising — story told before the narrator finishes.
```

**Preview:**

```
2000                    2024
  │                       │
  ●──────────────────────● Norway   (+12%) ← blue #2563EB
  │                       │
  │   ●───────────────●   Germany  (+3%)  ← gray #B4B2A9
  │                       │
  ●───────────────────────────●  Argentina (-23%) ← red #EF4444 exits down
```

**Specs:** Growth `#2563EB` 2px · decline `#EF4444` 2px · neutral `#B4B2A9` 1px · dots r=4 · two axes only

**The rule:** 1–2 colored lines (the story), all others gray (context). Red = down only, never for decoration.

---

## 4. Choropleth Map

**Made iconic by:** RealLifeLore, Vox, Wendover Productions

```
Channel signature: RealLifeLore zooms from global → regional in 2 seconds.
The map appears before the narrator explains — geographic orientation first.
```

**Preview:**

```
  ┌─────────────────────────────┐
  │ ░░░░ ▒▒▒▒ ▓▓▓▓ ████ ████  │  ← single-hue sequential scale
  │ ░░░░ ▒▒▒▒ ████ ████ ▒▒▒▒  │
  │ ░░░░ ░░░░ ▒▒▒▒ ▓▓▓▓ ████  │
  └─────────────────────────────┘
  [low]──────────────────[high]   ← legend always horizontal below map
```

**Specs:** Single-hue ramp only (never red-green) · country borders 0.5px white · ocean `#F1F5F9` light / `#111827` dark · zoom animation 2s

**The rule:** Map appears BEFORE explanation. Labels only for countries mentioned in narration. Never red-green (colorblind).

---

## 5. Icon Array (Unit Chart)

**Made iconic by:** Kurzgesagt — their most distinctive format

```
Channel signature: Dark background #0d1117, yellow active icons #FBBE00.
"1 in 4 people" shown as 25 yellow circles out of 100. Emotionally 3× stronger than pie.
```

**Preview:**

```
  1 in 4 people

  ● ● ● ● ● ● ● ● ● ●   ← #FBBE00 yellow (active)
  ● ● ● ● ● ● ● ● ● ●
  ● ● ● ● ● ○ ○ ○ ○ ○   ← #1e293b dark (inactive)
  ○ ○ ○ ○ ○ ○ ○ ○ ○ ○
  ○ ○ ○ ○ ○ ○ ○ ○ ○ ○
```

**Specs:** Active `#FBBE00` (or `#EF4444` for risk) · inactive `#D3D1C7` · size 16×16px · 10 per row · gap 4px · fills top-left first

**The rule:** Sequential fill from top-left always. Large number displayed alongside. Never scatter randomly.

---

## 6. Timeline

**Made iconic by:** Wendover Productions, ColdFusion, Johnny Harris

```
Channel signature: Wendover's timeline nodes appear at exact moment
narrator says the date — not a millisecond before. The animation IS the format.
```

**Preview:**

```
       ●─────────────────●─────────────────◉─────────────────●
     2015               2018             2021               2024
    "Founded"          "IPO"          "$1T cap"           "Crisis"
                                      ↑ accent node #F59E0B r=11
```

**Specs:** Axis `#2563EB` 2px · standard node r=8 `#2563EB` · accent node r=11 `#F59E0B` · labels alternate above/below

**The rule:** One accent node maximum (the pivot of the story). Nodes appear exactly when narrator names the date.

---

## 7. Area Chart

**Made iconic by:** Our World in Data, The Economist

```
Channel signature: Our World in Data uses nearly transparent fills (12% opacity)
to show volume without blocking the lines beneath.
```

**Preview:**

```
  100% ┤
   75% ┤    ╭────────────────────────────  #10b981 fill 8%
   50% ┤╭───╯╭──────────────────────────  #2563EB fill 12%
   25% ┤│    │
    0% ┼─────────────────────────────────▶
```

**Specs:** Primary fill `#2563EB` 12% opacity · secondary fill `#10b981` 8% · lines 2px and 1.5px · max 2 layers · legend embedded

**The rule:** Fill is nearly transparent — suggests volume, doesn't block. Two layers need two distinct color families.

---

## 8. Donut Chart

**Made iconic by:** Vox, The Economist, Bloomberg

```
Channel signature: Vox uses thin-ring donuts (68% cutout) with the dominant
percentage in the center. Used only when one segment clearly leads.
```

**Preview:**

```
         ╭──────────────────╮
      ╭──╯ ████████████████ ╰──╮
     │  ╭─╯ ██ 62% ██████ ╰─╮  │
     │  │      62%           │  │  ← center: number + label
     │  │    market          │  │
     │  ╰─╮ ████████████ ╭─╯  │
      ╰──╮ ████████████ ╭──╯
         ╰──────────────────╯
```

**Specs:** Cutout 68% · dominant `#2563EB` · others lighter same ramp · gap 3px white · max 4 segments · legend right with %

**The rule:** Only when one segment dominates. More than 4 segments → use horizontal bar instead.

---

## 9. Scatter / Bubble Chart

**Made iconic by:** Our World in Data, New York Times, Hans Rosling (Gapminder)

```
Channel signature: Our World in Data's GDP vs Life Expectancy chart —
bubbles sized by population, colored by region, trend line dashed.
Only 3–4 country labels maximum.
```

**Preview:**

```
  Life exp ↑
   85 ┤                              ◉ Norway
   80 ┤              ● ●  Germany ●
   75 ┤      ●  ● ●
   70 ┤  ●●●
   65 ┤●
      └────────────────────────────▶ GDP per capita
                      trend line - - - - -
```

**Specs:** Bubbles by region color · opacity 0.55–0.65 · min r=4 max r=20 · trend line `#64748B` 1px dashed · label only 3–4 outliers

**The rule:** Never label all bubbles. The trend line is optional — only if correlation is the story.

---

## 10. Sankey / Flow Diagram

**Made iconic by:** Wendover Productions, Real Engineering, The Economist

```
Channel signature: Wendover uses Sankey for logistics and money flows.
Flow width = volume. Amber highlight on the key path. Dark background.
```

**Preview:**

```
  Oil ██████████╮
                 ╰████████████╮─── Refinery ████── Transport ██── Consumer
  Gas ████████╮                │
               ╰───────────────╯
  Coal ████╮                         (width = volume)
            ╰─────────────────────── Power plant ██── Grid ████── Consumer
```

**Specs:** Background `#0B1426` · primary flow `#2563EB` 70% · accent path `#F59E0B` 85% · nodes same color as exiting flows

**The rule:** Width strictly proportional to value. Max 3 colors. Amber for the one path the viewer must follow.

---

## 11. Diverging Bar Chart

**Made iconic by:** FiveThirtyEight, The Economist, Pew Research

```
Channel signature: FiveThirtyEight uses diverging bars for polling data.
Red extends left (against), blue extends right (in favor). Zero line is the hero.
```

**Preview:**

```
  against ←          → in favor
  Austria  ████ │ ██████████████████
  France   ██████████ │ ████████
  Canada   ███████ │ ████████████
  Brazil   ████████████████ │ █████
                  │ ← zero line (the most important element)
```

**Specs:** Positive `#2563EB` right · negative `#EF4444` left · center axis 1px `#64748B` · same scale both sides

**The rule:** Zero line labeled explicitly. Both sides identical scale. Use only for genuinely symmetric data.

---

## 12. Small Multiples

**Made iconic by:** New York Times, The Pudding, ProPublica

```
Channel signature: NYT's small multiples show "same crisis, different countries"
in one frame. Every panel identical scale. One panel highlighted = what narrator explains now.
```

**Preview:**

```
  ┌──────┐ ┌──────┐ ┌──────┐
  │Germany│ │France│ │Japan │
  │  /╲  │ │ /╲   │ │  /╲  │  ← identical scale across ALL panels
  └──────┘ └──────┘ └──────┘
  ┌──────┐ ┌──────┐ ┌──────┐
  │Spain │ │Canada│ │Brazil│
  │╱╲    │ │  /╲  │ │   /╲ │  ← highlighted panel = current narration
  └──────┘ └──────┘ └──────┘
```

**Specs:** 3×N or 4×N grid · shared fixed axis scale · same color all panels · accent panel outlined · label 11px above each

**The rule:** Identical axis scale across all panels — non-negotiable. Max 12 panels.

---

## 13. Heatmap / Matrix

**Made iconic by:** New York Times, Axios, Bloomberg

```
Channel signature: NYT's "when Americans sleep" heatmap — hour × day of week.
Single-hue blue scale. Darkest = most activity. Instantly scannable pattern.
```

**Preview:**

```
       M    T    W    T    F    S    S
  6am  ░░   ░░   ░░   ░░   ░░   ▒▒   ▒▒
  12pm ▒▒   ▓▓   ████ ████ ▓▓   ▒▒   ░░
  6pm  ████ ████ ████ ████ ████ ▒▒   ░░
  12am ▒▒   ▒▒   ▒▒   ▒▒   ▒▒   ████ ████

  [low]─────────────────────────────[high]
```

**Specs:** Single-hue ramp `#DBEAFE` → `#1E40AF` · cell min 20×20px · 1px white gap · no-data `#F3F4F6` · horizontal legend below

**The rule:** Single hue only — never rainbow. Darkest = highest. Legend always present.

---

## 14. Pie Chart

**Used sparingly by:** Most channels avoid it. Vox uses max 3 slices.

```
Channel signature: No channel is famous for pie charts — the opposite is true.
Kurzgesagt, Wendover, and Vox all prefer icon arrays or bar charts.
Pie is included here as a reference for when it is the only correct choice.
```

**Preview:**

```
         ╭──────────────────────╮
      ╭──╯ ██████████████████   ╰──╮
     │  ╭─╯    65%             ╰─╮  │   ← only if one segment >50%
     │  │                        │  │
     │  ╰─╮      25%          ╭─╯  │   ← max 3 slices total
      ╰──╮  ████████████████ ╭──╯
         ╰──────╮10%╭──────╯
```

**Specs:** Max 3 segments · labels outside with leader lines · never 3D · never exploded · dominant segment `#2563EB`

**The rule:** Ask first — does one segment clearly dominate? If no → use horizontal bar. If yes → consider donut instead.

---

## 15. Mechanism Diagram (Illustrative)

**Made iconic by:** Kurzgesagt, Real Engineering, Branch Education

```
Channel signature: Kurzgesagt's immune system explainers, Real Engineering's
engine cross-sections. Flat iconographic style, dark background, max 5 elements,
each appearing exactly when narrator names it.
```

**Preview:**

```
  ┌─────────────────────────────────────────┐  ← dark #0d1117 background
  │                                         │
  │       ┌──────────┐                      │
  │       │  FPSO    │──────────→ tanker    │  ← #10b981 flow line
  │       │  vessel  │                      │
  │       └────┬─────┘                      │
  │            │ ↓ amber dashed             │
  │            ● oil well (seabed)          │  ← #F59E0B accent
  │                                         │
  └─────────────────────────────────────────┘
  max 5 elements · flat style · no 3D · labels outside
```

**Specs:** Background `#0d1117` · max 5 elements · flat iconographic · 2–3 colors · labels outside with 0.5px leaders · each element appears on narration cue

**The rule:** Voice and visual carry different information. Diagram shows "what," voice explains "why." If diagram makes sense without audio — the voice is redundant.

---

## Quick Reference

| # | Chart Type | Made Iconic By | Best For | Viral Potential |
|---|-----------|----------------|---------|----------------|
| 1 | Horizontal bar | Wendover Productions | Rankings, comparisons | ★★★★★ |
| 2 | Animated line | Veritasium, Our World in Data | Trends over time | ★★★★ |
| 3 | Slope chart | Vox | Before/after change | ★★★★ |
| 4 | Choropleth map | RealLifeLore, Vox | Geographic distribution | ★★★★ |
| 5 | Icon array | Kurzgesagt | Risk, "1 in N" | ★★★★★ |
| 6 | Timeline | Wendover, ColdFusion | Chronological history | ★★★ |
| 7 | Area chart | Our World in Data | Volume over time | ★★★ |
| 8 | Donut chart | Vox, The Economist | Dominant segment | ★★ |
| 9 | Scatter / bubble | Our World in Data, NYT | Relationships, outliers | ★★★ |
| 10 | Sankey / flow | Wendover, Real Engineering | Systems and flows | ★★★★ |
| 11 | Diverging bar | FiveThirtyEight, Pew | Two opposing sides | ★★★ |
| 12 | Small multiples | NYT, The Pudding | Same pattern, many categories | ★★★ |
| 13 | Heatmap | NYT, Axios | Two-dimensional patterns | ★★★ |
| 14 | Pie chart | No channel — avoid | Dominant segment only | ★ |
| 15 | Mechanism diagram | Kurzgesagt, Real Engineering | How things work | ★★★★★ |

---

## The One Universal Rule

> Before publishing any chart frame: remove the audio and watch the first 60 seconds.
> Does the visual story make sense without sound?
> **If yes — the voice is redundant.**
> **If no — the pairing is correct.**

---

*Visual reference for YouTube educational channel production.*
*Channels analyzed: Kurzgesagt · Wendover Productions · Vox · Our World in Data · The Pudding · 3Blue1Brown · RealLifeLore · Johnny Harris · Real Engineering · FiveThirtyEight · The Economist · NYT Graphics.*

---

## 16. Card Infographic

**Made iconic by:** Kurzgesagt, Vox

```
Channel signature: Kurzgesagt uses card infographics between animation scenes
as "fact frames" — 4–6 seconds on screen, one number per card, three cards per row.
Dark background, colored top bar encodes the topic, large bold number, icon circle.
```

**Preview:**

```
  ┌──────────────────────┐  ┌──────────────────────┐  ┌──────────────────────┐
  ██████████████████████    ████████████████████████    ██████████████████████
  │  (blue accent bar)   │  │  (green accent bar)  │  │  (amber accent bar)  │
  │                      │  │                      │  │                      │
  │       ╭────╮         │  │       ╭────╮         │  │       ╭────╮         │
  │       │ ic │         │  │       │ ic │         │  │       │ ic │         │
  │       ╰────╯         │  │       ╰────╯         │  │       ╰────╯         │
  │                      │  │                      │  │                      │
  │        8.1B          │  │         44%          │  │        11.6B         │
  │   world population   │  │    GDP growth 2024   │  │  barrels of oil      │
  │   +800M since 2015   │  │  fastest in the world│  │  Stabroek Block      │
  └──────────────────────┘  └──────────────────────┘  └──────────────────────┘
```

**Specs:**

| Element | Value |
|---------|-------|
| Background | `#0d1117` |
| Card fill | `#111827` |
| Card border | 0.5px, same color as accent |
| Accent top bar | 6px height, full card width |
| Icon circle | r=22, dark fill matching accent |
| Main number | 26px, weight 700, accent color |
| Primary label | 10px, `#94a3b8` |
| Secondary label | 9px, `#475569` muted |
| Cards per row | 3 maximum |
| Hold time | 4–6 seconds |

**Color logic for accent bars:**

| Topic | Accent color | When |
|-------|-------------|------|
| Population / scale | `#2563EB` blue | Size, counts, geography |
| Growth / positive | `#10b981` green | GDP, improvement, success |
| Resources / warning | `#F59E0B` amber | Oil, energy, caution |
| Risk / decline | `#EF4444` red | Loss, danger, falling |

**The rule:** One card = one number = one insight. Never put two numbers on one card. The icon is decorative — the number is the information. Cards appear together, not one by one.

---

## 17. Pull-Quote Card

**Made iconic by:** Johnny Harris, Wendover Productions, Vox

```
Channel signature: Johnny Harris overlays pull-quotes directly on b-roll.
Left border color encodes the speaker's role: amber = provocation,
blue = authority/institution. Attribution always below in small sans-serif.
Quote text in serif italic — never in the same font as the rest of the video.
```

**Preview:**

```
  ┌─────────────────────────────────────────────────────────────────────────┐
  ▌  "What gives you the right to lecture us about climate change?"         │
  ▌                                                                         │
  ▌  — Irfaan Ali, President of Guyana · BBC HARDtalk, March 2024          │
  └─────────────────────────────────────────────────────────────────────────┘
  ↑ 4px amber left border = provocative / emotional quote

  ┌─────────────────────────────────────────────────────────────────────────┐
  ▌  "The Stabroek Block is a trillion-dollar opportunity."                 │
  ▌                                                                         │
  ▌  — ExxonMobil Production Division · Fortune, August 2024               │
  └─────────────────────────────────────────────────────────────────────────┘
  ↑ 4px blue left border = institutional / authoritative quote
```

**Specs:**

| Element | Value |
|---------|-------|
| Background | `#0f172a` or semi-transparent over b-roll |
| Card fill | `#111827` |
| Left border | 4px, accent color — the only structural color |
| Quote text | Serif italic, 15px, `#f1f5f9` |
| Attribution | Sans-serif, 11px, `#64748b` |
| Attribution format | `— Name, Title · Publication, Date` |
| Hold time | 6–10 seconds |
| Max quote length | 2 lines — longer quotes lose the viewer |

**Border color logic:**

| Color | Meaning | Use for |
|-------|---------|---------|
| `#F59E0B` amber | Provocation, tension | Politicians, activists, controversial statements |
| `#2563EB` blue | Authority, data | Institutions, scientists, official reports |
| `#10b981` green | Hope, positive | Progress, solutions, optimistic projections |
| `#EF4444` red | Warning, crisis | Emergency statements, alarming facts |

**The rule:** Attribution always includes four elements: name, title, source, date. Serif italic for quote text is non-negotiable — it signals "this is a direct quote" without needing quotation mark graphics.

---

## 18. Summary Frame — "3 Things"

**Made iconic by:** Kurzgesagt, Vox, TED-Ed

```
Channel signature: The final frame before the outro. No data — only conclusions.
Three equal cards. The center card carries the main insight and gets an accent border.
Appears for 8–12 seconds while narrator delivers the closing question.
```

**Preview:**

```
                         WHAT WE LEARNED

  ┌──────────────────┐  ┌──────────────────┐  ┌──────────────────┐
  │                  │  ║                  ║  │                  │
  │      ① blue      │  ║  ② amber ★★★   ║  │      ③ green     │
  │                  │  ║  accent border   ║  │                  │
  │  Scale is        │  ║  The deal        ║  │  Two paths       │
  │  everything      │  ║  matters most    ║  │  ahead           │
  │                  │  ║                  ║  │                  │
  │  11.6B barrels   │  ║  Guyana gets     ║  │  Norway model:   │
  │  discovered in   │  ║  ~25% of value   ║  │  save & diversify│
  │  9 years         │  ║  — set before    ║  │  — or spend fast │
  │                  │  ║  the boom        ║  │  and face curse  │
  └──────────────────┘  └──────────────────┘  └──────────────────┘

                    ↑ center card always = the KEY INSIGHT
```

**Specs:**

| Element | Value |
|---------|-------|
| Background | `#0d1117` |
| Card fill | `#111827` |
| Card 1 & 3 border | 0.5px `var(--color-border-tertiary)` — neutral |
| Card 2 border | 1.5px accent color — the insight |
| Number circle | r=18, dark fill matching card accent |
| Number | 16px, weight 600, accent color |
| Card title | 12px, weight 500, `#e2e8f0` |
| Card body | 10px, `#64748b`, max 4 lines |
| Header label | 12px, `#475569`, letter-spacing 3px, uppercase |
| Hold time | 8–12 seconds |
| After this frame | B-roll + open question — never another chart |

**Structure logic:**

```
Card 1 (left)   = Context — what happened / the scale
Card 2 (center) = The KEY INSIGHT — what it means ← accent border here
Card 3 (right)  = The open question — what comes next
```

**The rule:** No data on this frame — only conclusions in plain language. The center card carries the one thing the viewer must remember. This frame appears once per video, always last before the outro. After this: b-roll, no charts.

---

## Updated Quick Reference (18 Formats)

| # | Format | Made Iconic By | Purpose | Hold Time |
|---|--------|----------------|---------|-----------|
| 1 | Horizontal bar | Wendover | Rankings | 10–20 sec |
| 2 | Animated line | Veritasium, OWID | Trends | 20–30 sec |
| 3 | Slope chart | Vox | Before/after | 10–15 sec |
| 4 | Choropleth map | RealLifeLore | Geography | 15–25 sec |
| 5 | Icon array | Kurzgesagt | Risk / "1 in N" | 5–8 sec |
| 6 | Timeline | Wendover | Chronology | 15–25 sec |
| 7 | Area chart | Our World in Data | Volume | 15–20 sec |
| 8 | Donut chart | Vox, Economist | Composition | 6–10 sec |
| 9 | Scatter / bubble | OWID, NYT | Relationships | 15–20 sec |
| 10 | Sankey / flow | Wendover | Systems | 20–30 sec |
| 11 | Diverging bar | FiveThirtyEight | Two sides | 10–15 sec |
| 12 | Small multiples | NYT, Pudding | Many categories | 15–25 sec |
| 13 | Heatmap | NYT, Axios | Patterns | 10–15 sec |
| 14 | Pie chart | Avoid — max 3 slices | Dominant segment | 5–8 sec |
| 15 | Mechanism diagram | Kurzgesagt | How it works | 20–30 sec |
| 16 | Card infographic | Kurzgesagt, Vox | Key stats | 4–6 sec |
| 17 | Pull-quote card | Johnny Harris | Direct quotes | 6–10 sec |
| 18 | Summary "3 things" | Kurzgesagt, Vox | Final conclusions | 8–12 sec |

---

*Document updated with formats 16–18: card infographic, pull-quote card, and summary frame.*
*Total: 18 production-ready visual formats with channel attribution and hold time specifications.*

---

## 19. European & German Market Visual Conventions

**Why this matters:** Evergreen channels targeting European audiences use different visual conventions than US-first channels. Simplicissimus, Kurzgesagt (DE), and NEO Magazin have built loyal audiences by adapting these conventions deliberately.

### Key differences from US-style channels

| Element | US channels (Vox, Wendover) | European evergreen channels |
|---------|----------------------------|----------------------------|
| Color temperature | Cool blues, high contrast | Warmer, slightly desaturated |
| Information density | One insight per frame | Slightly denser — audience tolerates more |
| Data source display | Small caption, bottom corner | More prominent — European audiences expect it |
| Typography | Sans-serif throughout | Mix of sans + occasional serif for gravitas |
| Map style | Flat, minimal borders | More geographic detail, terrain visible |
| Narration pace | ~160 words/min (fast) | ~140 words/min (deliberate) |
| B-roll style | Cinematic, wide shots | More archival, documentary feel |

### Channels that built evergreen libraries through European visual style

**Kurzgesagt (German version — Dinge Erklärt)**
- Same format as English, but narration pace slower
- More explicit sourcing on-screen (German audiences expect Quellenangabe)
- Color palette slightly warmer — less neon, more amber and teal
- Evergreen topics: biology, physics, existential questions, climate

**Simplicissimus**
- Dark background, white typography, minimal animation
- Strong on data cards — German economic data presented as clean numbers
- Evergreen topics: German economic history, social systems, infrastructure

**Real Engineering (Ireland — European sensibility)**
- Technical diagrams with more detail than US equivalents
- Engineering cross-sections as primary format
- Evergreen topics: aviation, energy systems, infrastructure megaprojects

### Visual spec adjustments for European evergreen content

| Parameter | US standard | European evergreen adjustment |
|-----------|-------------|-------------------------------|
| Primary blue | `#2563EB` | `#1d4ed8` — slightly deeper, more serious |
| Source credit | 11px bottom corner | 12px, more visible, format: "Quelle: World Bank 2024" |
| Narration silence on key number | 2 seconds | 2.5–3 seconds — let it land |
| Map detail level | Country outlines only | Country + major rivers/terrain when relevant |
| Grid line opacity | 0.15 | 0.18 — slightly more visible |

---

## 20. Production Budget per Format

**The most practical table in this document.** Evergreen channels like Wendover and Kurzgesagt invest heavily upfront because each video generates views for years. Budget accordingly.

### Time investment (hours per format, experienced editor)

| Format | After Effects | Research & data | Total per video |
|--------|--------------|-----------------|----------------|
| Card infographic (×3) | 1–2 hrs | 0.5 hrs | 2–3 hrs |
| Pull-quote card | 0.5 hrs | 0.5 hrs | 1 hr |
| Summary "3 things" | 1 hr | 1 hr | 2 hrs |
| Horizontal bar chart | 2–3 hrs | 1–2 hrs | 3–5 hrs |
| Animated line chart | 2–3 hrs | 1 hr | 3–4 hrs |
| Timeline | 3–4 hrs | 2 hrs | 5–6 hrs |
| Choropleth map | 4–6 hrs | 2–3 hrs | 6–9 hrs |
| Slope chart | 2–3 hrs | 1 hr | 3–4 hrs |
| Mechanism diagram | 6–12 hrs | 3–4 hrs | 9–16 hrs |
| Sankey / flow | 8–12 hrs | 3–5 hrs | 11–17 hrs |
| Icon array | 1–2 hrs | 0.5 hrs | 1.5–2.5 hrs |
| Small multiples | 4–6 hrs | 2–3 hrs | 6–9 hrs |

### Typical full video production budget (evergreen quality)

| Channel tier | Visuals budget | Total production | Expected lifespan |
|-------------|----------------|-----------------|-------------------|
| Solo creator (starting) | 20–40 hrs | 60–80 hrs | 2–3 years views |
| Small team (2–3 people) | 40–60 hrs | 80–120 hrs | 3–5 years views |
| Wendover / Kurzgesagt level | 100–200 hrs | 200–400 hrs | 5–10 years views |

### Priority order for evergreen channels (start here, expand later)

**Phase 1 — Master first (low cost, high impact):**
Horizontal bar · Card infographic · Pull-quote card · Animated line · Summary frame

**Phase 2 — Add when team is stable:**
Timeline · Choropleth map · Slope chart · Icon array

**Phase 3 — Invest when revenue supports it:**
Mechanism diagram · Sankey · Small multiples · Scatter/bubble

---

## 21. Topic → Format Matrix for Evergreen Content

**How to use:** Find your video topic in the left column. The matrix shows which formats are essential, which add depth, and which to avoid for that topic type.

### Economics & finance (Wendover, Our World in Data)

| Format | Role |
|--------|------|
| Horizontal bar | Essential — comparisons between countries/companies |
| Animated line | Essential — GDP growth, debt levels over time |
| Slope chart | Essential — who won, who lost over a decade |
| Choropleth map | Strong — regional economic distribution |
| Sankey / flow | Strong — how money moves through a system |
| Card infographic | Strong — key stats ($47T GDP, 8% growth) |
| Donut chart | Optional — budget breakdown, ownership structure |
| Scatter / bubble | Optional — GDP vs. happiness, income vs. life expectancy |
| Pie chart | Avoid |

### Geography & geopolitics (RealLifeLore, Wendover)

| Format | Role |
|--------|------|
| Choropleth map | Essential — multiple maps per video |
| Annotated map | Essential — borders, disputed territories |
| Flow map | Essential — trade routes, migration, military |
| Timeline | Strong — historical context of current situation |
| Slope chart | Strong — power shifts between nations |
| Horizontal bar | Strong — military budgets, population comparisons |
| Mechanism diagram | Optional — how a system (port, canal, pipeline) works |
| Donut chart | Avoid — too simple for geopolitical complexity |

### Science & technology (Kurzgesagt, Real Engineering, Veritasium)

| Format | Role |
|--------|------|
| Mechanism diagram | Essential — how the technology works |
| Animated line | Essential — exponential growth curves |
| Icon array | Essential — risk statistics, "1 in N" facts |
| Card infographic | Essential — key numbers between explanations |
| Timeline | Strong — history of the technology |
| Scatter / bubble | Optional — performance comparisons |
| Choropleth map | Optional — where the technology is deployed |
| Sankey / flow | Optional — energy systems, data flows |

### History & society (Johnny Harris, ColdFusion)

| Format | Role |
|--------|------|
| Timeline | Essential — chronological backbone |
| Pull-quote card | Essential — primary sources, eyewitness accounts |
| Annotated map | Essential — where events happened |
| B-roll + number card | Essential — scale of historical events |
| Slope chart | Strong — before/after policy or war |
| Small multiples | Strong — same event across different countries |
| Horizontal bar | Optional — comparative statistics |
| Sankey | Optional — how resources moved |

### Climate & environment (Our World in Data, Kurzgesagt)

| Format | Role |
|--------|------|
| Animated line | Essential — temperature anomaly, CO₂ over time |
| Choropleth map | Essential — regional impact distribution |
| Icon array | Essential — risk to human populations |
| Area chart | Essential — cumulative emissions |
| Card infographic | Strong — key climate numbers |
| Scatter / bubble | Strong — emissions vs. development |
| Diverging bar | Strong — above/below baseline temperature |
| Slope chart | Optional — country-by-country progress |

---

## 22. Thumbnail Strategy for Evergreen Topics

**Why thumbnails matter more for evergreen:** A news channel's thumbnail is relevant for 48 hours. An evergreen channel's thumbnail generates clicks for 3–5 years. It must work at every point in that lifespan — not just on launch day.

### The evergreen thumbnail formula

```
  ┌──────────────────────────────────────────────────────────┐
  │                                                          │
  │   [LARGE NUMBER or GEOGRAPHIC IMAGE]   [3–5 WORD TEXT]  │
  │                                                          │
  │   60% of frame = visual           40% = text/contrast   │
  │                                                          │
  └──────────────────────────────────────────────────────────┘
```

**What works for each evergreen topic:**

| Topic type | Left 60% | Right 40% | What to avoid |
|-----------|---------|---------|--------------|
| Economics | Large number ($47T) or chart fragment | "Why X happened" | Full charts (unreadable at thumbnail scale) |
| Geography | Satellite or political map | Country name + question | Maps with too many labels |
| Science | Mechanism illustration | Short factual claim | Abstract art |
| History | Archival photo or map | Date + "what happened" | Cluttered timelines |
| Climate | Before/after visual | The key number | Doom framing (reduces clicks) |

### Thumbnail specs for evergreen channels

| Parameter | Spec |
|-----------|------|
| Canvas | 1280×720px |
| Safe text zone | Left 40% or right 40% — not both |
| Primary number/text | 80–100px, weight 700, high contrast |
| Background | Photo or solid dark — never gradient |
| Max text | 5 words |
| Mobile check | Must read at 120×68px |
| Color | One accent color matching channel system |
| Face | Present in 60–70% of top-performing evergreen thumbnails |

### Evergreen thumbnail mistake to avoid

**The "news thumbnail" trap:** Many new channels design thumbnails for the moment of upload — using references that only make sense in the week of publication. An evergreen thumbnail must make sense to someone discovering the video two years later with no prior context.

**Test:** Show your thumbnail to someone with no context. Can they tell: (1) what country or topic it's about, (2) why it's interesting, (3) approximately when it was made? If the answer to (3) is "I can tell exactly — it was made during that specific news cycle" — the thumbnail has an expiration date.

---

*Document complete. 18 visual formats + 5 strategic sections.*
*Evergreen channel references throughout: Wendover Productions · Kurzgesagt · RealLifeLore · Our World in Data · Johnny Harris · Real Engineering · Simplicissimus · Veritasium · ColdFusion · The Pudding · FiveThirtyEight · The Economist · New York Times Graphics.*