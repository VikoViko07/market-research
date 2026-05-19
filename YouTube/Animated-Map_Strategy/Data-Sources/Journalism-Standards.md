# Source Verification for Evergreen YouTube
## A Standalone Reference Document

---

## Part 1 — What Good Journalism Actually Is

Three principles used by every serious news organization — Reuters, AP, BBC, The Economist. These are not suggestions. They are the operational standards that distinguish journalism from content creation.

### 1. Verifiability
Every factual claim must have a source that can be independently checked. Not "sources say" — a specific document, a named person, a named database. If a claim cannot be traced to a verifiable source, it is an assertion, not a fact.

### 2. Corroboration
Sensitive or significant claims require at least two independent sources that agree. One source saying X is a claim. Two independent sources saying X is a fact. Reuters calls this the corroboration rule. AP calls it the two-source standard.

### 3. Separation of fact and interpretation
"Germany's industrial output fell 4.5% in 2024" — fact (Destatis data).
"Germany is losing its industrial identity" — interpretation.
The audience must always be able to tell which is which. In video: facts appear with source attribution on screen. Interpretations are clearly framed as analysis.

---

## Part 2 — What Data Gets Collected by Journalists

For every factual claim in a published piece, professional journalists record:

| Field | What it is | Example |
|-------|-----------|---------|
| Claim | The exact wording used | "Production fell 4.5%" |
| Primary source | Name of the document or institution | Destatis press release |
| Source date | When the source was published | February 7, 2025 |
| Access date | When you retrieved it | April 17, 2026 |
| URL | The direct link | destatis.de/EN/Press/... |
| Archive URL | Wayback Machine snapshot | web.archive.org/web/... |
| Second source | Corroborating source if exists | IMF Country Report 2024 |
| Tier | Reliability level 1–4 | Tier 1 |

This is the source trail. If a claim is disputed years later, you can reconstruct exactly where it came from and when you accessed it.

---

## Part 3 — Where Attribution Goes in a Video

Three separate places, each with a different purpose:

**On screen (during the frame):**
Small text at the bottom of every chart or data frame.
Format: `Source: World Bank, 2024`
Purpose: Viewer knows the origin of this specific data point in real time.

**In the video description (full list):**
Every source used in the video, grouped by type, with full URLs.
Purpose: Viewer can verify any claim independently.
This is the source trail made public.

**Copyright notice for your own work:**
At the end of the description: `© 2026 [Channel Name]. Original analysis and visualizations. Data sources listed above.`
This protects your editorial work — the visualizations, structure, narrative — while acknowledging the underlying data belongs to its sources.

**What you do NOT own:**
- World Bank, EIA, Eurostat data — CC BY, free to use with attribution
- Reuters or AP article text — copyrighted, you can cite findings but cannot reproduce text
- A politician's quote — you can use it (it's a public statement), but cannot claim it as your content

---

## Part 4 — Journalism Standards by Publication

### Reuters Trust Principles

Three legally binding principles in place since 1941:

**Freedom from bias.** Reuters must never take sides. This makes it the most reliable source for geopolitical and economic claims where other sources have institutional interests.

**Integrity of the news.** Every claim must be attributable to a named source or clearly labeled as analysis. Key distinction for your agents:
- "According to the company" = press release paraphrase. Weaker.
- "According to documents reviewed by Reuters" = genuine primary source journalism. Stronger.

**Independence from commercial interest.** Reuters cannot be paid to cover a story.

**How to read Reuters in your prompts:**
When a Reuters article uses "confirmed" — two sources agreed. When it uses "said" — one source. When it uses "claimed" — reporter has doubts. Your agents should flag the attribution verb.

---

### AP Stylebook Key Rules

**Anonymous sources:** Only when information is essential and cannot be obtained otherwise. For your agents: a claim supported only by unnamed sources in a news article is weaker than a named source — flag as single-sourced.

**Attribution verbs signal confidence:**
- `said` — neutral factual statement
- `claimed` — implies doubt
- `alleged` — legal uncertainty
- `confirmed` — verified by second source

**Every statistic must have a named source.** If a news article quotes a number without naming where it came from — that article is not a reliable citation for the number itself. Find the original.

---

### BBC Editorial Guidelines (Public, bbc.co.uk/editorialguidelines)

**Due impartiality:** Controversial topics must represent all significant credible viewpoints. For evergreen video: if genuine expert disagreement exists (climate policy, economic forecasts), present the range of credible positions.

**Source transparency:** "Experts say" without naming the experts fails BBC standards. Apply the same rule to your channel.

**Harm through selective presentation:** A statistic presented without its full context can mislead even if technically accurate. BBC requires that statistics be presented with sufficient context that a reasonable viewer draws an accurate conclusion.

---

### Conflicting Sources Protocol

When two authoritative sources give different numbers:

**Step 1:** Check if they measure the same thing. World Bank and IMF GDP often differ because of different base years, PPP conversion rates, or revision cycles. Different methodology = expected difference.

**Step 2:** Check dates. More recent data supersedes older data.

**Step 3:** Use the more conservative figure and note the range: "Between $X (World Bank) and $Y (IMF)."

**Step 4:** Flag as contested on screen if unresolved: state that different methodologies yield different results.

---

## Part 5 — AI and LLM Standards in Journalism (2024–2025)

All three major news organizations have published explicit policies:

**Reuters (2023):** AI-generated content requires human editorial review before publication. AI research outputs are drafts, not publishable facts.

**AP (2023):** "AI cannot replace the judgment of a trained journalist." AI is permitted for transcription and data analysis. All AI-assisted content must be labeled and reviewed.

**BBC (2024):** Factual claims verified only by AI must be flagged for additional human review before broadcast.

**The universal standard that emerges:** AI as research assistant. Human as editorial authority. Your agent system should be built on this principle — agents gather, flag, and format. You decide what goes in the video.

---

## Part 6 — How Top YouTube Channels Actually Handle Sources

### Our World in Data — The Gold Standard

OWID is the most rigorously sourced educational channel on YouTube. Their approach is fully documented at ourworldindata.org/faqs.

**What they do:**
- Every chart shows the data source inline — not in a footnote, but directly on the visualization
- When they combine or transform data (regional aggregations, per capita calculations), they explicitly state what was done: "Our World in Data based on WHO and UN data"
- When they produce original data themselves, they label it: "Official data collated by Our World in Data"
- Every chart has a download button — viewers can get the raw data and verify it themselves
- CC BY license — anyone can use their charts with attribution

**The OWID source chain in practice:**
Data point on screen → "Source: World Bank" → clicking the source link opens the World Bank page → from there you reach the raw dataset.

There is no gap in the chain. Every number has a trail you can follow from the screen to the primary institution.

**What this means for your prompts:** When you tell an agent "use OWID as a source," the correct citation is not OWID itself but the underlying source OWID draws from. OWID is a processor, not an origin. Cite: "World Bank data via Our World in Data."

---

### Wendover Productions — Structural Data Over Event Claims

Wendover's sourcing is visible in their video descriptions. Observable patterns:

**They avoid event claims in favor of structural claims.** Instead of "On March 14, 2019, ExxonMobil announced X" — they say "By 2024, production had reached X barrels per day." The structural claim is anchored to a dataset (EIA), not to a news event. The dataset verifies itself.

**Their source list is institutional, not journalistic.** Typical Wendover sources: EIA, World Bank, Bloomberg (paywalled), academic papers, company investor relations pages. They rarely cite news articles as primary sources for data.

**They build derived metrics.** The Guyana video table — Oil Reserves Per Capita — does not exist in any dataset. Wendover computed it from EIA reserves divided by World Bank population. The derived metric is attributed as computed, not cited as found.

**For your prompt system:** Wendover's implicit standard is: if a number comes from a dataset, cite the dataset. If a number is computed, show your work.

---

### Kurzgesagt — Scientific Citation Standard

Kurzgesagt applies a science publication standard to YouTube:

**All scientific claims cite peer-reviewed papers.** Not news articles about papers — the papers themselves.

**They maintain a dedicated fact-checking team** that reviews scripts before production, not after.

**They publish corrections publicly** — including in pinned comments and updated video descriptions — when errors are found.

**They have re-uploaded videos** when errors were significant enough that correcting the description was insufficient.

**What McGill University found** (published analysis, 2023): High production values create an "illusion of scholarship." Tight editing and dramatic music reduce a viewer's critical thinking. This is the specific risk your channel must manage: production quality must not outpace research quality.

---

### Johnny Harris — The Cautionary Pattern

Johnny Harris started adding source lists to video descriptions after public criticism. But the McGill University analysis identified a recurring pattern: sources are listed, but not always correctly represented. The problem was not lack of sources — it was sources cited for claims they did not fully support.

**What this means for your agent system:** Listing sources is necessary but not sufficient. Agent 7 (Editorial Integrity Check) exists precisely to catch the case where a source is technically cited but the claim overstates what the source actually says.

---

## Part 7 — Wikipedia: Nuanced Standard

### How Journalists Actually Use It

Journalists at Reuters, AP, and BBC use Wikipedia for exactly three things — and only these three:

**1. Orientation.** Learning the names of key actors, institutions, and documents before searching for primary sources. "What is the Stabroek Block?" → Wikipedia tells you it's an offshore oil block in Guyana operated by ExxonMobil. Now you know what to search for in EIA and SEC EDGAR.

**2. Finding document names.** Wikipedia articles about treaties, laws, and contracts list their official names. Knowing the correct official name is essential for finding the primary document in official databases.

**3. Following footnotes to primary sources.** A Wikipedia footnote pointing to a government report, court document, or peer-reviewed paper is a pointer to a primary source. The Wikipedia text is irrelevant. The footnote is the value.

### The Footnote Method

```
1. Find the Wikipedia claim
2. Find the footnote number [N]
3. Scroll to References — find footnote N
4. Read the citation — does it name a specific verifiable document?
5. Retrieve that document directly
6. Verify it says what Wikipedia claims

STOP if:
→ No footnote on the claim
→ Footnote links to another Wikipedia article  
→ Footnote links to dead URL (try Wayback Machine)
→ Footnote cites a blog, forum, or social media
→ Document says something different from Wikipedia
```

### More Authoritative Than Wikipedia — By Topic

| Topic | Go directly to |
|-------|---------------|
| Country economic data | World Bank country overview, IMF Article IV reports, central bank annual reports |
| Corporate facts | Company investor relations page, SEC 10-K or 20-F filing |
| Historical events | National newspaper archive from the event date, national archives (archives.gov, nationalarchives.gov.uk, bundesarchiv.de) |
| Science / medicine | PubMed, arXiv, specific journal databases |
| Treaties and law | UN Treaty Collection (treaties.un.org), EUR-Lex (eur-lex.europa.eu) |
| Government statistics | Destatis, Eurostat, ONS, US Census — always more authoritative than Wikipedia's summary of their data |

---

## Part 8 — Off-the-Record, Embargo, Legal Minimums

### Off-the-Record

A source gives you information with the condition you will not publish it or attribute it to them. This is a binding agreement in professional journalism. Breaking it ends careers.

**For YouTube:** If anyone gives you data or context "not for publication" — it cannot appear in your video, even paraphrased.

**Practical rule:** Never agree to off-the-record terms without understanding exactly what you're agreeing to. Clarify: "Do you mean I cannot use this at all, or I can use it without naming you?"

### Embargo

Information provided in advance on condition you do not publish before a specified date and time.

**Consequence of breaking:** Permanent loss of access to that source.

**Check for:** Press releases from companies and governments often carry embargo terms. The document will state them at the top.

### Legal Minimums for Educational YouTube

**Copyright on quoted material:** Approximately 14 words from a copyrighted source without permission — this is fair use (US) / fair dealing (UK/EU) for commentary, criticism, or education. Longer quotes require permission.

**Attribution ≠ copyright clearance.** Saying "according to Reuters" does not give you the right to read their article text on camera.

**Government data is generally copyright-free:** EIA, World Bank, Eurostat, Destatis — free with attribution.

**Corporate data:** Company reports and industry statistics may be copyrighted — check terms before reproducing tables or charts.

---

## Part 9 — Chain of Custody for Data

For every piece of data used in a video:

```
1. Download the source document (PDF or CSV)
   Filename: [indicator]-[source]-[YYYY-MM-DD]

2. Archive the source URL:
   Go to web.archive.org/save/[your-url]
   Save the resulting archive URL

3. Log:
   Original URL | Archive URL | Date accessed | 
   Exact value | Page/section | Agent that retrieved it | 
   Verification tier | Challenger verdict

4. Store in: /[video-title]-sources/
```

**Why this matters:** A video published today will be watched in 2029. Government agencies update and revise historical data. A number that was correct on publication day can appear "wrong" three years later when the source revises it. Your archive URL shows what the source said on the day you published.

---

*Standalone reference document. Covers: journalism principles, data collection standards, attribution placement, publication standards (Reuters, AP, BBC), conflicting sources protocol, AI standards in newsrooms, how top YouTube channels handle sources (OWID, Wendover, Kurzgesagt, Johnny Harris), Wikipedia nuanced standard, off-the-record/embargo rules, legal minimums, chain of custody.*

---

## Part 10 — Media Bias and Political Slant of Sources

Not all sources are equally neutral. For evergreen videos on geopolitics, economics, or policy, the political orientation of a source affects how it frames facts — even when the underlying data is accurate.

### Tools for Assessing Source Bias

**AllSides (allsides.com)**
Rates news sources on a spectrum: Left / Lean Left / Center / Lean Right / Right.
Based on blind surveys of political scientists and the public.
Free to use. Most useful for: US news outlets.

**Media Bias/Fact Check (mediabiasfactcheck.com)**
Rates sources on bias AND factual reporting quality separately.
A source can be biased but factually accurate (opinion-driven journalism).
A source can appear neutral but have poor fact-checking.
The combination of both ratings is more useful than either alone.

**Ad Fontes Media — Media Bias Chart (adfontesmedia.com)**
Places sources on a two-axis chart: political bias (horizontal) + reliability (vertical).
The chart is updated regularly. Free version available.
Most comprehensive visual tool for comparing outlets.

**Reuters Institute Digital News Report (reutersinstitute.politics.ox.ac.uk)**
Annual survey of news trust across 46 countries.
Useful for: assessing which outlets audiences in specific countries trust.
Especially relevant for European and German sources.

### How to Use Bias Ratings in Your Agent Prompts

```
SOURCE BIAS CHECK for this claim:
"[claim]"

Sources found: [list from Agent 1]

For each source, check:
1. AllSides rating (if US source): [Left/Center/Right]
2. Media Bias/Fact Check factual rating: [Very High/High/Mixed/Low]
3. If source rates LOW on factual reporting:
   - Flag this source
   - Find a replacement from a higher-rated outlet

BIAS DIVERSITY CHECK:
- Are all sources from the same political orientation? FLAG if yes.
- Are all sources from the same country? FLAG if yes.
- Is there at least one source from each side of a contested claim? 
  Required for: any political, economic policy, or geopolitical claim.

OUTPUT: List of sources with bias rating + factual rating.
Flag any source that is LOW factual OR lacks a counterbalancing perspective.
```

### The Key Distinction for Educational YouTube

A biased source is not necessarily wrong. Reuters (rated Center) and a center-right outlet can both accurately report the same GDP figure. The bias becomes a problem when:

- The source selects which facts to include and which to omit
- The source frames a neutral fact with charged language
- The source presents analysis as fact

Your Agent 7 (Editorial Integrity) should check whether your claim inherits the framing of a biased source — not just whether the underlying number is correct.

---

## Part 11 — Image and Video Verification

Educational YouTube uses b-roll, archival photos, maps, and satellite imagery. Each of these can be misidentified, misattributed, or fake. This part covers verification tools specific to visual content.

### Reverse Image Search

**Google Reverse Image Search (images.google.com)**
Drag and drop any image, or paste a URL.
Shows where else this image appears online.
Use to: find the original source of an image, check if it's been reused in misleading contexts.

**TinEye (tineye.com)**
Reverse image search with date-sorting capability.
Most useful for: finding the earliest known appearance of an image.
If an image "from 2024" appears in TinEye results from 2018 — it is misdated.

**Yandex Image Search (yandex.com/images)**
Often finds results Google misses, especially for Eastern European and Middle Eastern content.
Use alongside Google for complete coverage.

### Video Verification

**InVID / WeVerify Browser Extension**
Plugin for Chrome/Firefox. Extracts keyframes from a video and reverse searches each one.
Use for: verifying news footage, b-roll provenance, historical video clips.
Free. Download at: invid-project.eu

**YouTube DataViewer (by Amnesty International)**
amnesty.digimethods.net/youtube
Extracts exact upload time and thumbnails from any YouTube video.
Thumbnails can be reverse-searched to verify origin.
Use for: verifying the date a video was actually uploaded vs. when it claims to show.

### Satellite and Geographic Image Verification

**Sentinel Hub (apps.sentinel-hub.com)**
Free access to European Space Agency satellite imagery.
Search any location, any date back to 2015.
Use for: verifying that a location looks as described, checking infrastructure that "was built in year X."

**Google Earth Historical Imagery**
In Google Earth desktop: View → Historical Imagery.
Shows aerial imagery going back to the 1980s for many locations.
Use for: verifying changes over time — "the factory was built between 2010 and 2015."

**NASA Worldview (worldview.earthdata.nasa.gov)**
Free real-time and historical satellite imagery from NASA.
Especially useful for: natural events (fires, floods, oil spills), land use change.

### Verification Prompt for Visual Content

```
IMAGE/VIDEO VERIFICATION for this visual element:
Description: [what the image/video supposedly shows]
Source where found: [Pexels / archive / news outlet / other]
Claimed date: [date]
Claimed location: [location]

VERIFICATION STEPS:
1. Reverse image search via Google Images and TinEye:
   - Does the image appear earlier than claimed date? [YES/NO]
   - Is it used in a different context elsewhere? [YES/NO]
2. If video: run through InVID to extract and reverse-search keyframes
3. If location claim: verify against Google Earth or Sentinel Hub
   for the claimed date

OUTPUT:
- Visual status: VERIFIED / UNVERIFIED / MISLEADINGLY USED / FAKE
- Original source (if different from where found):
- Correct date (if different from claimed):
- License: [CC0 / CC BY / All Rights Reserved / unclear]
- Safe to use: YES / NO / WITH ATTRIBUTION
```

---

## Part 12 — OSINT: Open Source Intelligence Tools

OSINT is the practice of gathering intelligence from publicly available sources. Professional journalists use OSINT for stories that do not have official press releases — shipping routes, military movements, corporate behavior, infrastructure changes. For educational YouTube covering geopolitics, energy, and economics, OSINT provides a category of primary sources not available elsewhere.

### Maritime and Shipping Data

**MarineTraffic (marinetraffic.com)**
Real-time and historical position data for commercial ships globally.
AIS (Automatic Identification System) data — ships broadcast their position by law.
Free tier: current positions. Paid tier: historical tracks.
Use for: verifying shipping routes, tracking oil tankers, confirming port visits.
Example: "The first LNG tanker from Guyana loaded at the Liza FPSO on [date]" — verifiable through MarineTraffic vessel history.

**VesselFinder (vesselfinder.com)**
Alternative to MarineTraffic. Sometimes has better coverage for specific regions.
Free tier available.

### Aviation Data

**FlightAware (flightaware.com)**
Historical and real-time commercial flight data.
Free tier: 7-day history. Paid: unlimited history.
Use for: verifying aircraft movements, confirming scheduled routes exist, tracking cargo aircraft.

**Flightradar24 (flightradar24.com)**
More consumer-friendly interface. Historical data in paid tier.
Use for: same as FlightAware. Use both for cross-reference.

### Corporate and Financial OSINT

**OpenCorporates (opencorporates.com)**
Database of 200M+ companies globally.
Shows registration date, directors, filing history.
Free to search.
Use for: verifying a company exists, finding subsidiary structures, checking registration dates.

**Companies House (find-and-update.company-information.service.gov.uk)**
UK company registry — free, complete filings.
Use for: any UK-registered company or UK subsidiary of international company.

**Unternehmensregister (unternehmensregister.de)**
German company registry equivalent.
Free, official filings for German companies.

### Geospatial and Infrastructure

**Overpass Turbo (overpass-turbo.eu)**
Query the OpenStreetMap database programmatically.
Find: all oil refineries in a region, all ports in a country, pipeline networks.
Free. Requires basic query syntax — examples available on the site.

**Global Fishing Watch (globalfishingwatch.org)**
Tracks fishing vessel activity globally using AIS data.
Free to use.
Use for: ocean economics, fishing rights disputes, maritime stories.

### OSINT in Your Agent Prompts

```
OSINT VERIFICATION for this claim:
"[claim involving shipping / aviation / infrastructure / corporate structure]"

RELEVANT OSINT SOURCES FOR THIS CLAIM:
Maritime: MarineTraffic, VesselFinder
Aviation: FlightAware, Flightradar24
Corporate: OpenCorporates, SEC EDGAR, Companies House (UK), 
           Unternehmensregister (Germany)
Geographic: Sentinel Hub, Google Earth historical, Overpass Turbo

VERIFICATION TASK:
1. What specific vessel/flight/company/location needs to be confirmed?
2. What date range is relevant?
3. Which OSINT tool is most likely to have this data?
4. What is the exact search query or coordinates to use?

OUTPUT:
- OSINT source that can verify this: [tool name]
- Exact search to run: [query / vessel name / coordinates]
- What to look for in the results: [specific confirmation needed]
- Data confidence if found: HIGH (AIS/official registry) / 
  MEDIUM (third-party aggregator) / LOW (crowdsourced)
```

---

## Part 13 — Data Staleness Matrix

Not all data ages at the same rate. Using two-year-old data for some topics is fine. Using two-month-old data for others is already outdated. This matrix defines maximum acceptable data age by topic for an evergreen video.

### Staleness Thresholds by Topic

| Topic | Max acceptable age | Why | Best source |
|-------|-------------------|-----|-------------|
| Population (national) | 3–5 years | Changes slowly | UN World Population Prospects |
| GDP (annual) | 1–2 years | Annual revisions | World Bank, IMF |
| GDP (quarterly) | 6 months | Revised frequently | IMF, national statistics |
| Oil/gas production | 1 year | Annual data | EIA, BP Statistical Review |
| Oil prices | Real-time for context, annual avg for trends | Volatile | EIA, World Bank commodity prices |
| Military spending | 2–3 years | Annual SIPRI data | SIPRI |
| Government debt as % GDP | 2 years | Annual IMF/World Bank | IMF Fiscal Monitor |
| Trade flows | 1–2 years | Annual data | UN Comtrade, WTO |
| CO₂ emissions | 1–2 years | Annual Global Carbon Project | Global Carbon Project |
| Inflation | 3–6 months | Changes monthly | World Bank, IMF |
| Unemployment | 3–6 months | Changes monthly | ILO, OECD |
| Election results | Permanent once certified | Historical fact | Official electoral commission |
| Political leader / position holder | Real-time | Changes without notice | Official government website |
| Company CEO / leadership | Real-time | Changes without notice | Company investor relations |
| Country credit rating | 6 months | Updated regularly | S&P, Moody's, Fitch |
| Energy capacity (installed) | 2 years | Annual IRENA/IEA | IRENA Statistics |

### Staleness Check in Agent Prompts

```
DATA FRESHNESS CHECK for this claim:
"[claim with a data point]"

Data used: [value + source + year of data]
Topic category: [from table above]
Maximum acceptable age for this topic: [from table]

CHECK:
1. Is the data within the acceptable age window? YES / NO / BORDERLINE
2. If NO or BORDERLINE:
   a. Is more recent data available from the same source?
   b. If yes: use the more recent data
   c. If no: flag in the video description with the data year
3. For "real-time" topics (political positions, CEO, credit ratings):
   Verify current status at official source before script is finalized.
   These MUST be checked within 48 hours of video publication.

OUTPUT:
- Data age status: FRESH / ACCEPTABLE / BORDERLINE / STALE
- Action required: [none / update / flag / re-verify before publish]
- Suggested on-screen text if flagging age: 
  "As of [year], [data point] — verify current figures in description"
```

---

## Part 14 — Source Diversity Check

Professional editorial standards require that sources do not all come from the same institutional, geographic, or political perspective. This is most important for claims about: economic policy, geopolitical disputes, environmental issues, and historical events.

### The Four Dimensions of Source Diversity

**1. Geographic diversity**
Are all sources from one country's perspective?
Example failure: Using only US sources (EIA, World Bank) for a story about an African country's economy — without including African Development Bank or regional national statistics.

**2. Institutional diversity**
Are all sources from the same type of institution?
Example failure: Using only IMF and World Bank (both Bretton Woods institutions with similar frameworks) for a story where alternative economic models are relevant.

**3. Political/ideological diversity**
For contested policy claims: are sources from only one side of the debate?
Example failure: Only using sources that support one interpretation of a disputed historical event.

**4. Temporal diversity**
Are all sources from the same period?
Example failure: Using only 2024 data for a "long-run trend" story — missing the historical context that would change the interpretation.

### Source Diversity Check Prompt

```
SOURCE DIVERSITY AUDIT for this video:

TOPIC: [topic]
ALL SOURCES USED: [list from Agent 6]

CHECK FOUR DIMENSIONS:

1. GEOGRAPHIC DIVERSITY
   Countries/regions represented in sources: [list]
   Is the subject country/region directly represented? 
   (e.g., for a story about Indonesia, is there an Indonesian source?)
   Flag if: only Western or only one regional perspective

2. INSTITUTIONAL DIVERSITY
   Institution types represented: [list]
   Are both multilateral institutions AND national sources present?
   Are both government AND independent research sources present?
   Flag if: only one type of institution

3. POLITICAL/IDEOLOGICAL DIVERSITY
   For contested claims: is more than one analytical framework represented?
   Flag if: all sources reach identical conclusions using identical assumptions

4. TEMPORAL DIVERSITY
   Date range of sources: [earliest] to [latest]
   For trend claims: is there historical data going back far enough?
   Flag if: all sources from same narrow time period

OUTPUT:
- Diversity status: DIVERSE / ACCEPTABLE / NARROW / SINGLE-PERSPECTIVE
- Missing perspective: [what type of source would add balance]
- Suggested additional source: [specific institution or outlet to check]
```

---

## Part 15 — Real Failure Case: How Errors Happen and Compound

### The Pattern: How a Small Error Becomes a Big Problem

This is a composite of several documented failures across educational YouTube channels. No specific channel is named — but the pattern is common enough that understanding it is more valuable than knowing which channel made the mistake.

**Stage 1 — The original error**
A claim appears in a secondary source (news article or analysis piece): "Country X's economy grew 400% in 10 years."
A researcher sees this and uses it in a script without tracing it to the primary source.
What actually happened: the original statistic was GDP growth in local currency terms, unadjusted for inflation and a currency devaluation. In real, comparable terms, growth was approximately 60%.

**Stage 2 — The claim goes on screen**
The number 400% appears on a chart, fully designed and animated.
The video description lists the secondary source that contained the error — not the primary data.

**Stage 3 — The first comment**
A viewer who works in the country's finance ministry leaves a comment: "This figure is incorrect. You're looking at nominal local currency growth. Real growth was much lower."
The comment gets 200 likes.

**Stage 4 — The amplification**
A competing YouTube channel or Twitter/X account posts: "Popular education channel publishes misleading economic statistics." The original error has now become a reputational story.

**Stage 5 — The correction dilemma**
The channel now faces: (a) pin a correction comment, (b) add a correction card to the video, (c) re-upload a corrected version, (d) delete the video. Each option has costs.

If they choose (a) or (b): the video stays live with the error, but the correction is visible. Most viewers still see the original number and never read the correction.
If they choose (c): the re-upload loses all watch time, comments, and algorithmic momentum. For an evergreen video this can mean losing years of accumulated SEO value.
If they choose (d): the error disappears but so does the content.

### What This Error Would Have Been Caught By

| Agent | What it would have caught |
|-------|--------------------------|
| Agent 1 | Found the primary World Bank GDP data showing real vs nominal figures |
| Agent 2 | Flagged the secondary source (news analysis) as Tier 4, not primary |
| Agent 5 | Noticed that secondary source figure (400%) diverges significantly from World Bank real GDP figure (60%) |
| Agent 7 | Editorial integrity check: "nominal local currency GDP growth presented as general economic growth creates false impression of prosperity" |
| Agent 8 | Chain of custody would have shown the data came from a Tier 4 source — prompting re-verification before publication |

### The Lesson

Every step of the failure was preventable with the 8-agent system. The error was not a research failure — the researcher found a source. It was a **classification failure** (Tier 4 source treated as Tier 1) and an **integrity failure** (the headline number was technically from the source, but the source was itself using a misleading metric).

This is why Agent 7 — the editorial integrity check — is the most important agent in the system. A claim can have a source, pass all technical checks, and still mislead.

---

## Part 16 — Research Brief Template

Before launching agents, fill this document for every video. It takes 15–20 minutes and saves 2–3 hours of unfocused searching.

```
═══════════════════════════════════════════════════════════
VIDEO RESEARCH BRIEF
═══════════════════════════════════════════════════════════

TITLE (working): [video title]
Topic category: [economics / geopolitics / energy / science / history]
Evergreen test: [why will this be relevant in 5 years?]

───────────────────────────────────────────────────────────
CORE ARGUMENT
───────────────────────────────────────────────────────────
Story in one sentence:
[what happened / is happening / what it means]

Three-act structure:
Act 1 (context): [what was]
Act 2 (change): [what changed and why]
Act 3 (open question): [what comes next — no answer]

───────────────────────────────────────────────────────────
CLAIMS REQUIRING VERIFICATION
───────────────────────────────────────────────────────────
Claim 1: [exact wording as in script]
Type: [ ] event fact with date  [ ] statistic  [ ] causal claim
Target source tier: [1 / 2]
Where to look first: [specific source]

Claim 2: [exact wording]
Type: [ ] event fact  [ ] statistic  [ ] causal claim
Target source tier: [1 / 2]
Where to look first: [specific source]

[add more as needed]

───────────────────────────────────────────────────────────
QUOTES REQUIRING VERIFICATION
───────────────────────────────────────────────────────────
Quote 1:
Person: [name, title]
Words: "[exact as in script]"
Alleged source: [program / speech / date]
Verification target: [YouTube / transcript archive / wire service]

[add more as needed]

───────────────────────────────────────────────────────────
TRUSTED SOURCE SET FOR THIS VIDEO
───────────────────────────────────────────────────────────
Primary data sources (Tier 1):
[ ] [source name] — for [what data]
[ ] [source name] — for [what data]

Wire services for event verification (Tier 2):
[ ] Reuters — [what to search for]
[ ] AP — [what to search for]

───────────────────────────────────────────────────────────
SENSITIVE ZONES
───────────────────────────────────────────────────────────
Claims that may be contested or politically charged:
1. [claim] — contested by: [who / what perspective]
2. [claim] — contested by: [who / what perspective]

These claims require: [ ] corroboration [ ] bias diversity check
[ ] both sides represented in sources

───────────────────────────────────────────────────────────
DATA FRESHNESS REQUIREMENTS
───────────────────────────────────────────────────────────
Time-sensitive elements that must be re-verified within 
48 hours of publication:
[ ] [element] — verify at: [source URL]
[ ] [element] — verify at: [source URL]

───────────────────────────────────────────────────────────
VISUAL CONTENT TO VERIFY
───────────────────────────────────────────────────────────
B-roll / images to verify origin and license:
[ ] [description] — reverse search needed
[ ] [description] — license unclear

───────────────────────────────────────────────────────────
PUBLICATION CHECKLIST
───────────────────────────────────────────────────────────
Before upload:
[ ] All Tier-1 claims verified with primary source
[ ] All quotes confirmed with original video or transcript
[ ] Source list formatted and ready for description
[ ] Chain of custody log saved in /[title]-sources/ folder
[ ] Wayback Machine archives created for all key URLs
[ ] Time-sensitive elements re-verified within 48 hours
[ ] Agent 7 editorial integrity: PASS
[ ] Bias diversity check: complete
[ ] Data freshness: all within acceptable thresholds
═══════════════════════════════════════════════════════════
```

---

*Document updated with: media bias assessment tools, image/video verification, OSINT sources for maritime/aviation/corporate data, data staleness matrix by topic, source diversity audit framework, composite failure case analysis, and research brief template.*