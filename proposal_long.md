
# Autonomous Simulation-First B2B Sales System for European Solar Distribution

## Proposal for Sunlumo Energy — AI Sales Challenge

---

### The Problem

In late 2025, a Reddit post documented what has become the defining failure mode of autonomous B2B sales: **"Artisan: 1,400 emails sent, zero replies."** The pattern repeats across the category. Generic AI-generated copy, hallucinated personalization, and no pre-deployment testing conspire to burn deliverability, budget, and — most critically — brand reputation with the installer base you depend on. The root cause is structural: every major sales engagement platform on the market today — whether Artisan, 11x, Clay, Apollo, Outreach, Salesloft, or Cognism — follows the same deploy-first, learn-later paradigm. Campaigns are launched against live prospects and optimized only after real damage is done. **No platform on the market offers pre-deployment campaign simulation against synthetic buyer personas before a single email is sent.** For a distributor scaling across eight European countries, six languages, and distinct installer cultures, this gap is not a missing feature. It is an existential risk to the entire outbound motion.

The European solar distribution market compounds this challenge. Sunlumo targets approximately 50,000 to 80,000 fragmented installer firms across the DACH region, Italy, France, Spain, Poland, and the Balkans — each market governed by its own legal framework, language, business culture, and subsidy landscape. Cold outreach that works in the Netherlands is illegal in Germany under UWG §7 without explicit consent. WhatsApp dominates installer communication in Italy and Spain but is irrelevant in German Handwerk culture. A Polish growth-stage firm evaluating battery inventory responds to entirely different signals than a solo Elektromeister in Bavaria. Generalist AI sales tools — built by US-based companies, trained on English-language SaaS sales motions, and indifferent to Europe's regulatory patchwork — are structurally incapable of operating this motion. **The market is asking for a category of software that does not yet exist.**

We are building it.

---

### What We Are Building

We propose a **simulation-first, agentic sales operating system purpose-built for European solar distribution.** It is not an incremental improvement over existing sales engagement platforms. It is an architectural departure grounded in a single principle: before any message reaches a real installer, it must survive a war game against 500 synthetic installer personas whose behavior is calibrated against Sunlumo's own historical sales data.

The system comprises six integrated engines, each embodied as a specialized AI agent operating under a central Supervisor that plans, delegates, monitors, and adapts. The architecture is exposed to Sunlumo's sales team through a **visual directed acyclic graph (DAG) canvas** — a drag-and-drop orchestration layer where campaigns are designed, simulated, approved, and deployed without writing a single line of code. The core differentiator is the **Simulation Engine**: a multi-step, persona-grounded forecasting layer that predicts reply rates, objection patterns, channel preferences, and full-funnel conversion before any real outreach begins. Every probability surfaced by the system emerges not from an LLM guessing at likelihoods, but from counting outcomes across parallel simulation runs — each constrained by empirical behavioral priors extracted from Sunlumo's existing CRM data, email history, Intercom logs, and webshop transactions.

This is not a tool for automating emails. It is an **AI sales organization** that Sunlumo directs — not configures — from a visual control room. The Supervisor Agent decomposes high-level goals ("launch SigenStor 10kWh in Italy and Poland this quarter") into task plans. The Research Agent monitors legislation, trade registers, forums, and competitor pricing to surface opportunities proactively. The Persona Builder maintains a library of installer digital twins whose behavioral parameters are continuously updated through Bayesian inference as real campaign outcomes return. The CopyWriter Agent generates native-language outreach in German, Italian, French, Spanish, Polish, and Dutch — not machine-translated, but composed with the formality registers, technical vocabulary, and cultural conventions of each installer archetype. The Outreach Agent manages multi-channel execution across email, LinkedIn, and WhatsApp, handling replies autonomously when confidence is high and escalating to human judgment when it is not. And the Feedback Analyst closes the loop, comparing every real campaign outcome against its simulation forecast and tightening the model so that each deployment makes the next one sharper.

---

### How Simulation Works: The Digital Twin Grounding Methodology

The most important question any evaluator will ask is this: *how do we know the simulation's predictions are not hallucinated?* LLMs are excellent at role-playing conversation and terrible at calibrated probability estimation. Asking a language model to produce a reply-rate percentage yields a number that feels plausible but has no empirical anchor. Our methodology therefore separates two jobs: the LLM role-plays conversational behavior, while **probabilities emerge from aggregation across hundreds of constrained simulation runs.** Every behavioral degree of freedom is bounded by real data before the LLM is invoked.

**Phase 1 — Behavioral Prior Extraction.** Before any simulation runs, the system ingests Sunlumo's existing sales assets: past email campaigns with known open, reply, and conversion outcomes; CRM deal records with won/lost flags, installer types, deal sizes, and countries; Intercom chat logs capturing real installer questions, objections, and language patterns; webshop order histories revealing purchase cadences and product affinities; Salesviewer visitor logs showing which companies browse which pages; and trade-show badge-scan follow-up results with known conversion rates. From these sources, the system extracts empirical base rates — not industry averages, not LLM estimates. A concrete example: *"German solo Elektromeister: historical email-1 reply rate 4.2% from 847 sends; email-2 reply rate 2.1% from 412 sends; average deal cycle 18 days; top objection categories: price at 38%, compatibility at 27%, existing supplier relationship at 19%."* These are hard constraints that the LLM cannot override.

**Phase 2 — Constrained Persona Construction.** Each of the six to eight installer archetypes is built from three layers, only one of which involves generative AI. The demographic shell — company size, location, legal form, certification type, employee count — is sourced directly from Cognism and national trade registers (Handelsregister, KvK, INSEE-SIRENE, KRS, Camera di Commercio). This is factual, not generated. The behavioral prior layer carries the empirical ranges from Phase 1 and operates as a hard cage: reply-rate baseline, channel preference, objection distribution, price sensitivity band. The psychographic and conversational layer is LLM-generated — communication style, formality register, cultural norms, the *how* of a reply — but it operates entirely within the constraints set by the first two layers. The LLM decides how an installer phrases a price objection. It does not decide whether they object. That rate comes from the prior.

**Phase 3 — Simulation as Aggregation.** For a given campaign, the Simulation Orchestrator Agent runs the full conversational sequence against each persona in the cohort. At each decision point — open, reply, object, convert — the persona agent makes a weighted random draw within its empirical prior range. The LLM role-plays the conversation that follows. After 500 parallel runs, the outcomes are simply counted: 42 replies from 500 personas yields an 8.4% predicted reply rate. 11 meetings booked yields a 2.2% meeting rate. The probability is descriptive, not generative. It is the emergent property of a counting exercise constrained by ground truth.

**Phase 4 — Retrodiction Calibration.** Before Sunlumo trusts the simulator on any future campaign, we prove it can reconstruct the past. Three to five historical campaigns with known, measured outcomes are rebuilt in the simulator — same audience profile, same copy, same sequence, same timing. The predicted reply rate is compared against the actual reply rate. If the system predicts 5.1% ± 1.8% and the actual was 4.8%, calibration is confirmed within the confidence interval. This is the methodological standard used in quantitative finance backtesting and epidemiological model validation. We are bringing it to B2B sales simulation for the first time.

**Phase 5 — Live Bayesian Updating.** Every real campaign outcome flows back through the Feedback Analyst Agent. Empirical priors are updated through Bayesian inference: new evidence weights the prior toward observed reality. After three campaigns, confidence intervals typically halve from ±2.1% to ±0.8%. After ten campaigns, they converge below ±0.5%. Sunlumo does not need to believe in LLM magic. They can watch the error between predicted and actual shrink on a dashboard, campaign over campaign, until the simulator knows their installer market better than any individual sales manager.

This five-phase methodology — extract, constrain, aggregate, retrodict, update — is the intellectual foundation of the entire system. The LLM is a tool for generating conversational fidelity. The truth lives in the priors, and the priors come from Sunlumo's own data.

---

### The System, Engine by Engine

**The Sales Workflow Builder** is the entry point: a visual DAG canvas where Sunlumo's team designs campaigns by dragging nodes — data sources, intelligence filters, a mandatory Simulation Node, content generators, channel selectors, wait timers, conditional branches, and human approval gates — and connecting them into sequences. Data source nodes ingest CRM exports, trade-register feeds, Shopware 6 cart-abandonment events, Salesviewer deanonymization triggers, trade-show badge scans, and uploaded documents. The canvas ships with three pre-built templates that map directly to Sunlumo's known workflows: post-trade-show multilingual follow-up (Intersolar badge scan → enrich → persona-match → simulate → deploy within six hours of the event closing), cart-abandonment recovery (Shopware 6 trigger → intent score → UWG-compliant existing-customer outreach in the installer's native language), and subsidy-triggered campaign activation (legislation change detection → affected-installer identification → simulation-optimized messaging → multi-channel deployment within 24 hours of a new KfW or Superbonus announcement). The Simulation Node sits as a mandatory gate on every campaign path. No sequence deploys without a forecast. No real euros are spent without a predicted outcome.

**The Synthetic Personalized Decision Engine** fuses data from every available source — legislative signals, contact purchase history, forum activity, trade-register updates, and live intent telemetry — into a unified installer profile that drives personalization at scale. The engine does not merely append a first name to a template. It queries the solar knowledge graph to determine product compatibility, checks subsidy eligibility by region, selects the appropriate language and channel, and surfaces the most relevant hook for each individual installer. A Research Agent operates continuously in the background, monitoring photovoltaikforum.com and trade press for installer sentiment and emerging topics, tracking competitor pricing and product launches, and scraping legislation portals for changes to KfW 442, EEG, Superbonus, MaPrimeRenov', and Poland's "My Electricity" program. Signal delivery is both scheduled (weekly market intelligence briefs, pre-campaign enrichment runs) and push-based (real-time alerts when legislation changes or high-intent installer clusters are detected). A conversational interface allows Sunlumo's team to query the knowledge base directly: *"Which of our Bavarian installer partners have not ordered batteries in the last six months and are located in KfW-enhanced subsidy zones?"*

**The Outreach Pipeline** executes only after simulation is complete and the human approval gate has been passed. It manages multi-channel sequences across email, LinkedIn, and WhatsApp Business API — each channel governed by country-specific compliance presets, rate-limiting awareness, and cultural appropriateness. The CopyWriter Agent generates native-language copy in German, Italian, French, Spanish, Polish, and Dutch — not machine-translated from English, but composed from the ground up with correct formality registers (the Du/Sie distinction in German is non-negotiable), sector-specific vocabulary, and cultural conventions of the installer trade in each market. Smart follow-up logic reads and classifies every reply: interested, objection, not-now, unsubscribe, out-of-office. Objections are handled autonomously when the system's confidence exceeds threshold; ambiguous or high-stakes replies are escalated to a human with full conversational context. Every interaction is logged to CRM. Loss and success metrics — sent, delivered, opened, replied, positive reply, objection breakdown, meeting booked, partner registered, first order — are tracked per country, per language, per persona cohort, and per campaign variant. Most critically, real outcomes are displayed alongside their simulation predictions, so the gap between forecast and reality is always visible and always shrinking.

**The Feedback Reactor** closes the learning loop. After every campaign, the Feedback Analyst Agent compares predicted versus actual at every funnel stage, updates behavioral priors through Bayesian inference, and detects calibration drift before it becomes material. It surfaces insights that are strategically actionable: *"WhatsApp-first sequences for Italian multi-tech installers outperform email-first sequences by a factor of 2.7 — updating channel-mix recommendations for all future IT campaigns."* It also powers the product-market fit backrun: by aggregating installer objections, compatibility questions, and feature requests across all campaigns, it detects product gaps — *"230 installers in Poland requested ≤5 kWh residential batteries this quarter, a capacity not in Sunlumo's current catalog"* — and market gaps — *"KfW subsidy increase triggered a 340% spike in Bavarian installer inquiries, but no dedicated landing page exists"* — giving Sunlumo not just a sales tool but a strategic intelligence layer for portfolio and expansion decisions.

---

### Why This Is Defensible

Our competitive analysis scored ten leading platforms — Artisan, 11x, Clay, Apollo, Outreach, Salesloft, Cognism, Amplemarket, Lemlist, and Humanlinker — against twelve capabilities critical to the European solar distribution use case. **Six rows of the matrix show every single incumbent at zero: pre-deployment campaign simulation, synthetic persona reply forecasting, solar and installer vertical product knowledge, distributor-to-installer ICP focus, trade-show badge ingestion, and Shopware or Salesviewer intent-signal integration.** These are not marginal feature gaps. They are categorical absences.

Moreover, no US-built agentic SDR ships UWG-compliant DACH outbound presets. The German requirement for explicit consent before B2B email — enforced by active data protection authorities — structurally disqualifies most American platforms from operating on German soil without legal workarounds. Our system ships country-by-country compliance presets with auto-generated Legitimate-Interest Assessments, Impressum automation, double-opt-in flows, and a court-grade consent ledger with timestamped audit trails. Compliance is not buried in a terms-of-service document. It is a visible dashboard that shows, before every campaign, the legal basis for outreach in each target country.

The combination — simulation-first architecture, Bayesian-grounded digital twins, native multilingual generation across six European languages, UWG and GDPR compliance as a shipped feature, and a solar-vertical knowledge graph covering product compatibility, certification requirements, and subsidy programs — creates a moat that no US generalist can clone in under eighteen months and no European generalist has the vertical depth to assemble. The only credible adjacent threats are Bravi, a YC-backed AI operating system for home-services businesses that could expand from fenestration into solar, and Turian.ai of Munich, which could pivot from inbound automation to outbound. Speed matters, and a twelve-to-twenty-four-month head start with deep vertical integration is sufficient to establish category dominance.

---

### The First Thirty Days

Our MVP wedge targets the warmest, fastest, and most compliant path to demonstrable ROI. We deploy in three phases: first, a cart-abandonment and cross-sell agent connected to Sunlumo's Shopware 6 webshop, operating exclusively on existing customer relationships and therefore fully UWG-compliant from day one. This delivers measurable conversion uplift within thirty days. Second, the post-trade-show workflow — Intersolar and EES badge scans ingested, enriched, persona-matched, simulated, and deployed as multilingual sequences within hours of each event closing. Third, Salesviewer deanonymization triggers driving personalized agentic follow-up to companies already browsing Sunlumo's site.

The simulation engine itself is productizable beyond Sunlumo. We envision "SalesLab" — a standalone campaign-testing SaaS sold to other European distributors and brand owners in adjacent verticals — with the Sunlumo engagement serving as the reference case. This is not a single-client services project. It is the foundation of a new category.

---

### Summary Architecture

The figure below captures the complete system. Data flows in from the left. The Supervisor Agent sits at the top, orchestrating. The Simulation Node is the mandatory gate before any deployment. The Feedback Reactor closes the loop on the right. And the entire surface is exposed to Sunlumo's team as a visual DAG canvas — no code, no configuration files, just a directed graph of agents and decisions that can be understood, audited, and trusted.

```
                          ┌──────────────────────────────┐
                          │      SUPERVISOR AGENT        │
                          │    Plans → Delegates →       │
                          │    Monitors → Adapts         │
                          └──────────────┬───────────────┘
                                         │
        ┌────────────────────────────────┼──────────────────────────────────┐
        │                                │                                  │
        ▼                                ▼                                  ▼
┌───────────────┐              ┌─────────────────┐              ┌───────────────────────┐
│   RESEARCH    │              │    SIMULATION   │              │     FEEDBACK          │
│   AGENT       │──────────────▶    ENGINE       │◀─────────────│     ANALYST           │
│               │              │                 │              │                       │
│ • Forum scrap │              │ • 500 synthetic │              │ • Bayesian prior      │
│ • Legislation │              │   installer     │              │   update              │
│ • Trade reg.  │              │   agents        │              │ • Drift detection     │
│ • Competitor  │              │ • Multi-step    │              │ • Predicted vs.       │
│ • Subsidy map │              │   sequences     │              │   actual comparison   │
│ • Intent sig. │              │ • A/B optimiser │              │ • Product-gap         │
└───────┬───────┘              │ • Confidence    │              │   detection           │
        │                      │   scoring       │              └───────────┬───────────┘
        │                      └───────┬─────────┘                          │
        │                              │                                    │
        ▼                              ▼                                    │
┌────────────────────────────────────────────────────────────────────┐      │
│                    VISUAL DAG ORCHESTRATION CANVAS                  │      │
│                                                                    │      │
│  ┌──────────┐   ┌──────────┐   ┌──────────┐   ┌──────────┐        │      │
│  │  DATA    │   │ FILTER & │   │SIMULATION│   │ OUTREACH │        │      │
│  │ SOURCES  │──▶│INTELLIGE.│──▶│   NODE   │──▶│ PIPELINE │───────────────┘
│  │          │   │          │   │(MANDATORY│   │          │        │
│  │ • CRM    │   │ • ICP    │   │  GATE)   │   │ • Email  │        │
│  │ • Shop   │   │ • Persona│   │          │   │ • LinkedIn│       │
│  │ • Badges │   │ • Subsidy│   │ Predicted│   │ • WhatsApp│      │
│  │ • Registers│  │ • Intent │   │ reply:   │   │ • Phone   │      │
│  │ • Forums │   │ • Lang.  │   │ 8.4%±2.1%│   │ • Follow- │      │
│  └──────────┘   └──────────┘   └────┬─────┘   │   up logic│      │
│                                     │         └──────────┘      │
│                          ┌──────────▼─────────┐                 │
│                          │  HUMAN APPROVAL    │                 │
│                          │  GATE              │                 │
│                          │  (review → approve)│                 │
│                          └────────────────────┘                 │
└──────────────────────────────────────────────────────────────────┘

  ◀──────────────── continuous Bayesian updating ──────────────────▶
```

**Data sources** feed the system. **Research Agent** monitors the world. **Intelligence filters** enrich and score every contact. **Simulation Node** is the mandatory gate — no campaign passes without a forecast, and every forecast is grounded in Sunlumo's own historical priors. **Human approval** gates deployment. **Outreach Pipeline** executes across channels in native languages. **Feedback Analyst** compares prediction to reality, updates priors through Bayesian inference, and tightens the model with every campaign. The **Supervisor Agent** orchestrates the whole. The DAG canvas makes the entire system visual, auditable, and operable by a sales team — not an engineering team.
