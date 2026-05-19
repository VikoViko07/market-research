## How Top Channels Do It — Free vs Paid Sources, Complete Guide

---

## Why This Document Exists

LLMs hallucinate. YouTube channels make mistakes. Johnny Harris has been fact-checked by McGill University and found to have significant errors. Vox has issued corrections. Even Wendover Productions has inaccuracies pointed out in comments years after publication.

For an evergreen video, an error lives in the video forever — every new viewer encounters it, and comment sections become permanent records of mistakes. The only protection is a verification workflow built before production, not after.

This document covers two types of claims that require verification:

**Type 1 — Factual events.** "The first oil tanker passed through the Strait of Hormuz on [date]." "Company X made decision Y in year Z." Historical firsts, specific dates, specific decisions.

**Type 2 — Direct quotes.** "The president said: '[exact words].'" "According to the CEO: '[statement].'" Words attributed to a real person.

Both types require different verification strategies. Both are covered here.

---

## Part 1 — The Core Problem with LLMs and Facts

Before the sources: understand why this matters specifically for YouTube research.

### How LLMs fail on factual claims

An LLM (including this one) can produce a plausible-sounding specific fact with complete confidence — and be wrong. The failure mode is not "I don't know" — it is "Here is a detailed, specific, confident answer that is incorrect."

Specific failure patterns:

**Plausible date fabrication.** "The first commercial oil shipment from Guyana departed on March 14, 2020." This type of claim sounds precise and verifiable. An LLM may produce it fluently. The correct answer requires checking ExxonMobil press releases and Lloyd's List shipping records.

**Quote contamination.** "As Irfaan Ali said in the BBC interview: '[words].'" The LLM may have the general meaning correct but the exact wording wrong. In a pull-quote card on screen, wrong exact wording is a factual error — visible, screenshottable, damaging.

**Composite facts.** An LLM may synthesize two true things into one false thing. "Country X became the world's [Nth] largest exporter of Y in [year]" — where the country, the rank, the commodity, and the year are each individually plausible but the combination is wrong.

**The practical rule:** Any specific claim of the form "[who] did [what] on [date]" or "[person] said '[exact words]'" must be verified through a primary source before going into a script. Never use an LLM output as the citation — use the LLM to find the direction, then verify the destination.

---

## Part 2 — Verifying Factual Events

### The verification hierarchy for events

| Tier | Source type | Example | Strength |
|------|-------------|---------|---------|
| 1 | Primary document | ExxonMobil press release, government decree, company filing | Strongest — the original record |
| 2 | Wire service report from the date | Reuters or AP article published the day the event occurred | Very strong — contemporaneous journalism |
| 3 | Academic paper citing the event with footnote | Peer-reviewed article with named primary source | Strong |
| 4 | Reputable news outlet published within 30 days | NYT, BBC, The Economist, FT | Good |
| 7 | LLM output | Any AI-generated claim | Never use as citation |

**The working rule:** Before including any specific event claim in a script, find its Tier 1 or Tier 2 source. If you cannot find it — the claim does not go in the video.

---

### Free Sources for Verifying Factual Events

#### Reuters Archive (Free Articles)
**URL:** reuters.com  
**What it covers:** Wire service dispatches from 1851 to present. The most important news archive for evergreen research because Reuters was present at most major global events as they happened.  
**Free access:** Reuters.com search returns articles from approximately 1990s onward freely. Use site search: `reuters.com "first oil tanker" "Strait of Hormuz"`.  
**Limitation:** Full archive before ~1995 requires paid access (Reuters Professional).  
**How to use for verification:** Search for the event name + approximate date. A Reuters dispatch from the date of the event is Tier 2 verification.

#### Associated Press (AP) News
**URL:** apnews.com  
**What it covers:** AP wire dispatches from 1846 to present.  
**Free access:** AP News website provides recent articles and some historical content free.  
**Limitation:** Deep historical archive (pre-1990) requires AP Newsroom subscription.  
**How to use:** Same approach as Reuters — contemporaneous AP dispatch = Tier 2 verification.

#### Google News Archive (Partial)
**URL:** news.google.com + site-specific searches  
**What it covers:** Indexed news from thousands of outlets.  
**Free access:** Fully free. Use date range filters to find articles published at the time of the event.  
**Limitation:** Not a true archive — articles may have been deleted from original sources. Access to paywalled content not included.  
**How to use:** `site:nytimes.com "first oil" Guyana before:2020-06-01` to find contemporaneous coverage.

#### Wayback Machine / Internet Archive
**URL:** web.archive.org  
**What it covers:** Snapshots of websites going back to 1996, including news articles that have since been deleted or moved behind paywalls.  
**Free access:** Fully free, CC0.  
**Best use case:** A Reuters or BBC article from 2003 that is now behind a paywall — find the archived version.  
**How to use:** Enter the original URL of the article → Wayback Machine shows the captured version from the date it was live.

#### SEC EDGAR (For Corporate Events)
**URL:** sec.gov/edgar  
**What it covers:** All filings of US-listed public companies — press releases, earnings calls, annual reports, 8-K event filings.  
**Free access:** Fully free, government data.  
**Best use case:** Verifying when a company announced a decision, what exactly was said in an official statement, financial figures.  
**How to use:** Search company name → select filing type (8-K for events, 10-K for annual reports) → find the exact document.

#### Official Government and Institutional Press Releases
**URL:** Varies — search `[country] ministry official statement [event] site:.gov`  
**What it covers:** Every major government action, policy decision, treaty signing.  
**Free access:** Fully free, public domain.  
**How to use:** For "when did Guyana's government sign the Stabroek PSA" — search Guyana government official site or Ministry of Natural Resources. The press release is the Tier 1 primary document.

#### Hansard (UK Parliamentary Debates)
**URL:** hansard.parliament.uk  
**What it covers:** Complete verbatim transcripts of UK Parliament debates from 1803 to present.  
**Free access:** Fully free.  
**Best use case:** Verifying what a British politician said, when a policy was announced in Parliament.

#### Congressional Record (US)
**URL:** congress.gov  
**What it covers:** Complete verbatim transcripts of US Congress proceedings.  
**Free access:** Fully free, government data.

#### The Internet Archive Newspaper Collection
**URL:** archive.org/details/newspapers  
**What it covers:** Digitized historical newspapers, many from 19th and early 20th century.  
**Free access:** Fully free, CC0 or public domain.  
**Best use case:** Events before 1950 that have no digital news archive equivalent.

---

### Paid Sources for Verifying Factual Events

#### LexisNexis / Nexis Uni
**URL:** lexisnexis.com  
**What it covers:** 4 billion+ documents from 36,000+ sources. News archives going back 40+ years. Newspapers, newswires, transcripts, trade journals, court records.  
**Cost:** Professional subscription — approximately $150–300/month for individual access. Academic version (Nexis Uni) available through university library access — effectively free if you have a library card.  
**Best use case:** Finding a specific Reuters or AP dispatch from 1985. Searching across 100 newspapers simultaneously for an event.  
**The alternative:** If you have any university library access, Nexis Uni is available free through that institution.

#### Dow Jones Factiva
**URL:** professional.dowjones.com/factiva  
**What it covers:** Wall Street Journal archive from 1889, plus 33,000+ news sources globally.  
**Cost:** Approximately $100–200/month for individual access.  
**Best use case:** Wall Street Journal and Financial Times archives for business and financial event verification.  
**The alternative:** FT.com and WSJ.com both have free article limits — 3–5 articles/month without subscription.

#### ProQuest Historical Newspapers
**URL:** proquest.com  
**What it covers:** Digitized archives of major newspapers going back to founding dates — New York Times from 1851, Washington Post from 1877, The Guardian from 1821.  
**Cost:** Subscription varies — approximately $20–50/month individual. Available through many public libraries for free.  
**Best use case:** Historical events in the 19th and early 20th century.  
**The free alternative:** Many public libraries in Germany (Stadtbibliothek) and the UK provide ProQuest access with a library card.

#### Lloyd's List Intelligence (For Shipping and Maritime)
**URL:** lloydslistintelligence.com  
**What it covers:** Maritime shipping records from 1734. Every significant ship movement, cargo, route, incident.  
**Cost:** Professional subscription — approximately $300+/month.  
**Best use case:** Your "first tanker through the Strait of Hormuz" example. Lloyd's List would have the original record.  
**The free alternative:** Lloyd's List publishes some historical articles free at lloydslist.com. For deep archive access, university libraries sometimes have subscriptions.

#### Oil & Gas Journal Archive
**URL:** ogj.com  
**What it covers:** Technical and business news about the oil and gas industry from 1902.  
**Cost:** Subscription — approximately $200/year.  
**Best use case:** First oil discoveries, pipeline completions, refinery openings — any petroleum industry historical fact.

---

## Part 3 — Verifying Direct Quotes

Quotes require a completely different verification approach from factual events. A quote is wrong not just if the person never said it — it is also wrong if the person said something similar but the exact wording differs.

### The verification hierarchy for quotes

| Tier | Source | Example | Strength |
|------|--------|---------|---------|
| 1 | Official transcript | Parliamentary Hansard, White House transcript, UN official record | Strongest — verbatim official |
| 2 | Video of the person saying it | YouTube clip, C-SPAN, BBC iPlayer — you can see and hear it | Very strong |
| 3 | Wire service article quoting it with attribution | Reuters: "President Ali said: '[words]'" in same-day report | Strong |
| 4 | Original interview transcript published by the outlet | BBC HARDtalk published transcript | Strong |
| 5 | Newspaper article from the day with direct quote | NYT, FT, The Guardian direct quote with "said" | Good |
| 6 | Aggregated quote on a quote website | Brainyquote, Goodreads Quotes | Never use — unverified |
| 7 | LLM-generated quote | Any AI output | Never use |

### The Most Important Rule for Quotes

**Never use a quote you cannot find in a Tier 1–4 source.** Quote aggregators (BrainyQuote, QuoteInvestigator pending verification, Goodreads) frequently contain misattributed, paraphrased, or fabricated quotes. If you cannot find the quote in a primary or tier 2–4 source, it does not go in the video.

---

### Free Sources for Verifying Quotes

#### YouTube + C-SPAN (For Video Verification)
**URL:** youtube.com + c-span.org  
**What it covers:** Speeches, press conferences, interviews, parliamentary sessions.  
**Best use case:** Political speeches, presidential addresses, CEO earnings calls. If the person said it publicly in a recorded setting, it is often on YouTube.  
**How to use:** Search `[person name] "[approximate quote fragment]" speech` — find the original video, timestamp the exact words.  
**Why this is Tier 2:** You can see and hear the person saying the exact words. Unambiguous.

#### BBC, CNN, Al Jazeera Interview Archives
**URL:** bbc.co.uk/news + edition.cnn.com + aljazeera.com  
**What it covers:** Published transcripts and video of major interviews.  
**Free access:** Most interview content free on their websites.  
**Best use case:** The BBC HARDtalk interview (President Ali vs BBC's Sackur on climate — mentioned in Guyana analysis). BBC publishes transcripts of many HARDtalk episodes.  
**How to find:** `bbc.co.uk hardtalk "Ali" transcript 2024`

#### Quote Investigator
**URL:** quoteinvestigator.com  
**What it covers:** Research into the true origin of famous quotes — extremely useful for debunking misattributed quotes.  
**Free access:** Fully free.  
**Best use case:** Before using a famous quote attributed to Churchill, Einstein, or Twain — check here first. Approximately 90% of famous attributions are wrong or paraphrased.  
**Important:** Quote Investigator shows what was actually said and by whom, with primary source links.

#### Google Scholar + Full Text Search
**URL:** scholar.google.com  
**How to use for quotes:** Search the approximate text of a quote in quotation marks. If a peer-reviewed paper cites this quote, its footnote leads to the primary source.  
**Example:** `"trusting your viewer to go fact-check everything you say is irresponsible"` — this leads to the Johnny Harris source where he said it.

#### Hansard + Congressional Record
(Covered in Part 2 — same sources apply for politician quotes in parliamentary settings)

#### UN Official Document System
**URL:** documents.un.org  
**What it covers:** Verbatim records of UN General Assembly, Security Council, all official UN meetings.  
**Free access:** Fully free.  
**Best use case:** Verifying what a head of state said at the UN General Assembly or Security Council.

---

### Paid Sources for Verifying Quotes

#### LexisNexis / Nexis — Same as Part 2
**Additional quote use case:** Search `"Ali" AND "right to lecture" AND BBC` with date filter → find the Reuters or AP dispatch that quoted him the day of the interview. The wire service report is Tier 3 verification.

#### Factiva — Same as Part 2
**Additional quote use case:** Wall Street Journal and FT interviews often have verbatim quote passages. The original interview transcript is Tier 4 verification.

#### Broadcast Media Archives (For Video Quotes)
**URL:** Various — BBC Archive, CNN Vault, C-SPAN Archive  
**Cost:** C-SPAN full archive free. BBC Archive access varies. CNN Vault — contact directly.  
**Best use case:** Finding the exact broadcast where a statement was made, with precise timestamp.

---

## Part 4 — How Top Channels Actually Do This

### Wendover Productions

Wendover's verification approach is visible from the source lists in their video descriptions and the types of claims they make. Three observable patterns:

**Pattern 1 — Data claims only from institutional sources.** Wendover does not make claims of the form "On [exact date], [person] decided [thing]." They make claims of the form "By 2024, production had reached X barrels per day" — which comes from EIA or World Bank data, not from a news narrative. This is a deliberate editorial choice that reduces the verification burden. When you anchor your claims to datasets rather than events, the verification is the dataset itself.

**Pattern 2 — The video description as a source list.** Every Wendover video description includes sources. Looking at the types of sources cited, the pattern is: EIA, World Bank, Bloomberg (paywalled articles), academic papers. No quote aggregators. No LLM outputs.

**Pattern 3 — Structural claims over event claims.** "The Stabroek contract gives ExxonMobil 45% of profit oil" — this is verifiable from the contract itself (a primary document), not from a news article reporting on it. Wendover gravitates toward claims that can be anchored to primary documents.

### Our World in Data

OWID has the most rigorous citation practice of any educational YouTube channel. Every single data point on their website links to a primary source. Their verification approach:

- Every chart has a "Sources" section linking to the original dataset
- Every statistic in narration appears in the chart
- No claim exists in narration that does not appear in the chart
- The chart's source is always Tier 1 (World Bank, WHO, UN)

**The OWID standard** is the gold standard for evergreen content. It is also the most labor-intensive — approximately 3–5 hours of additional verification per video. But it is why OWID videos are cited by Nature, The Economist, and Harvard.

### Johnny Harris — The Cautionary Case

McGill University published a detailed analysis of Johnny Harris's factual errors. The pattern of errors is instructive:

- Oversimplification of complex historical causation (presenting one factor as the cause)
- Economic claims that contradict mainstream academic consensus
- Historical narrative that collapses multi-actor events into single-actor stories
- Quotes that capture the spirit but not the exact words of a statement

The McGill analysis noted that Johnny Harris's production values "give the illusion of scholarship" — tight editing and dramatic visuals create confidence in the viewer that the research is equally tight. This is the specific risk for visually sophisticated educational YouTube: the production quality can outpace the research quality.

**The lesson:** High production value requires commensurate research quality. A beautiful slope chart built on an unverified fact is more dangerous than a simple chart built on verified data — because more viewers will trust it.

### Kurzgesagt

Kurzgesagt's verification approach differs from Wendover and OWID because their topics are often scientific rather than event-based. Their approach:

- All scientific claims cite peer-reviewed papers
- They maintain a dedicated fact-checking team
- Corrections are published publicly when errors are found
- They have retracted and re-uploaded videos when errors were significant

The Kurzgesagt model works for science topics where peer-reviewed consensus is the Tier 1 source. For historical or geopolitical events, the equivalent is primary documents and wire service archives.

---

## Part 5 — The Verification Workflow

### Step 1 — Flag every specific claim in the script

Go through the script. Mark every claim that is:
- A specific date ("in 1973...")
- A specific number not from a dataset ("the contract was signed by...")
- A direct quote ("the minister said...")
- A historical first ("the first time this happened was...")
- A causal claim ("this caused X")

These are verification targets. Everything else — structural trends, general descriptions, dataset-anchored numbers — is lower priority.

### Step 2 — For each flagged claim, find the Tier 1–3 source

For each verification target, search in this order:
1. Primary document (government, company, institution)
2. Wire service report from the date (Reuters, AP)
3. Academic paper with footnote to primary source

If you find a Tier 1–3 source: record the URL, date accessed, and the specific text that confirms the claim.

If you cannot find a Tier 1–3 source after 15 minutes of searching: either reframe the claim to remove the specific detail, or cut the claim from the script.

### Step 3 — For quotes, find the video or transcript

For every direct quote attributed to a named person:
1. Search YouTube for the interview or speech
2. Search the outlet's website for the transcript
3. Search Reuters/AP for the same-day wire dispatch quoting it

If you find the original: timestamp it, copy the exact words, verify they match what you have in the script.

If there is any discrepancy between your quote and the original: use the original, not your version.

### Step 4 — Build the source document alongside the script

Create a parallel document with two columns: the claim in the script, and the source that verifies it. This document becomes the video description sources list.

**Template:**

```
CLAIM IN SCRIPT                          SOURCE
"First oil from Guyana: Dec 2019"        ExxonMobil press release, Dec 20, 2019
                                         URL: [link]

"Contract gives ExxonMobil 45%"          Stabroek PSA, Global Witness analysis
                                         URL: [link]

"Ali said: '[exact words]'"              BBC HARDtalk transcript, March 2024
                                         URL: [link]
```

### Step 5 — The two-source rule for sensitive claims

For any claim that:
- Contradicts common knowledge
- Makes a specific accusation
- Involves a disputed historical event
- Attributes a motive to a person or institution

Require two independent sources confirming the same fact before including it. If only one source exists — note it as single-sourced in the video description.

---

## Part 6 — Cost Comparison

### Full Free Tier (€0/month)

| Tool | What you get |
|------|-------------|
| Reuters.com search | News from ~1995+ |
| AP News | News from ~2000+ |
| Google News with date filter | Broad news search |
| Wayback Machine | Archived paywalled articles |
| YouTube / C-SPAN | Video verification of quotes |
| SEC EDGAR | US corporate primary documents |
| Government websites | Official press releases |
| Quote Investigator | Famous quote verification |
| UN Documents | Official UN meeting transcripts |
| Congressional Record / Hansard | Parliamentary quotes |
| Internet Archive newspapers | Pre-1950 historical press |

**Coverage:** Adequate for events from 1995 onward and for recent quotes. Adequate for government and corporate primary documents of any era. Limited for 1950–1994 events not covered by freely accessible archives.

**Total cost: €0**

---

### Partial Paid Tier (€20–50/month)

| Tool | Cost | What it adds |
|------|------|-------------|
| Public library card (Germany/UK) | Free | Access to ProQuest, Nexis Uni, newspaper archives through library |
| ProQuest via library | Free with card | NYT from 1851, Washington Post from 1877, Guardian from 1821 |
| Nexis Uni via library | Free with card | 40-year news archive, 36,000+ sources |

**The most cost-effective upgrade:** A library card at a Stadtbibliothek (German municipal library) or UK public library typically provides ProQuest and Nexis Uni access. Cost is library card fee, often free or €10–20/year.

**Total cost: €0–20/year**

---

### Professional Tier (€150–400/month)

| Tool | Cost | What it adds |
|------|------|-------------|
| LexisNexis Nexis Professional | ~€150–300/month | Full 40-year archive, 36,000+ sources, advanced search |
| Dow Jones Factiva | ~€100–200/month | WSJ from 1889, FT archive, Dow Jones content |
| Lloyd's List Intelligence | ~€300+/month | Maritime records from 1734 |
| Oil & Gas Journal | ~€200/year | Petroleum industry records from 1902 |

**When professional tools are justified:** If your channel produces 2+ videos per month on topics requiring deep historical verification (pre-1990 events, maritime/energy industry history, financial history), the time saved by LexisNexis typically justifies the cost at scale.

**For a starting channel:** Begin with the free tier + library card. Upgrade to professional tools when production volume makes the time cost of free-tier searches consistently exceed the subscription cost.

---

## Part 7 — Topic-Specific Source Map

### Energy and oil industry history
- **Free:** EIA (eia.gov), BP Statistical Review, OilPrice.com, Reuters archive
- **Free historical:** Internet Archive (pre-1950 industry publications), OPEC official documents (opec.org)
- **Paid for deep history:** Oil & Gas Journal archive (1902+), Lloyd's List (maritime, 1734+)

### Geopolitics and diplomacy
- **Free:** UN Documents (documents.un.org), Reuters/AP, C-SPAN, official government sites
- **Free historical:** Avalon Project at Yale Law (international documents, treaties) — avalon.law.yale.edu
- **Paid:** LexisNexis for broad archive search

### Economics and business
- **Free:** SEC EDGAR, Reuters, Bloomberg (limited free articles), WSJ (limited free)
- **Free historical:** FRED (Federal Reserve archive), BIS working papers
- **Paid:** Factiva for WSJ/FT deep archive

### Science and technology
- **Free:** PubMed (pubmed.ncbi.nlm.nih.gov — all biomedical research), arXiv, Google Scholar
- **Free:** Nature.com and Science.org publish some articles free
- **Paid:** Full journal access requires institutional subscription — use library

### Political quotes and speeches
- **Free:** C-SPAN, Hansard, Congressional Record, UN verbatim records, YouTube
- **Free:** Miller Center (millercenter.org) — US presidential speech archive
- **Paid:** LexisNexis for broadcast transcripts

### Maritime and shipping
- **Free:** IMO (International Maritime Organization) official documents, Reuters maritime coverage
- **Paid:** Lloyd's List (definitive, 1734+), Clarksons Research

---

## Summary — The Three Rules

**Rule 1:** Any specific fact of the form "[who] did [what] on [date]" requires a Tier 1–3 source before going in the script. LLM output is never a citation.

**Rule 2:** Any direct quote requires finding the original video, transcript, or contemporaneous wire service report. Quote aggregators are not sources.

**Rule 3:** If you cannot find the Tier 1–3 source in 15 minutes of searching — reframe the claim to remove the unverifiable specific, or cut it.

---

## The Johnny Harris Warning — In His Own Words

On fact-checking and YouTube responsibility, Johnny Harris himself said (in reference to Joe Rogan): "The idea of trusting your viewer to go fact-check everything you say is irresponsible and naïve."

He was right. The same standard applies to every educational YouTube channel, including his own — and including yours.

---

*Verification guide for evergreen YouTube production. Sources and pricing verified as of April 2026. Tool costs vary — check current pricing before subscribing.*

---

## Part 8 — Three Real Verification Cases (How It Actually Works)

### Case A — Event Fact with a Date
**Claim to verify:** "Qatar's first LNG export shipment departed in 1997."

**Step 1 — Reuters search**
Go to reuters.com. In the search box type: `Qatar LNG first export 1997`
Set date filter: 1996–1998.

What you find: A Reuters dispatch from early 1997 reporting on the departure of the first LNG tanker from Ras Laffan Industrial City. The article names the vessel, the destination (Japan), and the date.

**What the source looks like:**
```
Reuters, January 1997
"Qatar ships first LNG cargo to Japan"
Author: [Reuters staff]
URL: reuters.com/[article-path]
Accessed: April 2026
```

**Result:** Tier 2 verification. Claim confirmed. The source goes in the video description.

**If Reuters finds nothing:** Try AP News with the same query. Then try Google News: `"Qatar" "first LNG" 1997 site:ft.com OR site:economist.com`. Then try the Wayback Machine on a Financial Times URL from 1997.

---

### Case B — Political Quote
**Claim to verify:** President Ali's exact words to BBC HARDtalk on climate.

**Step 1 — YouTube search**
Search: `Irfaan Ali BBC HARDtalk climate 2024`
Find the interview. It exists — it became widely shared.

**Step 2 — Find the exact timestamp**
Watch or scrub through the video. The exchange about climate begins approximately at the 8–12 minute mark depending on the episode cut. Ali's words: "What gives you the right to lecture us about climate change?"

**Step 3 — Cross-check with BBC transcript**
Search: `bbc.co.uk hardtalk Ali transcript 2024`
BBC publishes HARDtalk transcripts for most episodes. The transcript confirms the exact wording.

**What the source looks like:**
```
BBC HARDtalk, March 2024
Irfaan Ali, President of Guyana
Original broadcast: bbc.co.uk/programmes/hardtalk
Timestamp: [XX:XX]
Transcript confirmed at: bbc.co.uk/[transcript-path]
```

**Result:** Tier 2 verification (video) confirmed by Tier 4 (published transcript).

**Critical rule:** If the transcript says "What right do you have to lecture us" and your script has "What gives you the right to lecture us" — use the transcript version. The difference is small but the quote is on screen. Exact words only.

---

### Case C — Historical Fact Not Freely Available
**Claim to verify:** "The first oil tanker regularly passing through the Strait of Hormuz did so in [year]."

**Step 1 — Free sources first**
Search Reuters archive: `Strait of Hormuz oil tanker first 1950s`
Search Google News with date range: `"Strait of Hormuz" tanker before:1960-01-01`
Search Internet Archive newspapers: `hormuz tanker`

**Likely result:** Nothing definitive in free sources. Pre-1960 maritime history is not well covered in freely accessible digital news archives.


**Step 3 — What to do when you cannot verify**
Option A: Reframe the claim. Instead of "the first tanker passed through in [year]" — say "oil shipments through the Strait began in the 1950s as Persian Gulf production expanded." This is verifiable from EIA production history. No specific date needed.

Option B: Acknowledge the limit. "The exact date of the first commercial oil shipment through the Strait is not recorded in publicly available sources." This is itself a verifiable fact — and it is more honest than a specific date you cannot confirm.

Option C: Use Lloyd's List (paid). Lloyd's List Intelligence has maritime records from 1734. If the answer exists anywhere, it is there. Cost: ~€300/month. Justified only if maritime history is a recurring topic for your channel.

**The key lesson from Case C:** An unverifiable specific date is more dangerous than no date at all. A wrong date in an evergreen video lives there for years. "The 1950s" is weaker storytelling but stronger journalism.

---

## Part 9 — Signals That a Source Cannot Be Trusted

Before using any source, scan for these red flags. Each one alone is a warning. Two or more together means do not use.

| Signal | What it means |
|--------|--------------|
| No author named | Cannot be held accountable. Professional news always has a byline. |
| No publication date | You cannot tell if this is current or outdated. |
| No links to primary sources | The claim has no trail back to verifiable data. |
| Website created less than 2 years ago | Insufficient track record to assess reliability. |
| Fact appears in only one place online | Either very obscure (verify harder) or fabricated (do not use). |
| URL contains blog, wordpress, medium | Individual opinion, not institutional reporting. |
| Headline contradicts the article body | Click-bait construction — the detail matters more than the headline. |
| Numbers differ from World Bank / IMF on the same indicator | One source is wrong. Find out which before using either. |
| "According to experts" with no named expert | Fabricated authority. Real journalism names the expert. |
| Quote site (BrainyQuote, AZQuotes) | These sites do not verify quotes. Never cite them. |

### The Single Most Useful Quick Check

Search the specific claim + "wrong" or "false" or "debunked" in Google. If someone has already fact-checked and refuted it, you will find it in 30 seconds. This does not replace verification — but it catches obvious errors instantly.

---

## Part 10 — When You Cannot Find the Source

This is the most common real situation. You search for 15 minutes and find nothing. Here is what to do, in order.

### Step 1 — Broaden the search terms

The fact may exist under different terminology.
- "Strait of Hormuz" → try "Persian Gulf shipping lanes"
- "First LNG export" → try "liquefied natural gas tanker departure"
- Proper nouns → try acronyms (LNG / "liquid natural gas" / "liquefied gas")

Try three different formulations before concluding the source does not exist.

### Step 2 — Search in a different language

If the event happened in a non-English speaking country, the primary coverage may be in that language. Google Translate + search in Arabic, German, French often surfaces sources not indexed in English.

### Step 3 — Find a secondary source that cites the primary

Search Google Scholar for academic papers on your topic. A paper from 2010 about Gulf oil history may cite a 1997 primary source you cannot find directly. The paper's footnote is your path to the primary.

### Step 4 — Check if the claim is actually a compound fact

Many "specific facts" are actually two facts combined. "Country X became the world's Nth largest exporter of Y in year Z" — check each component separately: Is Country X in the top exporters? What year did it reach that rank? Sometimes the components are verifiable even when the combined claim is not.

### Step 5 — Decide: reframe, remove, or flag

**Reframe:** Remove the unverifiable specific. "In the 1990s, Qatar began LNG exports" is weaker but verifiable. "On March 14, 1997, the first LNG tanker departed" is stronger but requires verification.

**Remove:** If the specific fact is decorative rather than essential to the argument — cut it. The video does not need the exact date to tell the story.

**Flag as single-sourced:** If you find one source but cannot find a second confirmation — include the fact but note in the video description: "Date based on single source: [citation]. If you have a primary source confirming or correcting this, please comment below." This is honest and turns your audience into fact-checkers.

---

## Part 11 — Source Citation Templates

Use these exact formats in the video description. Consistency builds credibility.

### Press release / official statement
```
[Organization name], [Title of release], [Date]
URL: [full URL]
Accessed: [Month Year]
```
Example:
```
ExxonMobil Corporation, "ExxonMobil Achieves First Oil at Liza Phase 1 Offshore Guyana," December 20, 2019
URL: corporate.exxonmobil.com/news/...
Accessed: April 2026
```

### News wire report (Reuters / AP)
```
[Author if named, otherwise "Reuters Staff" or "AP"], "[Article title]," [Publication], [Date]
URL: [full URL]
```
Example:
```
Reuters Staff, "Guyana reaches oil production milestone," Reuters, March 2022
URL: reuters.com/...
```

### Academic paper
```
[Author Last, First], "[Paper title]," [Journal name], Vol. [X], [Year], pp. [XX–XX]
DOI or URL: [link]
```

### Interview / speech (video)
```
[Person name], [Role/Title], [Program name], [Broadcaster], [Date]
Video URL: [YouTube or broadcaster link]
Timestamp: [XX:XX]
```
Example:
```
Irfaan Ali, President of Guyana, BBC HARDtalk, BBC World Service, March 2024
Video URL: youtube.com/watch?v=...
Timestamp: 09:42
```

### Government document
```
[Country] [Ministry/Agency name], "[Document title]," [Date if available]
URL: [official government URL]
```

### World Bank / IMF / UN data
```
[Organization], "[Indicator name]," [Database name], [Year of data]
URL: [direct data URL]
License: CC BY 4.0 [or relevant license]
```
Example:
```
World Bank, "Oil rents (% of GDP)," World Development Indicators, 2024
URL: data.worldbank.org/indicator/NY.GDP.PETR.RT.ZS?locations=AE
License: CC BY 4.0
```

---



---

## Part 12 — Using AI for Cross-Verification

### The Core Idea: Red Team / Blue Team

Use two AI agents with opposing instructions on the same claim. One searches for confirmation, the other searches for reasons the claim might be wrong, incomplete, or misattributed. This is a technique from intelligence analysis — if both agents reach the same conclusion independently, confidence is high. If they diverge, dig deeper.

This is especially powerful for quotes, where the risk is not just "did they say it" but "did they mean what the quote implies when taken out of context."

---

### How to Structure the Two-Agent Check

**Agent 1 — Confirmer**

Prompt:
```
I need to verify this claim for an educational video:
"[your claim or quote]"

Please:
1. Find the most likely primary source for this fact
2. Suggest the exact Reuters/AP search query that would confirm it
3. Tell me if this claim is consistent with other verified data you know
4. Rate your confidence: high / medium / low
```

**Agent 2 — Challenger**

Prompt:
```
I need to stress-test this claim before using it in a video:
"[your claim or quote]"

Please:
1. What are the most likely ways this could be wrong or misleading?
2. Is there a known misattribution risk for this type of quote?
3. Is this consistent with what you know, or does something feel off?
4. What would a fact-checker specifically look for to challenge this?
```

Run both. Compare. If Agent 1 says "high confidence, consistent with EIA data" and Agent 2 says "I can think of no plausible objection" — proceed to find the primary source. If they diverge — the divergence tells you exactly where to focus your manual verification.

---

### AI Verification Workflow for Quotes — Step by Step

Quotes are the highest-risk claim type because a slightly wrong word can change meaning, and the person quoted may object publicly.

**Step 1 — Paste the quote to Agent 1 (Confirmer)**
```
Verify this quote attributed to [person], [context]:
"[exact words as you have them]"

- Is the attribution plausible?
- Do you know of this quote from training data?
- What is the most likely source document or broadcast?
- What search query would find the original?
```

**Step 2 — Paste the same quote to Agent 2 (Challenger)**
```
Challenge this quote attributed to [person]:
"[exact words as you have them]"

- Is this a known misquote or paraphrase of something else?
- Is the attribution to [person] plausible given their known positions?
- What context might change the meaning if this is taken out of context?
- Rate misattribution risk: high / medium / low
```

**Step 3 — Use AI output to build your search queries**

Agent 1 will suggest something like: "Search YouTube for [program name] [year] [person name], or search BBC HARDtalk transcript archive."

That is your verified search direction. Now do the manual step — find the actual video or transcript.

**Step 4 — Paste the found original back to AI**

Once you have the original source:
```
I found the original source of this quote:
"[original exact words from transcript/video]"

My version was:
"[your version]"

Are these materially the same or different? 
Does the difference change the meaning?
```

This final check catches the subtle paraphrase problem — where you have the right spirit but wrong words.

---

### AI for Statistical Fact Cross-Check

For numbers and statistics, AI can cross-check internal consistency before you go to primary sources.

**Prompt:**
```
I'm using this statistic in a video:
"[country/entity]: [metric] = [value] in [year]"
Source: [where you found it]

Please check:
1. Is this consistent with related indicators you know? 
   (e.g. if GDP per capita is X, does that fit with the total GDP and population?)
2. Does this match what you know from World Bank / IMF data?
3. Any reason to be suspicious of this number?
```

**What this catches:**
- Unit errors (millions vs billions)
- Year mismatches (2022 data labeled as 2024)
- Currency confusion (nominal vs PPP)
- Outliers that are real but need context to not mislead

---

### What AI Cannot Do — Hard Limits

Even with two agents, these tasks still require manual primary source verification:

| Task | Why AI cannot replace it |
|------|--------------------------|
| Confirm exact quote wording | AI may have seen a paraphrase, not the original |
| Verify a date is correct | AI training data may contain the same error that's in news articles |
| Access paywalled archives | AI cannot browse Reuters 1997 archives |
| Confirm a fact has only one source | AI cannot know what is NOT in the internet |
| Verify a document has not been edited | AI cannot see current live documents |

**The rule that does not change:** AI tells you where to look. The primary source confirms what is there.

---

### Recommended Tools for AI Cross-Verification

| Tool | Best for | Cost |
|------|---------|------|
| Claude (this) | Structured two-prompt verification, quote consistency check | Free / Pro |
| Perplexity AI | Real-time web search + citation, good for recent quotes | Free / Pro |
| ChatGPT with web browsing | Current news verification, recent speeches | Free / Plus |
| You.com | Parallel search + AI summary with sources shown | Free |

**Two-agent setup in practice:** Use Claude for the Challenger prompt (structured reasoning about what could be wrong) and Perplexity for the Confirmer prompt (real-time web search for the source). The combination covers both reasoning quality and current web access.

---

*AI cross-verification added. The two-agent method is most valuable for quotes where misattribution or context loss is the primary risk.*
