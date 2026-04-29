# Agentic Sales System — Animated Pitch Scenario

## For: Sunlumo Energy (Austria)
## Purpose: Video demo of an AI-driven B2B sales system for European battery storage distribution

---

## Overview

An animated product demo (~2.5 minutes) showing how an agentic AI sales system works end-to-end. The video uses a horizontal scrolling canvas with cards, connection lines, and agent visualizations. The viewer follows a left-to-right flow through 8 scenes.

### Visual Style (match Tempo payroll video)
- **Background**: Warm light gray (#eeecea) with subtle grid lines
- **White cards**: Clean white, 14px rounded corners, subtle shadow — used for data, installers, metrics
- **Dark cards**: Pure black (#111), white text, teal accent values — used for engines/systems
- **Agent cards**: White with 4px teal left border, teal avatar square, pulsing green status dot — distinctive from regular cards
- **Green pills**: Teal (#3ecf8e) background, white text — used for completed actions/status
- **Connection lines**: Animated bezier curves in teal, drawing progressively left-to-right with small arrowhead at endpoint
- **Feedback lines**: Dashed, peach/orange color (#e8956a), drawing right-to-left (backward)
- **Fleet dots**: 32px teal circles with agent number, subtle glow shadow
- **Scene label**: Large frosted glass pill at top center with step number in teal: "Step 3 — Spin Up Agent Fleet"
- **Bottom bar**: Frosted glass strip: "Agentic Sales System · 24 AI Agents · Built for Sunlumo Energy"
- **Cursor**: Black pointer arrow with white stroke, animates smoothly to simulate user interaction
- **Camera**: Smooth horizontal pan (2s ease-in-out) following the flow left-to-right. One zoom-out moment in Scene 8.

### Animation Principles
- Elements fade in (opacity 0→1, ~0.5s)
- Connection lines draw progressively using animated bezier curves (~0.8s)
- Counter values animate up (e.g., 0 → 12,847 over 1.2s)
- When multiple lines connect to the same card, spread endpoints vertically along the edge (don't converge to single point)
- Old elements stay visible as camera pans past — the full flow accumulates on canvas
- No elements disappear between scenes

---

## Context: Sunlumo Energy

- **Company**: Sunlumo Energy, Perg, Austria
- **Business**: Official Gold Distributor for Sigenergy in Europe
- **Products**: SigenStor (home battery storage), SigenStack (commercial/industrial), SigenMicro (microinverters)
- **Markets**: Austria, Germany, Czech Republic, Hungary, Croatia, Slovenia, Serbia (7 countries)
- **Target customers**: Solar installers, electricians, EPC firms (B2B only)
- **Goal**: Scale from current revenue to €100M
- **Problem**: 4 sales reps cannot cover 7 countries. Traditional hiring is too slow.
- **Solution**: AI-driven autonomous sales system with 24 agents covering all markets

---

## SCENE 1: Connect Your Data Sources
**Label**: "Step 1 — Connect Your Data Sources"
**Duration**: ~12 seconds
**Camera**: Centered on workspace area

### Elements

**Agent Workspace** (dark card, center):
- Title: "Agent Workspace"
- Subtitle: "Connect your data · Power your agents"
- Row: Sources → counter animates 0 to 5
- Row: Records → counter animates 0 to 12,847
- Lock icon: ⚡

**"Add Sources" button** (dark pill, right of workspace):
- Text: "S Add Sources"
- Connected to workspace with thin gray line
- Cursor moves to it and clicks (peach border highlight)

**5 Data Source pills** (teal, stacked vertically, left side):
Each appears one by one, with a teal bezier line drawing from pill → workspace left edge. Endpoints spread vertically along workspace edge (-60px to +60px from center).

| # | Source | Detail label below |
|---|--------|--------------------|
| 1 | CRM · 3,241 Deals | win_rate: 34%  avg_deal: €38K |
| 2 | Emails · 8,102 Threads | objections · follow-ups · pricing |
| 3 | Product Catalog | SigenStor · SigenStack · SigenMicro |
| 4 | Monday Notes | pipeline_notes · deal_stages |
| 5 | AI Meeting Notes | call_transcripts · action_items |

Detail labels are monospace text with white semi-transparent background for readability against the grid.

### Animation Sequence
1. Workspace card fades in
2. "Add Sources" button fades in, gray connector draws
3. Cursor moves to button, button gets peach border highlight
4. Source pills appear one by one (0.35s gap), each with:
   - Pill fades in
   - Detail label fades in
   - Teal bezier line draws from pill right edge → workspace left edge
   - Sources counter increments
5. Records counter animates 0 → 12,847
6. Hold 2s

---

## SCENE 2: Build Sales Workflow
**Label**: "Step 2 — Build Sales Workflow — Each Step = An Agent"
**Duration**: ~15 seconds
**Camera**: Pan right to workflow area

### Elements

**Connector line**: Teal bezier from Workspace right edge → Workflow Builder left edge

**Sales Workflow Builder** (dark card):
- Title: "Sales Workflow Builder"
- Subtitle: "Each step = an agent role"
- Row: Steps → counter 0 to 8
- Row: Agent Roles → counter 0 to 8
- Lock icon: 🔧

**8 Workflow Step Nodes** (white bordered cards, arranged in 3 rows):

Row 1 (top, y~80):
| Node | Icon + Label | Agent Role (teal subtitle) |
|------|-------------|---------------------------|
| 1 | 🔍 Lead Discovery | Prospector Agent |
| 2 | 📊 Enrichment | Enricher Agent |
| 3 | 🎯 Intent Scoring | Scorer Agent |

Row 2 (middle, y~260):
| Node | Icon + Label | Agent Role |
|------|-------------|------------|
| 4 | ✍️ Personalization | Writer Agent |
| 5 | 📤 Outreach | Outreach Agent |
| 6 | 🔄 Follow-up | Nurture Agent |

Row 3 (bottom, y~430):
| Node | Icon + Label | Agent Role |
|------|-------------|------------|
| 7 | 📋 Qualify + Book | Qualifier Agent |
| 8 | 🤝 Close / Handoff | Closer Agent |

**"8 steps · 8 agent roles"** (teal pill, appears at end)

### Connections Between Steps
- Builder → Node 1, Builder → Node 4 (two branches from builder)
- Node 1 → Node 2 → Node 3 (top row, left to right)
- Node 4 → Node 5 → Node 6 (middle row, left to right)
- Node 3 → Node 7 (top-right down to bottom), Node 6 → Node 7 (middle-right down to bottom)
- Node 7 → Node 8 (bottom row)

### Animation Sequence
1. Connector line draws from Workspace → Builder
2. Builder card fades in
3. Step nodes appear one by one (0.3s gap), counters increment
4. Connection lines draw between steps (0.15s per line)
5. All nodes turn green/teal (active state: teal border + teal background tint)
6. "8 steps · 8 agent roles" pill appears
7. Hold 1.8s

---

## SCENE 3: Spin Up Agent Fleet
**Label**: "Step 3 — Spin Up Agent Fleet — DACH Market"
**Duration**: ~15 seconds
**Camera**: Pan right to agent fleet area

### Elements

**Connector line**: Teal bezier from "8 steps" pill → Orchestrator

**Agent Orchestrator** (dark card):
- Title: "Agent Orchestrator"
- Subtitle: "Spinning up fleet for DACH market"
- Row: Fleet Size → counter 0 to 10
- Row: Status → text changes from "Deploying..." to "All Online ✓"
- Lock icon: 🧠

**10 Agent Cards** (white cards with teal left border, arranged in 2 columns of 5):

| Agent | Name | Role Description |
|-------|------|-----------------|
| 01 | DE-01 Prospector | Bavaria · Lead Discovery |
| 02 | DE-02 Prospector | NRW · Lead Discovery |
| 03 | DE-03 Enricher | Company Data · Contacts |
| 04 | DE-04 Scorer | Intent Signals · 6sense-style |
| 05 | DE-05 Writer | German · Personalization |
| 06 | DE-06 Email Agent | Outreach · Deliverability |
| 07 | DE-07 LinkedIn Agent | Connect · InMail |
| 08 | DE-08 Nurture Agent | Follow-up · Cadence |
| 09 | DE-09 Qualifier | Score Replies · Book |
| 10 | DE-10 Closer | Handoff to Sales Team |

Each agent card has:
- Teal square avatar with agent number (e.g., "01")
- Bold name (14px)
- Gray role description (11.5px)
- Pulsing teal status dot (10px, animated glow)
- 4px teal left border

**"Fleet Online · 10 Agents Active"** (teal pill)

### Animation Sequence
1. Connector line from previous scene pill → Orchestrator
2. Orchestrator fades in
3. Agents appear one by one (0.25s gap):
   - Teal bezier line draws from Orchestrator right edge → Agent card left edge
   - Lines spread vertically along Orchestrator edge (offsets: -65 to +15px)
   - Fleet Size counter increments
   - Agent card fades in with pulsing dot
4. Status changes to "All Online ✓"
5. "Fleet Online" pill appears
6. Hold 2.2s

---

## SCENE 4: Simulate, Tune, Compare, Pick Best
**Label**: "Step 4 — Simulate → Tune → Re-Run → Compare → Pick Best"
**Duration**: ~25 seconds
**Camera**: Pan right to simulation area

This is the most important scene. It shows the iterative simulation process: run a workflow, see results, tune parameters, run again, compare, pick best.

### Elements

**Connector line**: Teal bezier from Orchestrator → Simulation Engine

**Simulation Engine** (dark card):
- Title: "Simulation Engine"
- Subtitle: "Run multiple instances · Compare · Pick best"
- Row: Simulations Run → counter 0 to 3
- Row: Agents Per Run → "10" (static)
- Row: Best Result → starts "—", ends "Sim #3 · 34%"
- Lock icon: 🎮

**Configuration Panel** (white card, below engine):
- Title: "⚙ Configuration"
- Subtitle: "Click parameters to tune between runs"
- Row: Tone → "Professional" (stays same)
- Row: Cadence → starts "Day 1, 3, 7, 14", changes to "Day 1, 3, 5, 10" (row flashes teal when edited)
- Row: Data Sources → starts "CRM + Email", changes to "CRM + Email + Notes" (row flashes teal when edited)
- Row: Language → "DE · Auto" (stays same)

Each row has an ID so it can be individually highlighted when edited. Editing animation: row background flashes bright teal (0.2s), value text changes, row stays with soft teal background (indicating "changed").

**"Run Simulation →" button** (dark pill, below config):
- Cursor moves to it and clicks before each sim run
- Gets peach border highlight on click

**3 Simulation Result Cards** (white cards with metric rows, stacked vertically to the right):

| Card | Title | Reply Rate | Meetings | Projected Win | Diff Tag |
|------|-------|-----------|----------|---------------|----------|
| Sim #1 | Sim #1 · Baseline | 22% | 12 | 18% | "Baseline: default parameters" |
| Sim #2 | Sim #2 · Faster Cadence | 31% | 19 | 26% | "Changed: Cadence → Day 1, 3, 5, 10" |
| Sim #3 | Sim #3 · +Data Sources ★ | 41% | 28 | 34% | "Added: AI Meeting Notes + Monday" |

Sim #3 gets a teal border + glow shadow when marked as best. Its metric values are in teal color.

Each result card has a **diff tag** (small teal-background pill at bottom) explaining what parameter change led to that result.

**3 Agent Fleet Dots per simulation** (small teal circles, positioned left of each result card):
- Sim 1: A1, A2, A3
- Sim 2: A4, A5, A6
- Sim 3: A7, A8, A9

**"Sim #3 selected · Deploying best workflow"** (teal pill, appears at end)

### Animation Sequence

**Run 1 — Baseline:**
1. Simulation Engine fades in
2. Configuration panel fades in (all default values)
3. "Run Simulation →" button fades in
4. Cursor moves to Run button, button highlights
5. Sim count: 0 → 1
6. Agent dots A1, A2, A3 appear (pulsing)
7. Teal line draws from Engine → Result Card #1
8. Result Card #1 fades in
9. Metrics populate: Reply 22%, Meetings 12, Win 18%
10. Diff tag appears: "Baseline: default parameters"
11. Hold 1.2s

**Tune 1 — Edit cadence:**
12. Cursor moves to Cadence row in config panel
13. Cadence row background flashes bright teal (0.2s "editing" state)
14. Value changes: "Day 1, 3, 7, 14" → "Day 1, 3, 5, 10"
15. Row stays soft teal ("edited" state)
16. Hold 0.3s

**Run 2 — Faster Cadence:**
17. Cursor moves to Run button
18. Sim count: 1 → 2
19. Agent dots A4, A5, A6 appear
20. Teal line draws from Engine → Result Card #2
21. Result Card #2 fades in
22. Diff tag appears: "Changed: Cadence → Day 1, 3, 5, 10"
23. Metrics populate: Reply 31%, Meetings 19, Win 26%
24. Hold 1.2s

**Tune 2 — Add data sources:**
25. Cursor moves to Data Sources row
26. Sources row flashes bright teal
27. Value changes: "CRM + Email" → "CRM + Email + Notes"
28. Row stays soft teal
29. Hold 0.3s

**Run 3 — More data = Best:**
30. Cursor moves to Run button
31. Sim count: 2 → 3
32. Agent dots A7, A8, A9 appear
33. Teal line draws from Engine → Result Card #3
34. Result Card #3 fades in
35. Diff tag appears: "Added: AI Meeting Notes + Monday"
36. Metrics populate (in teal color): Reply 41%, Meetings 28, Win 34%
37. Hold 0.6s

**Mark best:**
38. Result Card #3 gets teal border + glow shadow
39. Engine "Best Result" changes to "Sim #3 · 34%"
40. "Sim #3 selected" pill appears
41. Hold 2s

---

## SCENE 5: Outreach Agents Deliver Across Channels
**Label**: "Step 5 — Outreach Agents Deliver Across Channels"
**Duration**: ~15 seconds
**Camera**: Pan right to outreach area

### Elements

**Connector line**: Teal bezier from Simulation Engine → Outreach Fleet

**Outreach Fleet** (dark card):
- Title: "Outreach Fleet"
- Subtitle: "Agents delivering across channels"
- Row: Active Agents → counter 0 to 6
- Row: Channels → counter 0 to 4
- Lock icon: 📤

**4 Channel Nodes** (white bordered cards, stacked vertically):
| Channel | Icon | Subtitle |
|---------|------|----------|
| Email | 📧 | DE · CS · HU |
| LinkedIn | 💼 | Connect + InMail |
| Phone | 📞 | Follow-up calls |
| WhatsApp | 💬 | Quick touch |

Lines from Outreach Fleet → each channel, spread vertically along Fleet's right edge.

**3 Agent-to-Installer Chains** (Agent card → Installer card):

Chain 1 (Email channel):
- Agent: DE-06 → Weber (Email DE · Sent) [pulsing dot]
- Line: Channel → Agent → Installer
- Installer: Weber Solartechnik 🇩🇪 (Munich · SigenStor prospect)
- Status updates to: "Opened 3× · Clicked pricing"

Chain 2 (LinkedIn channel):
- Agent: DE-07 → EnergiePro (LinkedIn CS · Connect) [pulsing dot]
- Installer: EnergiePro s.r.o. 🇨🇿 (Prague · Electrician)
- Status updates to: 'Replied: "interested"'

Chain 3 (Phone channel):
- Agent: DE-08 → Green Power (Phone HU · Follow-up) [pulsing dot]
- Installer: Green Power Kft. 🇭🇺 (Budapest · Installer)
- Status updates to: "Meeting booked Jun 12"

### Animation Sequence
1. Connector line from Sim Engine → Outreach Fleet
2. Outreach Fleet fades in, counters animate
3. Channel nodes appear one by one with connecting lines
4. For each of 3 chains:
   - Line from channel → agent card
   - Agent card fades in
   - Line from agent → installer card
   - Installer card fades in
   - Status text updates to engagement result
5. Hold 2s

---

## SCENE 6: Feedback Loop — All Agents Learn
**Label**: "Step 6 — Feedback Loop — All Agents Learn in Real-Time"
**Duration**: ~14 seconds
**Camera**: Pan right to feedback area

### Elements

**Connector line**: Teal bezier from Outreach Fleet → Feedback Reactor

**Feedback Reactor** (dark card):
- Title: "Feedback Reactor"
- Subtitle: "All agents recalibrating from results"
- Row: Patterns Learned → counter 0 to 14
- Row: Win Rate Δ → "+12%"
- Lock icon: 🔄

**3 Result Items** (to the right of reactor, spread vertically):

| Type | Element | Text | Detail line below |
|------|---------|------|-------------------|
| Won | Teal pill | Won: Weber · €42K | Pattern: local_warehouse + 48hr_delivery → amplified to all agents |
| Stalled | Teal pill | Stalled: EnergiePro | Action: DE-08 switching to phone follow-up |
| Lost | Dark pill | Lost: Kovács · "has supplier" | Learning: new objection handler → deployed to all Writer Agents |

Lines from Reactor → each result, spread along Reactor's right edge (-40, 0, +40px).

**Feedback line**: Dashed peach/orange bezier from Lost pill back → Reactor bottom edge (drawing right-to-left, representing learning flowing backward into the system)

**Re-scoring pill** (muted teal):
"↩ Re-scoring 89 prospects · All 10 agents updated in real-time"

### Animation Sequence
1. Connector from Outreach → Reactor
2. Reactor fades in
3. Won pill + detail line appear, with teal line from reactor
4. Stalled pill + detail line appear
5. Lost pill + detail line appear
6. Counters animate (Patterns: 14, Win Rate Δ: +12%)
7. Dashed peach feedback line draws from Lost → Reactor (backward)
8. Re-scoring pill appears
9. Hold 2.2s

---

## SCENE 7: Expert Agents Review & Enhance
**Label**: "Step 7 — Expert Agents Review & Enhance Before Deploy"
**Duration**: ~14 seconds
**Camera**: Pan right to expert review area

### Elements

**Connector line**: Teal bezier from Feedback Reactor → Expert Review

**Expert Agent Assembly** (dark card):
- Title: "Expert Agent Assembly"
- Subtitle: "Specialized agents review + enhance"
- Row: Experts → counter 0 to 4
- Row: Enhancements → counter 0 to 12
- Lock icon: 👥

**4 Expert Agent Cards** (agent cards with colored accents, stacked vertically):

| # | Avatar Color | Avatar Icon | Name | Suggestion |
|---|-------------|-------------|------|------------|
| 1 | Orange (#e8956a) | 🎯 | Strategy Agent | Add competitor displacement playbook |
| 2 | Blue (#3b82f6) | 🌍 | Market Intel Agent | Add PV Austria installer registry |
| 3 | Purple (#8b5cf6) | 📝 | Language Agent | Czech vykání → +18% reply rate |
| 4 | Teal (#14b8a6) | ⚖️ | Compliance Agent | GDPR OK · all 7 markets verified |

Each expert card has:
- Colored left border matching avatar color
- Large avatar (40px) with emoji icon
- 15px name
- 12px suggestion text as role
- Pulsing status dot in matching color

Lines from Expert Review → each expert, spread along right edge (-55, -18, +18, +55px).

**"12 enhancements applied · Ready to deploy →"** (teal pill)

### Animation Sequence
1. Connector from Reactor → Expert Review card
2. Expert Review fades in
3. Expert agents appear one by one (0.5s gap):
   - Teal line draws from review card → expert agent
   - Expert counter increments
   - Agent card fades in with pulsing dot
4. Enhancement counter animates 0 → 12
5. "Ready to deploy" pill appears
6. Hold 2s

---

## SCENE 8: Deploy to Production
**Label**: "Step 8 — Deploy to Production — 24 Agents · 7 Markets"
**Duration**: ~22 seconds
**Camera**: Pan to deployment area

### Elements

**Connector line**: Teal bezier from "Ready to deploy" pill → Sales Shuttle

**24 Fleet Dots** (teal circles with agent numbers, arranged in 3 rows):

Row 1 — DACH Fleet (10 dots): agents 01-10
Label: "🇦🇹🇩🇪 DACH Fleet · 10 agents"

Row 2 — CEE Fleet (8 dots): agents 11-18
Label: "🇨🇿🇭🇺🇸🇰 CEE Fleet · 8 agents"

Row 3 — Balkan Fleet (6 dots): agents 19-24
Label: "🇭🇷🇸🇮🇷🇸 Balkan Fleet · 6 agents"

Dots appear one by one rapidly (60ms gap).

**Sales Shuttle** (dark card, below fleet dots):
- Title: "Sales Shuttle · Deploy"
- Subtitle: "Best workflow → production agents"
- Row: Selected → "DACH Workflow A · Enhanced"
- Row: Markets → counter 0 to "7 / 7"
- Row: Live Agents → counter 0 to 24
- Lock icon: 🚀

**Live Production Metrics Dashboard** (white card, to the right):
- Title: "Live Production Metrics"
- Subtitle: "24 agents · 7 markets · Real-time"
- Rows that animate through 4 time steps:

| Metric | Step 1 | Step 2 | Step 3 | Step 4 (final) |
|--------|--------|--------|--------|----------------|
| Pipeline | €180K | €620K | €1.4M | €2.4M |
| Conversion | 8% | 18% | 26% | 34% |
| Closed ✓ | 2 | 8 | 18 | 31 |
| Stalled ⏸ | 5 | 12 | 14 | 9 |
| Lost ✗ | 3 | 7 | 11 | 14 |
| Cost/Lead | €42 | €28 | €19 | €12 |

Each time step takes ~1.1s, all metrics animate simultaneously. Stalled is shown in peach/orange color. Lost in gray.

**"7 Markets · 24 Agents · Production"** (teal pill, appears at end)

### Animation Sequence
1. Connector from "Ready to deploy" pill → Shuttle area
2. Fleet dots appear rapidly (24 dots, 60ms each = ~1.4s)
3. Fleet labels appear (3 muted teal pills with flags)
4. Sales Shuttle card fades in
5. Selected text updates, Markets and Agents counters animate
6. Teal line from Shuttle → Dashboard
7. Dashboard fades in
8. Metrics animate through 4 time steps (4.4s total):
   - Pipeline grows from €180K to €2.4M
   - Conversion climbs from 8% to 34%
   - Closed deals increase from 2 to 31
   - Stalled peaks at 14 then drops to 9 (system learning)
   - Cost/Lead drops from €42 to €12
9. "Production" pill appears
10. Hold 3s

---

## End / Loop

After Scene 8 completes:
- Scene label fades out
- Cursor hides
- Hold 3 seconds
- All elements reset (hide, clear lines, reset counters)
- Loop back to Scene 1

---

## Full Element Inventory

### Card Types
| Type | CSS Class | Visual | Used For |
|------|-----------|--------|----------|
| White card | `.wc` | White bg, shadow, rounded | Data panels, installer cards, metrics |
| Dark card | `.dc` | Black bg, white text, teal values | Engines, systems, orchestrators |
| Agent card | `.ac` | White bg, teal left border, avatar, pulsing dot | Individual agents |
| Step node | `.sn` | White bg, thin border, turns teal when active | Workflow pipeline steps |
| Sim result | `.src` | White bg, optional teal border for "best" | Simulation comparison results |

### Pill Types
| Type | CSS Class | Visual | Used For |
|------|-----------|--------|----------|
| Green pill | `.gp` | Teal bg, white text | Completed actions, status |
| Muted pill | `.mp` | Light teal bg, dark teal text | Labels, tuning changes |
| Dark button | `.db` | Black bg, white text, optional peach border | Clickable actions |
| Hash label | `.tx` | Monospace, white bg chip | Technical details under pills |

### Other Elements
| Element | Visual | Used For |
|---------|--------|----------|
| Fleet dot `.fd` | 32px teal circle, glow | Agent fleet visualization |
| Activity log `.al` | 13px text with teal dot prefix, bold teal agent names | Real-time agent action feed |
| Lock icon `.lk` | 28px dark circle with teal border | Top-left of dark cards |

---

## Sunlumo-Specific Data Reference

### Products
- SigenStor 5kWh — Home storage
- SigenStor 10kWh — Home+ storage
- SigenStack — Commercial & Industrial battery
- SigenMicro — Microinverters

### Target Installer Companies (fictional but realistic)
- Weber Solartechnik GmbH — Munich, Germany 🇩🇪 (Solar installer)
- EnergiePro s.r.o. — Prague, Czech Republic 🇨🇿 (Electrician)
- Green Power Kft. — Budapest, Hungary 🇭🇺 (Solar installer)
- Kovács Elektro — (referenced as lost deal, "has supplier" objection)

### Markets (7 countries)
- DACH: Austria 🇦🇹, Germany 🇩🇪
- CEE: Czech Republic 🇨🇿, Hungary 🇭🇺, Slovakia 🇸🇰
- Balkan: Croatia 🇭🇷, Slovenia 🇸🇮, Serbia 🇷🇸

### Key Metrics Used
- CRM: 3,241 deals, 34% win rate, €38K avg deal
- Email archive: 8,102 threads
- Simulation results: Reply rates 22% → 31% → 41%
- Production: €2.4M pipeline, 34% conversion, 31 closed, €12 CPL
- Feedback: +12% win rate improvement, 14 patterns learned
- Language insight: Czech formal tone (vykání) → +18% reply rate
- Winning pattern: "Local warehouse (Perg) + 48hr delivery"
- Top objection: "Already has supplier" → counter with switching cost analysis

### Agent Fleet (24 total across 3 regions)
- DACH Fleet: 10 agents (DE-01 through DE-10)
- CEE Fleet: 8 agents (11-18)
- Balkan Fleet: 6 agents (19-24)

### Agent Roles (8 types)
1. Prospector — Regional lead discovery
2. Enricher — Company data + contacts
3. Scorer — 6sense-style intent scoring
4. Writer — Language-specific personalization
5. Email Agent — Outreach + deliverability
6. LinkedIn Agent — Connect + InMail
7. Nurture Agent — Follow-up cadence
8. Qualifier — Score replies + book meetings
9. Closer — Handoff to human sales team
10. (Expert types): Strategy, Market Intel, Language, Compliance
