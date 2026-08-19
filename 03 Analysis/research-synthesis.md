# IBM Z & LinuxONE Seller Enablement — Research Synthesis

**Source:** Qualitative design research (GTM Project Mural board)
**Method:** In-depth interviews + screen walkthroughs + think-aloud protocol + global comparative analysis
**Geographies covered:** India, France, Japan, Turkey, USA, South Africa
**Board:** [GTM Project — Mural](https://app.mural.co/t/ibm14/m/ibm14/1786592009673/c8a4aff9c9076ceb2e588c20c3d94c08a12964e4)

---

## Research Objective

> Map the end-to-end sales journey for IBM Z and LinuxONE sellers, identify tools and materials used at each stage, and surface key pain points, gaps, and opportunities that the CDC Design team can address through design and content strategy.

---

## Research Methods

| Method | Description |
|---|---|
| **In-Depth Interviews (IDIs)** | 60–90 minute semi-structured sessions with sellers and technical sellers covering daily workflows, sales journey, tool usage, and challenges. All sessions recorded and transcribed. |
| **Screen Walkthroughs** | Participants shared screens to demonstrate navigation of Seismic, Sales Kit, pricing tools, and AI assistants in real time — surfacing navigation friction and content gaps organically. |
| **Think-Aloud Protocol** | Participants narrated their thought process as they navigated tools, revealing mental models, workarounds, and expectations that structured questions alone would not capture. |
| **Global Comparative Analysis** | Insights from 5 geographies compared to identify universal vs region-specific challenges — particularly around language, localisation, and territory structure. |

---

## The Sales Journey — 7 Stages

| Stage | Seller Actions | Tools & Materials | Seller Emotion |
|---|---|---|---|
| **1. Identify & Qualify** | Identify target accounts; understand customer stack (Oracle/VMware/x86); cold calling; partner leverage; CXO relationship building | Claude AI (customer research), partner networks, cold outreach — no IBM-native tool | Frustrated, unsupported — relies on guesswork |
| **2. Discover & Educate** | First customer meeting; CXO pitch; educate on LinuxONE value proposition; initial qualification | Seismic Sales Kit (executive presentations), one-pagers, occasionally videos at events. Sellers customise downloaded slides. | Moderately confident — good materials exist but time needed to adapt |
| **3. Design & Solution** | Architecture of LinuxONE solution; TCO analysis; sizing; workload assessment; NMON data collection; consolidation ratio | IT Economics Team (consolidation ratio), E-config (sizing), Excel (TCO scenarios), Claude AI (customer tailoring) | Confident technically, but slowed by tool fragmentation |
| **4. Propose** | Create and deliver pricing proposal; DOAP; adapt Sales Kit decks to client; submit for price approval | ePricer (pricing tool), Excel (scenario modelling), Seismic (client presentation decks), DOAP templates | High stress — pricing approval is multi-level and slow |
| **5. Proof of Concept (POC)** | Set up and execute POC; prove Oracle database or target workload performance on LinuxONE; report results to customer | Internal tech teams, client data environment, performance benchmarks | Resigned — same POC repeated at every account |
| **6. Negotiate & Close** | Pricing negotiation; contract finalisation; legal approval (local); signing | ePricer, Q2C, contract portals, local legal translation (Turkey, Japan), Engage Support | Relieved but exhausted — process is opaque for new sellers |
| **7. Post-Sale & Expand** | Global Account Checklist submission; machine build (FOE); shipment; customer onboarding; identify expansion opportunities | Engage Support, Q2C, IBM internal shipping/build systems | Cautiously optimistic — limited cross-regional knowledge sharing |

**Structural mismatch:** The full cycle runs ~270 days. Sellers are measured on 90-day quarterly targets.

---

## The Central Research Insight

> The IBM Z / LinuxONE sales journey has **two critical collapse points** — Stage 1 (no prospect intelligence) and Stage 5 (9-month POC cycle) — that make the entire journey feel longer than it needs to be. Every other stage has workarounds. These two have none. Design must solve the **zero-to-qualified problem** and the **proof-to-trust problem** first.

---

## Tool Ecosystem

### IBM Official Tools
- Seismic / Sales Kit — primary content hub
- ePricer — pricing tool
- E-config — hardware configuration
- IT Economics Team — TCO & sizing
- Q2C — order management
- Engage Support — ticket portal
- W3 — internal IBM search
- YourLearning — training platform
- IBM Docs — public technical docs
- WatsonX / IBM Bob (used by some US sellers)

### Workaround / Shadow Tools (not IBM-sanctioned)
Sellers have independently built their own AI toolchain because IBM's official tools don't answer contextual questions fast enough:

- **Claude AI** — customer research, pitch personalisation
- **Microsoft Copilot** — email drafting, quick lookups
- **Google Gemini Notebook** — uploading Redbooks for Q&A
- **Excel** — scenario modelling, pricing comparisons
- **Local folders** — saving and reusing downloaded Seismic files
- **Slack channels** — informal SME knowledge queries
- **AI translation tools** — English → Japanese / Turkish localisation

> Every seller has independently built an AI workaround. This is not a behavioural quirk — it is a clear design requirement. The market has already voted.

---

## The 11 Problems Identified

### P1 · Critical (Universal, large revenue surface, design can own it fully)

**Problem 1 — Fragmented content ecosystem**
Sales content lives across Seismic Sales Kit, brand team decks, Tech Exchange presentations, public IBM Docs, and Redbooks — with no single searchable hub. Sellers must know where to look or they miss relevant content entirely.
> *"It's spread across Seismic, brand teams have their own presentations on Teams... it's hard to find the information you're looking for."*
> *"You need to know where to look... the search doesn't answer your questions."*

**Problem 2 — Tribal knowledge trap (universal)**
Critical operational knowledge — how to start a price approval, what tools to request access to, how to raise a credit check, FOE process, PO loading steps — exists only in people's heads. New sellers hit walls and ask managers or colleagues, creating bottlenecks. SMEs give theoretical answers that don't help field sellers close deals.
> *"There is no documentation for new sellers where to start. You need to find someone who knows it and ask... credit check, DPL, FOE — these steps are not documented anywhere."* — Bulent Palabiyik, Turkey
> *"A lot of tribal knowledge is required... the people we are directed to don't give us very good answers."* — Suresh Jayanthi, India
> *"Every pretty much every day, I'll message my manager and say, hey, who's the right person to talk to about this?"* — Matt Geran, USA

**New sellers take 12–18 months to become effective** because the entire sales process is undocumented.

---

### P2 · High (Strong signal, significant cycle impact, clear design solution)

**Problem 3 — Prospect intelligence vacuum**
There is no IBM tool to identify which customers are running Oracle or VMware and approaching a server refresh — the primary entry-point trigger for LinuxONE sales. Sellers rely entirely on cold calls and informal partner network intelligence.
> *"If there is a tool which can give me that insight as to what is the current stack of the customer... today if I'm targeting 5 opportunities, I'll be easily able to address 20."* — India team

**Problem 4 — The POC treadmill**
Nearly every LinuxONE deal requires a POC to prove Oracle database performance — a fact the market already accepts. POCs take 6–10 months and consume capacity that could be used for new accounts. Sellers are perpetually re-proving the same known truths.
> *"We are proving that Oracle databases work well on LinuxONE — every single client. Same chemistry experiment. Why spend time? The world already knows."*
> *"Axis Bank POC: started June 2025, finished December 2025, got order March 2026. That's a 9-month engagement — but I have a 3-month window to close a deal."*

**Problem 5 — Content-to-business-outcome gap**
IBM materials explain LinuxONE capabilities well but stop short of connecting them to measurable business outcomes. New sellers especially cannot bridge the gap between "8 nines availability" and "your exchange pays ₹100 crore per 4-hour outage." The sales enablement narrative is product-centric, not outcome-centric.
> *"The current enablement materials explain LinuxONE capabilities well, but field sellers need more guidance on how to connect those capabilities to specific business outcomes."*
> *"Even I didn't know in the initial years. It is only by practice that you get to know what the business outcomes are — a hard path to learn."*

**Problem 6 — Sales Kit: high potential, declining habit**
The Sales Kit (Seismic) is valued when sellers first join and for new product launches. However, once a seller knows the material, they stop returning — there is no push mechanism, no update notifications, and content is downloaded and localised locally, making the source stale.
> *"If I save the file, I assume it is finished... it is rare that I'm going for the updated file in Seismic."*
> Sellers have no idea when Sales Kit content is updated — they pitch with stale materials.

**The Sales Kit is not the problem — the ecosystem around it is.** Fixing notifications, search, and localisation delivers more value than redesigning the Kit itself.

---

### P3 · Medium (Real problem, moderate design leverage, needs partnership)

**Problem 7 — Localisation as a hidden tax**
Japan and Turkey bear a significant productivity penalty: all sales materials are English-only, requiring manual translation of 5–6 slides per deck, AI-assisted translation with human correction, and local legal approval for contracts. Rina (Japan) estimates 6 hours per document; the process is repeated for every new version and every customer customisation.
> *"We check the deck, then translate the deck, then customise and merge for each customer — so we need one extra step to translate to Japanese. This is not easy."* — Hideomi Ezumi, Japan
> *"For Turkey, I need to find contract changes, translate to Turkish, then ask for approval from our local legal team. US sellers just download and send."* — Bulent Palabiyik, Turkey

**Problem 8 — ISV certification and partner ecosystem lag**
Software not certified on LinuxONE creates deal-blocking moments mid-cycle. The certification pipeline is opaque and depends on sellers demonstrating opportunity before ISVs invest. Tier-2 channel partners are under-enabled and cannot independently position LinuxONE.
> *"NCDX specifically asked for Confluent on LinuxONE. It was not certified. I had to say no — it took worldwide escalation to get it certified in time, and only because we showed an active opportunity."*
> *"Partners who can position LinuxONE will advocate for it even when we are not in the room. Right now we have one or two. That's not enough."*

**Problem 9 — Shadow AI adoption**
Every seller has independently built an AI workaround (Claude, Copilot, Gemini Notebook). IBM's official tools cannot answer contextual questions fast enough. If IBM does not act, sellers will fully migrate their workflows to consumer AI tools.

---

### Quick Wins

**Problem 10 — Videos underused in client contexts**
Videos exist in the Sales Kit and are appreciated during onboarding. However, sellers rarely use them with clients: in India, links were flagged by client security systems; globally, sellers prefer live technical experts over pre-recorded video. Videos work effectively at events and exhibitions.
> *"It got flagged in their system. From that point onwards I stopped sharing links for the video."*

**Problem 11 — No cross-regional win story sharing**
No mechanism exists to learn from wins in Vietnam, South America, or EMEA. Win stories cover banking only. Sellers in pharma, utilities, and defence enter deals without analogous references. No cross-regional success story repository exists.

---

## Cathedral vs. Bazaar Design Principle

IBM Z and LinuxONE require fundamentally different sales enablement strategies. IBM currently applies a **cathedral-style approach** to both.

- **IBM Z** — deep, authoritative, structured documentation suits its established enterprise buyer
- **LinuxONE** — expanding into new markets (digital assets, sovereign cloud, AI infra, white-space accounts) needs a **bazaar model**: social proof, crowd signals, peer benchmarks, reusable evidence

Designing for the bazaar will unlock LinuxONE growth faster than any documentation improvement.

---

## Opportunities — Design Solutions

| Opportunity | Stage | Problem Addressed |
|---|---|---|
| **AI-Powered Prospect Intelligence Tool** — surface Oracle/VMware install base data, server refresh cycles, and transformation project signals | Stage 1 | Problem 3 |
| **Capability-to-Outcome Mapping Tool** — visual reference matrix: LinuxONE capability → customer question to ask → business outcome by industry (BFSI, Defence, Exchange) and persona (CIO, CFO, CISO) | Stage 2 | Problem 5 |
| **Workload Benchmark Content Library** — curated, BFSI-focused library of certified workload benchmarks (Oracle DB, Kafka, Red Hat, DB2 vs x86) — reusable across all deals | Stage 3 | Problem 4, 8 |
| **Fast-Track Budgetary Estimate Path** — streamlined pre-approval pricing flow giving sellers a budgetary range for early-stage conversations | Stage 4 | Problem 11 |
| **POC-Replacement Reference Package** — library of pre-certified, IBM-validated proof assets (benchmark results, workload performance data, third-party audits) that replace the live POC for common workloads — collapsing 9 months to weeks | Stage 5 | Problem 4 |
| **Seller Closing Process Playbook** — step-by-step digital guide covering every action from first pricing through to signed contract and PO loading, with tool links, access request instructions, and checklist by market/region | Stage 6 | Problem 2 |
| **Global Win Story Repository** — searchable, curated hub of deal win stories indexed by industry, workload, geography, and deal size | All stages | Problem 11 |
| **Smart Content Update Alerts** — push notification system (Slack/email) alerting sellers when Sales Kit assets are updated with a "What's Changed" summary | All stages | Problem 6 |
| **PO Loading Status Tracker** — lightweight visibility dashboard showing real-time PO loading status across all three levels | Stage 6–7 | Problem 2 |
| **WatsonX AI Assistant in Seismic** — contextual Q&A inside the Sales Kit before sellers fully migrate to consumer AI tools | All stages | Problem 9 |

---

## Success Metrics

| Opportunity | Metric | Target |
|---|---|---|
| Prospect Intelligence Tool | Qualified opportunities per seller per quarter (baseline: 3–5) | 2× within 2 quarters |
| Prospect Intelligence Tool | Time spent on manual prospecting (hrs/week) | 30% reduction |
| Capability-to-Outcome Mapping | % of sellers using the outcome mapping tool per quarter | 60% adoption within 2 quarters of launch |
| Workload Benchmark Library | Time to produce TCO analysis (baseline: 4–8 hrs manual Excel) | Under 90 mins |
| Closing Process Playbook | % of new sellers (under 18 months) who used the playbook for their first deal | 90% within 6 months of launch |
| Smart Content Update Alerts | % of sellers returning to Sales Kit after initial onboarding | 60%+ monthly active users |
| Win Story Repository | Monthly active users citing a win story as relevant to an active deal | 50% of sellers referencing ≥1 win story per quarter |

---

## Problem Classification

| Priority | Description |
|---|---|
| **P1 · Critical** | Universal problem, large revenue surface, design can own it fully |
| **P2 · High** | Strong signal, significant cycle impact, clear design solution |
| **P3 · Medium** | Real problem, moderate design leverage, needs partnership |
| **Quick Win** | Low effort, fast credibility for team, good first delivery |

---

## Design North Star

> *"We made it easier for every seller to find the right content, understand what to say, and know what to do next — and help move deals forward."*

Three design problems map to three measurable outcomes:

1. **Find the Right Content** → Unified hub + notifications → Sellers spend less time searching, more time selling → Measurable by return visits and time-to-find metrics
2. **Know What to Do Next** → Onboarding playbook → New sellers ramp faster → Measurable by time-to-first-deal for new hires before vs. after
3. **Say the Right Things** → Capability-to-outcome navigator → Sellers connect features to CXO value → Measurable by seller confidence surveys and deal stage progression

**Revenue enablement story:** Faster ramp + better pitches + less time lost. This is how design proves its worth without owning a revenue number directly.

---

## Recommended Next Step

Run a **1-hour virtual Design Thinking workshop** with 6–8 sellers across India, APAC, and EMEA to:
- Validate findings
- Prioritise the top 3 opportunities collaboratively
- Co-create the first sketches of Horizon 1 solutions
