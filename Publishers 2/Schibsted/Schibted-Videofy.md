### 1.1 Videofy Within Schibsted's Broader Video Strategy

Videofy is not an isolated tool. It exists inside a wider video strategy at Schibsted that is essential context for understanding its purpose and trajectory.

In parallel, VG (Norway's largest newspaper) shifted to a **vertical video format** *(TikTok-style, 9:16 aspect ratio)* for live broadcasts — and it worked: 833,000 livestream viewers during the US election coverage, 3,500+ real-time audience interactions. Schibsted's video platform **Stream** is now deployed across 40 newsrooms, including the external Polaris Media Group (30 Norwegian newspapers). Videofy is part of this ecosystem — not a standalone experiment.

> **📌 Editorial observation:** The fact that Schibsted operates both Videofy (automated text-to-video) AND a separate vertical video live platform reveals that no single tool solves the full video problem. Videofy handles the long tail of daily news articles. The vertical live platform handles breaking news and youth engagement. These are two different jobs, and conflating them would be a mistake.

---

### 1.2 The AI Academy and FAST Framework

Videofy was not built in a vacuum. Since 2019 Schibsted has run an **AI Academy** (600+ staff trained) and applies the **FAST framework** to all AI development:

- **F**airness
- **A**ccountability
- **S**ustainability
- **T**ransparency

Every AI tool, including Videofy, undergoes a risk assessment before production deployment. This explains why human-in-the-loop is not an optional feature in Videofy — it is an architectural requirement imposed by the FAST governance model.

Agnes Stenbom, head of IN/LAB at Schibsted Sweden: *"Our use of AI will be the best it can be if we also excel at managing the downsides of the technologies."*

---

### 1.3 Presentation at "Voices" Festival in Florence

Lopez Calvet demonstrated Videofy from the stage at **"Voices — European Festival of Journalism and Media Freedom"** in Florence shortly before the open source release. The framing matters: the tool is positioned not merely as a technical solution but as a **contribution to media freedom** — open source as a mechanism for lowering the innovation barrier for small newsrooms that cannot build this independently.

This public positioning — at a press freedom festival, not a tech conference — signals how Schibsted wants Videofy to be perceived: as a democratic infrastructure tool for journalism, not as a competitive product.

---

### 1.4 Key Statistics from Internal Use

Before going open source, Schibsted used Videofy internally to produce **thousands of videos** across its brands. The tool generates **20-second videos instantly** from any published article. The application is integrated directly into Schibsted's CMS — when a writer finishes an article, the video generation option appears immediately in the interface.

Per WAN-IFRA (November 2025): suggested stories powered by Schibsted's AI tools achieved the same click-through rate as the original first story, with an **85% thumbs-up ratio** — indicating that AI-assisted content was meeting editorial quality standards for readers.

---

## 2. Shortcomings and Limitations

### 2.1 Technical Limitations

**Local rendering only — no cloud infrastructure**

The open source version renders video **locally on a laptop**. For a single article, this is acceptable. For a newsroom publishing 50–100 articles per day, this is a fundamental bottleneck. Cloud rendering infrastructure must be built separately by each publisher. In Schibsted's full internal setup this is handled by proprietary integrations intentionally excluded from the open source release.

**Dependency on two paid external APIs**

The pipeline requires both **OpenAI** (script generation) and **ElevenLabs** (voiceover). Both are paid, both can change their pricing, and both are single-vendor dependencies. At scale — thousands of videos per month — API costs grow significantly. Schibsted can absorb this; a regional newspaper in Poland or a local broadcaster cannot necessarily do so.

**Horizontal format only (16:9)**

Videofy produces video for **digital signage** *(screens in public spaces)* and websites in horizontal 16:9 format. But TikTok, Instagram Reels, and YouTube Shorts require vertical 9:16. This is not a minor gap: Schibsted is building its vertical video platform for VG *separately* — meaning Videofy in its current form is entirely irrelevant for reaching younger audiences on social platforms. The tool solves one video problem while leaving another completely unaddressed.

**No video monetisation**

Videofy produces video but does **not monetise it**. There is no built-in ad inventory, no **SSAI** *(Server-Side Ad Insertion — the technology that inserts advertising server-side, seamlessly within the video stream)*. For publishers who need to not just create video but generate revenue from it, Videofy is only half a solution. This is precisely the gap that Videofy.ai (the Israeli startup) fills from day one.

**No support for external video assets within articles**

If an article contains links to external videos (YouTube, Vimeo), Videofy cannot use them — only images and video clips already embedded directly in the source article. This limits output quality for multimedia-rich journalism.

**Minimal fetcher plugin library**

The repository includes basic fetchers for Reuters, AP, and a test URL. There are no ready-made integrations for WordPress, Arc XP, Drupal, Ghost, or other widely used CMS platforms. Every publisher must write their own fetcher — a non-trivial engineering task.

---

### 2.2 Editorial and Ethical Shortcomings

**No mandatory AI content labelling**

Nowhere in the workflow is there a mandatory disclosure that the video was AI-generated. An editor can publish the output without any transparency to readers. Given growing public and regulatory demand for AI labelling in journalism — the EU AI Act, industry self-regulation initiatives — this is a notable gap.

**No fact-checking layer**

The LLM generates the script from the article's text. If the article contains an error, the video reproduces it. There is no built-in fact-checking mechanism between generation and publication. Human-in-the-loop theoretically addresses this, but in a high-volume, deadline-driven newsroom, the "approve" button can be pressed quickly. The system has no safeguard against this.

**Sensitive content handling**

Videos about terrorist attacks, deaths, violent incidents require careful image selection. The hotspot model can identify the focal point within a frame — but it cannot determine whether a given image is emotionally appropriate for a specific topic. A photograph of a smiling crowd matched to a story about a mass casualty event would be a catastrophic editorial failure. Human review must catch this, but it is the most critical failure mode of any automated video system.

**No engagement metrics built in**

Videofy produces MP4 files. It does not measure whether those videos are actually watched, how long viewers stay, or whether AI-generated video performs differently from manually produced video. Without this data, it is impossible to optimise the tool's editorial ROI.

---

### 2.3 Strategic and Adoption Limitations

**High technical barrier for the target audience**

The stated ambition of the open source release is to help small and local newsrooms that lack resources to build such tools themselves. But the reality is that deploying Videofy requires: a development team to set up the stack (Docker, FastAPI, Next.js), API credentials and billing accounts for OpenAI and ElevenLabs, cloud infrastructure for production deployment, and custom fetcher development for the newsroom's own CMS. This is not a barrier for Schibsted. It is a significant barrier for a 10-person regional newspaper — exactly the audience Schibsted says it wants to reach.

**The open source version is deliberately minimal**

Schibsted explicitly states that the public repository *"leaves out most of the internal integrations and infrastructure used in Schibsted's full Videofy setup."* What is open sourced is a proof-of-concept, not a production system. The community must build the gap between the two — which means the full value of the tool remains proprietary to Schibsted.

**No community governance structure yet**

The repository was released on 17 March 2026. As of the date of this analysis it has 67 stars and 12 forks — early engagement, but no contributor guidelines, no governance model, no roadmap published. Without active community stewardship, open source projects of this type frequently stagnate after initial interest fades.

---

## 3. Future Development — What Schibsted Plans and What the Community Will Build

No official public roadmap for Videofy exists. The following is reconstructed from Lopez Calvet's three-horizon AI framework, parallel video initiatives at Schibsted, and the observable gaps in the open source release.

---

### 3.1 Horizon 1 — Efficiency (Ongoing)

These are improvements already in progress or likely near-term within Schibsted's internal deployment:

- **Group-wide rollout** — expanding from VG and E24 to all Schibsted newsrooms (Aftonbladet, Svenska Dagbladet, Bergens Tidende, Aftenposten, Stavanger Aftenblad)
- **Rendering speed** — reducing generation time below current "minutes" towards near-real-time
- **Hotspot model improvement** — training on larger datasets of Schibsted editorial photography to improve focus accuracy
- **CMS integration stability** — hardening the integration point between Videofy and Schibsted's internal CMS across different brand configurations

---

### 3.2 Horizon 2 — Product Expansion (Planned)

These represent the logical next functional layer, required to close the gaps identified above:

**Vertical format (9:16)**
The most urgent gap. VG's vertical video strategy is already proven — 833,000 viewers for the US election livestream. Extending Videofy to produce vertical short-form video would connect automated article-to-video production with the existing vertical distribution infrastructure. This is not a marginal improvement; it changes the tool's audience from "people reading news on website" to "people watching short news on mobile."

**Multi-language support**
Schibsted operates across Norwegian, Swedish, Finnish, and Polish markets. Videofy currently generates content in the language of the source article. Automated translation and cultural adaptation — similar to the approach El País uses for LatAm content via its OpenAI partnership — would allow a single Norwegian article to generate localised video versions for multiple markets.

**Live video asset integration**
Enabling Videofy to pull and use externally hosted video clips (from news agencies, archival sources) rather than only static images already in the article would significantly improve video quality for breaking news and complex investigative journalism.

**AI content labelling**
Mandatory, standardised disclosure that a video was generated with AI assistance — both in the video itself and in metadata. Lopez Calvet has emphasised transparency as a core principle; the tooling should enforce it rather than relying on editorial discipline.

---

### 3.3 Horizon 3 — Uniqueness (Ambition)

These are longer-term possibilities consistent with Schibsted's stated AI strategy:

**Audience-personalised video versions**
Different video renditions of the same article tailored to different reader segments — by interest profile, age cohort, or platform context. By analogy with Aftenposten's AI homepage personalisation (which delivered +25% CTR), personalised video could be the next frontier. The same article generates one version for the sports-focused reader and another for the politics-focused reader — automatically.

**Agentic Videofy**
Rather than waiting for a journalist to trigger video generation, an agentic version of Videofy would monitor publication queues, identify articles most likely to benefit from video treatment (based on topic, traffic prediction, engagement history), and initiate production autonomously — routing the output to the human editor for final approval. This is consistent with Schibsted's three-horizon framework where Horizon 3 represents *"AI creating uniqueness."*

**Integration with ARIA**
ARIA is Schibsted's internal AI analytics agent — a multi-agent framework allowing staff to query real-time data across all brands through Slack. Connecting ARIA to Videofy would enable data-driven decisions about which articles to prioritise for video production: *"Which articles published today have the highest engagement trajectory and no video yet?"* becomes an automated trigger rather than a manual editorial judgement.

---

### 3.4 What the Open Source Community Will Likely Contribute

Based on observable gaps and standard patterns of open source contribution in media technology:

| Contribution | Why it's likely |
|---|---|
| **WordPress / Ghost fetcher plugins** | The two most common CMS platforms globally; obvious first community contributions |
| **Arc XP fetcher** | Washington Post's Arc XP is used by El País, La Nación, and dozens of major publishers; Arc users have strong incentive to integrate |
| **Whisper (OpenAI) voiceover alternative** | Whisper is free and open source; reduces ElevenLabs dependency for budget-constrained newsrooms |
| **Open LLM support (Llama, Mistral)** | Reduces OpenAI dependency; enables fully self-hosted, zero-external-API deployment |
| **Vertical 9:16 output mode** | The single most-requested likely feature given the dominance of TikTok/Reels |
| **AI disclosure watermark** | Automatic labelling of AI-generated video, consistent with emerging regulatory requirements |
| **Docker Compose cloud profiles** | Moving from laptop-local to AWS/GCP/Azure deployment for production use |

---

## 4. The Central Unresolved Question

Videofy solves the **production** problem elegantly. Three adjacent problems remain entirely unsolved:

**Distribution** — where does the video go after rendering? The tool produces an MP4. Getting it into YouTube, TikTok, the CMS article, digital signage screens, social channels simultaneously requires a separate distribution layer that Videofy does not provide.

**Monetisation** — who earns from the video and how? A publisher that creates 100 AI-generated videos per day needs to generate advertising revenue from them. Videofy has no ad insertion, no programmatic integration, no revenue model.

**Measurement** — what is the editorial and commercial impact of AI-generated video versus manually produced video? Without built-in analytics, it is impossible to know whether the tool is actually adding value or just adding volume.

Until these three dimensions are addressed — either within Videofy itself or through clear integration partners — the tool remains a production utility rather than a complete editorial video strategy.

The ambition of the open source release is to let the industry solve these collectively. Whether the community of 67 GitHub stars grows into a meaningful contributor ecosystem is the question that the next 12 months will answer.

---

## 5. Summary Assessment

| Dimension | Assessment |
|---|---|
| **Core functionality** | Strong — article to video in minutes with editorial control |
| **Hotspot model** | Genuinely innovative — purpose-trained for press photography |
| **CMS integration** | Best-in-class — zero friction for the journalist |
| **Open source strategy** | Correct and timely — lowers industry barrier |
| **Technical completeness** | Partial — local rendering, no cloud, no monetisation |
| **Format coverage** | Gap — horizontal only, no vertical for social |
| **Ethical safeguards** | Incomplete — no AI labelling, no fact-check layer |
| **Community maturity** | Early stage — 67 stars, 12 forks, no governance |
| **Strategic coherence** | High — fits clearly within Schibsted's three-horizon AI framework |

Videofy is a serious, production-tested tool made available to the industry at the right moment. Its limitations are real but tractable — most are engineering gaps rather than conceptual flaws. The human-in-the-loop design is the right editorial architecture. The open source release is the right strategic move.

The question is not whether Videofy is good. It is: good enough for *whom*, and at what cost of implementation? For Schibsted's internal brands — clearly yes. For a regional newsroom with two engineers and no cloud budget — the gap between what is published on GitHub and what is running in production at VG is still significant.

---

## Glossary

| Term | Definition |
|---|---|
| Digital signage | Screens in public spaces (airports, lobbies, transport hubs) displaying dynamic content including news videos |
| SSAI | Server-Side Ad Insertion — technology that inserts advertising into video streams at the server level, seamlessly and without ad-blocking |
| Human-in-the-loop | A workflow design where AI performs tasks but a human must review and approve before output is published or acted upon |
| Hotspot model | Schibsted's proprietary computer vision model that identifies the most important focal area within a press photograph, enabling accurate automatic cropping and zoom |
| Remotion | Open source JavaScript library for programmatically creating videos; used as the rendering engine in Videofy |
| FastAPI | Python web framework used for Videofy's backend API |
| ElevenLabs | AI voice synthesis platform — used in Videofy to generate narration from the video script |
| FAST framework | Schibsted's AI governance model: Fairness, Accountability, Sustainability, Transparency |
| ARIA | Schibsted's internal multi-agent AI analytics system, allowing staff to query real-time data across all brands via Slack |
| Fetcher plugin | A module in Videofy that retrieves article content from a specific source (Reuters, AP, CMS URL) and prepares it for processing |
| Vertical video (9:16) | Video format optimised for mobile viewing, used by TikTok, Instagram Reels, YouTube Shorts — the dominant format for reaching audiences under 35 |
| Agentic AI | AI systems capable of autonomous multi-step task execution without constant human prompting; the next frontier beyond reactive AI tools |
| Stream | Schibsted's internal video platform deployed across 40 newsrooms; separate from Videofy but part of the same video infrastructure ecosystem |
| Apache License 2.0 | The open source licence under which Videofy Minimal is published — permits free use, modification and distribution including for commercial purposes |
