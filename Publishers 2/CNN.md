# March 2026 · AI Strategy · Monetisation · Advertising · Video Player · Paywall · Newsroom · Comparison with NYT

---

## Who Is CNN

**CNN (Cable News Network)** is the largest American cable news channel. Founded in 1980 by Ted Turner as the world's first 24-hour news network. Owned by **Warner Bros. Discovery (WBD)**. Headquartered in Atlanta, Georgia. Global reach — **800+ million people**, 150 million monthly online users.

Projected CNN revenue for 2026 — **$1.8 billion**, profit — **$600 million**.

CNN is not just a website. It is a TV channel with a 45-year history that is now navigating one of the most challenging periods in its existence, attempting to build a digital future essentially from scratch.

---

## Context: Why CNN Is in Crisis

Unlike the NYT, CNN **never earned money from subscribers — it earned money from cable television**. Cable operators (Comcast, Charter, etc.) paid CNN to include the channel in their packages. These payments are called carriage fees — and they were CNN's primary revenue source for decades.

The problem: cable TV is dying. Americans are cutting the cord en masse, abandoning cable packages in favour of Netflix, YouTube, and streaming services. Every year, millions of households drop cable — and CNN loses revenue automatically, without even knowing who those people are. CNN never had a direct relationship with its audience — only through cable intermediaries.

This is the existential threat.

---

## Transformation Timeline

| Date | Event |
|---|---|
| **2022** | Failure of **CNN+** — streaming service shut down days after launch following the WBD merger |
| **October 2023** | **Mark Thompson** (former NYT CEO) appointed CNN Chairman and CEO |
| **July 2024** | Thompson announces digital transformation plan: target — **$1B+ digital business** |
| **July 2024** | First **100 layoffs** (3% of staff) as part of restructuring |
| **October 2024** | Launch of **paid paywall** on CNN.com — $3.99/month or $29.99/year |
| **January 2025** | Another **200 layoffs** (6% of staff), **$70M investment** in digital products |
| **May 2025** | Announcement of **CNN Weather** — the first lifestyle vertical |
| **October 2025** | Launch of **CNN All Access** — full streaming service at $6.99/month |
| **End of 2025** | CNN "trending well ahead of profit goals" according to Thompson |

---

## Monetisation — The Real Picture

### Historical Revenue Source: Carriage Fees

Before the digital transformation, approximately 60–70% of CNN's revenue came from **cable carriage fees** — monthly payments from cable operators for the right to include CNN in their bundles. A stable but dying business.

### Current Revenue Structure (Transition Period)

| Source | Status |
|---|---|
| **Carriage fees (cable)** | Primary, but declining — losing audience every year |
| **TV advertising** | Falling alongside ratings |
| **Digital advertising (website)** | Programmatic + direct sales, growing |
| **CNN.com subscription ($3.99/mo)** | New — launched October 2024 |
| **CNN All Access ($6.99/mo)** | New — launched October 2025 |
| **AI / content licensing** | Not yet publicly announced |

**Target for 2030:** $600M of CNN's total revenue should come from "new platform revenues" — subscriptions, streaming, and digital products.

### How Advertising Works

CNN operates a **broad advertising stack**: Google AdSense, Amazon Ad System, Rubicon Project, AppNexus, Index Exchange — meaning that unlike NYT, CNN participates in the open programmatic market. This delivers wider reach but less control and lower CPMs.

CNN offers advertisers placements across multiple channels: Connected TV, Display, Email, Mobile Video, Native, Social, and Linear TV. Global reach of 586 million monthly visitors makes this one of the largest digital audiences in the world.

### Video Player

CNN uses a **proprietary in-house video player** — built internally and integrated with their advertising stack and subscriber authentication system. This is significant: unlike NYT's use of Brightcove, CNN manages all of its video inventory independently, giving it flexibility to monetise video advertising across owned and partner channels.

Video is historically CNN's core format — the channel was built around it — and the player is embedded across all platforms: web, mobile app, and CTV. For CNN All Access, the video infrastructure extends into native apps for iOS, Android, Apple TV, Roku, and Fire TV.

**Key technical note:** the player uses standard VAST/VPAID protocols for video advertising, with Google Ad Manager (DFP) for ad serving, Prebid.js for header bidding, and Cloudflare or Akamai as CDN for global video delivery. Streaming is delivered via HLS protocol.

This is a meaningful architectural difference from NYT: a newspaper outsourced video to Brightcove because video was an added product. For CNN, video is the DNA of the entire organisation, which is precisely why they built their own solution.

---

## Paywall — How It Works

CNN launched a **metered paywall** in October 2024 — 13 years after the NYT.

**Structure:**
- **Free:** 3–5 articles per month for unregistered users
- **CNN.com subscription:** $3.99/month or $29.99/year — unlimited site access, exclusive content, fewer ads
- **CNN All Access:** $6.99/month — everything above plus live streaming of the TV channel, VOD library, CNN Originals, and exclusive live events

Important context: CNN's market research identified **18 million people in the US alone** who no longer have cable, consider themselves CNN fans, and have indicated willingness to pay for direct access. This is their primary target market for All Access.

**How it differs from the NYT paywall:** NYT spent 15 years building and refining their paywall using machine learning (the Dynamic Meter system). CNN is just starting — the paywall is simple, with no personalised limits. These are first steps, not a mature product.

---

## CNN All Access — The New Streaming Product

Launched October 2025. In CEO Thompson's words: *"the most ambitious digital offering from any news provider of TV heritage."*

**What it includes:**
- Live streaming of CNN US and CNN International
- VOD library of CNN Originals and CNN Films
- Subscriber-only exclusive content
- Interactive formats — for example, Anderson Cooper can engage with subscribers in real time during broadcasts
- Live field feeds

**Key detail:** existing cable subscribers get streaming access at no additional cost — CNN deliberately avoids competing with cable partners who still pay carriage fees.

---

## AI and the Newsroom

### What Is Known About CNN's AI Use

Publicly, CNN is significantly less transparent about AI than NYT. No specific internal AI tools comparable to Cheatsheet or Echo have been publicly announced. What is known:

- CNN actively uses AI for **video production** — quick cuts, subtitles, transcription
- As part of the transformation, Thompson announced the **merger of digital and TV newsrooms** into a unified "Follow the Sun" structure (following daylight hours across time zones)
- AI is used for **content personalisation** on the site and in the app
- Experiments with **AI-generated news summaries** for subscribers

### Position on AI Deals

Unlike NYT (active lawsuits) and The Guardian (OpenAI deal), CNN has **no publicly announced AI licensing deals** with technology companies. This is a significant gap — especially given CNN's enormous archive dating back to 1980, which carries obvious value for training AI models. A 45-year library of video footage, field reports, and breaking news coverage represents an asset that should be worth more in licensing than NYT's text archive, yet there has been no public movement on this.

---

## The Newsroom: How the Day Works

### The "Follow the Sun" Structure

Thompson's key organisational change: merging the digital and TV newsrooms into one. A single team now produces content simultaneously for TV, the website, the app, and social media. The goal: one story is produced once and adapted for all formats, rather than being created separately for each channel.

Thompson has said the "Follow the Sun" structure is already delivering measurable results in breaking news speed.

### Newsletters

CNN has several newsletters, but they are significantly less developed as a retention tool compared to NYT:

- **Five Things** — daily digest of five top stories
- **Meanwhile in China** — specialist newsletter
- **Topic-specific newsletters** across sections

CNN's newsletters function primarily as traffic drivers to the website rather than subscriber retention tools. This is a material weakness compared to NYT, where newsletters are central to the subscription flywheel.

---

## Conferences and Public Presence

- **Warner Bros. Discovery Upfronts (May 2025)** — Thompson announced CNN All Access and CNN Weather
- **Poynter** — detailed breakdown of CNN's five-year strategy with an interview with EVP Alex MacCallum
- **Deadline, Variety, Hollywood Reporter** — regular coverage of CNN's transformation
- **Reuters Institute** — CNN cited in the context of the cable TV crisis and digital transformation

---

## Strengths

✅ **A global brand with 45 years of history** — CNN is recognised worldwide. The name "CNN" means "news" to hundreds of millions of people across every continent.

✅ **Enormous audience** — 800M people globally, 150M monthly online users. A massive base for subscription conversion.

✅ **The right CEO** — Mark Thompson built NYT's subscription model from scratch. He is the only executive in the media industry with proven experience of exactly this type of transformation — and he has done it three times (BBC, NYT, CNN).

✅ **CNN All Access is architecturally correct** — direct streaming without intermediaries. There are 18M potential "cord-cutter" subscribers in the US alone.

✅ **Video as DNA** — CNN has always been a video-first organisation. Video is their primary format, and video is growing faster than any other digital format.

✅ **$70M investment** from Warner Bros. Discovery — real capital for transformation, not just rhetoric.

✅ **Ahead of financial targets** — Thompson confirmed at year-end 2025 that CNN was tracking ahead of profit projections.

---

## Weak Points

❌ **No subscription history** — NYT began building their subscription model in 2011, 15 years ago. CNN started in 2024. The infrastructure maturity gap is enormous.

❌ **CNN+ failure as reputational baggage** — the launch and near-immediate shutdown of CNN+ in 2022 was one of the most high-profile media failures in recent years. Every new CNN product carries that reputational shadow.

❌ **Political trust is damaged** — CNN ranked third among cable news networks in 2025, behind Fox News and MSNBC. A portion of the audience left permanently due to perceived bias. A subscription model depends on trust.

❌ **No AI policy and no AI newsroom tools** — no public editorial guidelines, no concrete tools like Cheatsheet. CNN is significantly behind NYT on AI integration.

❌ **No AI licensing deals** — a massive archive stretching back to 1980 is not being monetised through AI companies.

❌ **Paywall without personalisation** — a simple metered paywall with no Dynamic Meter equivalent. Significant revenue is being left on the table through low conversion rates.

❌ **Slow execution on promises** — the CNN Weather app, announced in May 2025, had not launched by year-end. The gap between announcements and delivery is visible.

❌ **Dependency on the parent company** — WBD itself is under financial pressure, with overall company revenues declining. CNN is not an independent entity and can be impacted by parent-level decisions — including the current M&A uncertainty involving Paramount.

---

## Forward Plans

**Official target: $1B+ digital business by 2030.**

$600M of that total should come from "new platform revenues" — subscriptions, All Access, and digital products.

**Five-year plan (2024–2029):**

Launch of **15+ "verticals"** — thematic digital products behind the paywall. CNN Weather is the first. Per EVP MacCallum: if 3–4 of the 15 succeed, that is a win.

**Specific near-term steps:**
- Global expansion of CNN All Access — currently US-only
- Launch of CNN Weather app (delayed, but still in plans)
- New lifestyle verticals (health, finance, travel — likely candidates)
- Partnerships: already signed a deal with **Variety** to stream their "Actors on Actors" series

**The 2026 Midterm elections and the 2028 Presidential election** have been named as key conversion moments for CNN All Access. Breaking news events historically drive subscription growth.

---

## Notes from My Own Perspective

**What CNN is getting right:**

The appointment of Thompson as CEO is the best strategic decision Warner Bros. Discovery could have made. He is the only person alive who has already done this exact transformation — at the NYT. He understands the task.

CNN All Access is architecturally correct. Not a separate product, but an extension of the existing brand. "It's not CNN 'plus' — it's CNN" is exactly the right message. It avoids the trap that CNN+ fell into.

**What raises serious questions:**

CNN is 13 years behind NYT in building a subscription model. In that time, NYT formed a daily habit for 13 million paying customers. CNN is starting from zero — and doing so in a significantly more competitive environment.

The absence of an AI strategy is a blind spot that is hard to explain. CNN has 45 years of video archive — field reports, breaking news, interviews. This is a more valuable AI training asset than NYT's text archive, which sold to Amazon for $20–25M per year. CNN could arguably command more. Yet there has been no public movement in this direction whatsoever.

---

## CNN vs NYT — Direct Comparison

| Parameter | CNN 📺 | NYT 📰 |
|---|---|---|
| **Revenue** | ~$1.8B (2026 projection) | ~$2.7B (2025) |
| **Historical primary revenue** | Cable carriage fees | Print advertising and subscriptions |
| **Digital subscription** | Launched October 2024 ($3.99/mo) | Running since 2011 (12.78M subscribers) |
| **Streaming** | CNN All Access — $6.99/mo (October 2025) | No standalone streaming product |
| **Paywall** | Simple metered, no personalisation | Dynamic Meter on ML, 15 years of evolution |
| **Video player** | Proprietary in-house player across all platforms | Brightcove + developing own infrastructure |
| **AI in the newsroom** | No public tools or editorial guidelines | Echo, Cheatsheet, published AI policy |
| **AI content licensing** | No announced deals | Amazon deal ($20–25M/year) |
| **Newsletters** | Weakly developed as retention tool | Core retention instrument, dozens of lists |
| **Bundle products** | None (one news product + All Access) | 5 products in one subscription |
| **CEO transformation experience** | Mark Thompson — built the NYT transformation | Meredith Kopit Levien — continuing it |
| **Primary risk** | Will not build subscription fast enough before cable collapses | AI search engines destroying traffic → fewer conversions |
| **Primary strength** | Global brand, 45-year video archive, 800M reach | 13M paid subscribers, 5-product bundle |

**The key difference in one sentence:**
NYT has already built their subscription model and is defending it. CNN is only beginning to build theirs — against a backdrop of their primary business dying and a significant time deficit.

---

*Sources: Warner Bros. Discovery SEC Filings 2025, CNN Business, Deadline, Variety, Hollywood Reporter, Poynter, Reuters Institute Digital News Report 2025, Status.news, Mediaite, Columbia Journalism Review, public statements by CNN CEO Mark Thompson and EVP Digital Alex MacCallum.*
