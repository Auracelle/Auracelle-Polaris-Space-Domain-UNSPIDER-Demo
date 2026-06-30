# Auracelle Polaris · UN-SPIDER Edition · Space Governance Wargaming Intelligence Platform

**Auracelle Polaris** is an interactive, browser-based wargaming simulation for space capacity governance decision-making under strategic pressure. The **UN-SPIDER Edition** integrates Earth Observation data governance and disaster risk reduction into the core simulation, directly supporting the 11th Annual UN-SPIDER Conference on Resilient Futures and WSIS Framework goals.

## 🎮 Play the Wargame

**[Launch Polaris UN-SPIDER Edition](index.html)**

**Access Code**: `UNSPIDER2026!`

## Overview

Polaris models how nations, military organizations, alliances, humanitarian agencies, and commercial operators make governance decisions when space systems are under strategic pressure—including scenarios where GPS signals degrade, satellites are threatened, Earth Observation data becomes unavailable, weather data is lost, or coordination channels are too slow to act.

### Six Crisis Scenarios

1. **Kessler Cascade Threshold** – Orbital debris collision generates cascade potential; liability unresolved under Outer Space Treaty Article VI.
2. **GPS Constellation Degradation** – Jamming and interference degrade coverage; alternative PNT activation is slow and untested at scale.
3. **Anti-Satellite Weapons Test** – A state conducts a destructive ASAT test with no binding notification or accountability requirement.
4. **Megaconstellation Governance Failure** – Commercial deployment outpaces spectrum and orbital slot governance; emerging spacefaring states lack equitable access.
5. **Allied Coordination Breakdown** – Interagency and allied coordination channels are too slow; execution capacity lags despite existing treaties and norms.
6. **Earth Observation Data Access Deadlock** *(UN-SPIDER Focus)* – A humanitarian emergency requires real-time satellite EO data, but geopolitical tensions have blocked multilateral open-access protocols. Space-faring nations control distribution; vulnerable nations cannot access data fast enough.

### How to Play (8 Steps)

1. **Log in** with your email and access code: `UNSPIDER2026!`
2. **Select a Space Crisis Scenario** – Choose from six governance challenges
3. **Review the Governance Challenge** – Examine ownership, responsibility, treaties, boundaries, and authority gaps
4. **Assess Actor Positions** – Understand the interests, capabilities, incentives, and constraints of all stakeholders
5. **Make a Policy or Operational Move** – Choose from unilateral, bloc-level, or multilateral governance actions (up to 4 moves per scenario)
6. **Agentic AI Stress-Tests the Move** – AI actor-agents simulate stakeholder responses: cooperation, delay, escalation, defection, or coalition strain
7. **Review the Cross-Track Diagnostic Score** – Compare Governance Capacity with Operational Resilience to see alignment
8. **Identify Gaps and Apply Corrective Action** – Use recommendations to improve institutional readiness, policy quality, and governance-resilience alignment

### Key Mechanic: Contested Negotiation Table

When unilateral or bloc-limited moves expose a coalition fracture or governance deadlock, the **Contested Negotiation Table** unlocks as a 4th move option. This forces a binding multi-actor session where all parties (US, allies, China, commercial operators, international institutions, etc.) must negotiate a real compromise. It is the only mechanic that resolves multilateral deadlock rather than just managing unilateral pressure.

### Scoring & Insights

**Computational Decision Intelligence (CDI)** across two independent tracks:
- **Governance Track**: Treaties, norms, institutional coordination, diplomatic frameworks (7 dimensions)
- **Resilience Track**: Backup systems, continuity of services, commercial-government integration, operational hardening (9 dimensions)

**Cross-Track Diagnostic**: Measures imbalance between governance capacity and operational resilience, surfacing strategic gaps before crisis.

**Integrated Leadership Score (ILS)**: Maximized when both tracks are high and balanced — integration, not specialization, is the strategic requirement.

**Space Governance Maturity Level (M·0 to M·4)**: Progression from pre-governance through established binding protocols.

---

## UN-SPIDER Edition Features

### Earth Observation Data Access Scenario (Scenario 06)

Directly addresses UN-SPIDER's mandate: **space-based disaster risk reduction through governance**.

**Scenario Context**:
- A climate catastrophe (drought, flooding) requires real-time satellite EO data
- Geopolitical tensions block multilateral open-access protocols
- Space powers control data distribution; vulnerable nations lack rapid access
- GeoAI models exist (Prithvi, Satlas) but technical capacity gaps persist

**Four Playable Moves**:
- **Invoke International Charter** – Activate "Space and Major Disasters" mechanism for emergency data sharing
- **Deploy Open-Source GeoAI** – Release foundation models publicly for local processing
- **Establish Open Data Norms** – Use WSIS Action Lines C1 & C6 to push binding agreements
- **Contested Negotiation Table** – Force multilateral session resulting in binding 2-hour open-access protocol during humanitarian emergencies

**Intelligence Findings**:
- Data sovereignty paradox: EO is public good but controlled privately/nationally
- Capacity mismatch: Open data means nothing without technical infrastructure
- Institutional deadlock: Norms and institutions both fail when urgency and equity collide

**Recommendations** (aligned with WSIS Action Lines):
- Emergency EO Protocol with binding 2-hour open access during declared emergencies
- Capacity-building investment in least-developed countries (20% of EO infrastructure budgets)
- WSIS C1 (information access) & C6 (enabling environment) implementation into UNDRR governance
- Regional data hubs through UN-SPIDER regional support offices

### WSIS Action Lines & SDG Alignment

The UN-SPIDER scenario explicitly supports:

**WSIS Action Lines**:
- **C1**: Role of governments and all stakeholders in the information society (data access governance)
- **C5**: Building confidence and security in use of ICTs (data security during emergencies)
- **C6**: Enabling environment (institutional capacity for EO data sharing)
- **C7**: ICT applications: e-government, e-business, e-learning, e-health, e-environment, e-agriculture, e-science
- **C10**: Ethical dimensions (equity in data access)
- **C11**: International and regional cooperation (multilateral space governance)

**UN Sustainable Development Goals**:
- **SDG 13**: Climate Action (EO for climate monitoring)
- **SDG 1 & 15**: No Poverty, Life on Land (disaster risk reduction in vulnerable nations)
- **SDG 17**: Partnerships for the Goals (multilateral space governance)

---

## Technical Specifications

### Architecture

- **Framework**: Vanilla JavaScript (no external dependencies except Google Fonts)
- **Runtime**: Browser-based, client-side only
- **Data**: No data collection, transmission, or storage beyond sessionStorage
- **Compatibility**: Modern browsers (Chrome, Firefox, Safari, Edge)
- **Accessibility**: WCAG 2.1 AA compliant

### Security

- **Client-side only**: No backend servers, no external API calls
- **No authentication backend**: Session-based via browser sessionStorage
- **Access control**: Simple access code (UNSPIDER2026!) for conference gating
- **Data privacy**: Zero data collection; all gameplay is local to the browser

### Performance

- **Page load**: < 2 seconds (4.4 MB single HTML file)
- **Interaction latency**: < 100ms for all user interactions
- **Browser support**: IE11+ (with graceful degradation)

---

## For UN-SPIDER 2026 Conference Use

### Quick Start for Conference Facilitators

1. **Deploy** this GitHub Pages repository or host the HTML file on your conference website
2. **Share the link** with participants (e.g., at conference sessions, workshops)
3. **Participants log in** with email + `UNSPIDER2026!`
4. **Select Scenario 06** (Earth Observation Data Access Deadlock) for UN-SPIDER-specific governance exploration
5. **Facilitate discussion** on how unilateral/bloc moves fail to resolve data governance deadlock
6. **Highlight the outcome** of the Contested Negotiation Table: binding protocols emerge from multilateral pressure

### For Presentations & Workshops

- **Duration**: 15–20 minutes per scenario (4 moves + discussion)
- **Group size**: 1–50+ participants (can play independently or collaboratively)
- **Equipment**: Web browser, no special software or plugins required
- **Learning outcomes**:
  - How space governance interacts with Earth Observation and disaster risk reduction
  - Why multilateral mechanisms (like negotiation tables) resolve deadlock that unilateral moves cannot
  - How WSIS Action Lines and UNDRR priorities map to operational space governance
  - Strategic trade-offs between speed (resilience) and legitimacy (governance)

### Access Code Management

- **Default access code**: `UNSPIDER2026!`
- **To customize for future events**: Edit line in JavaScript (around line 1005):
  ```javascript
  if(code === 'UNSPIDER2026!'){
  ```
  Replace `'UNSPIDER2026!'` with your custom code.

---

## About Auracelle AI Governance Labs

Auracelle designs governance stress-testing simulations that expose decision-making gaps under pressure. Our research focuses on the intersection of AI governance, simulation methodology, and decision-making under uncertainty.

**Founder & Principal Investigator**: Grace-Alice Evans  
**Research Supervisor**: Dr. John Curry (Bath Spa University)  
**Institutional Affiliations**:
- Non-Resident Senior Fellow, UC Berkeley Center for Long-Term Cybersecurity (CLTC)
- Technical Role Member, NATO STO SAS-219 (Disruptive Capabilities, Digitally-Enabled Wargaming, Diplomacy)

**Certifications & Background**: 
- PMP, ITIL Expert, CMMI v2, Security+, CISA, CISSP, CISM, CRISC
- 20+ years in government, defense, and civil infrastructure governance
- CIA, DHS OCIO, US Army INSCOM, SFO International Airport, MDOT

---

## The Auracelle Simulation Suite

Polaris is part of the **Auracelle Simulation Suite** for AI governance:

- **Auracelle Charlie / Fault Line** – Contested Negotiation Table for AI governance policy (California SB-53 whistleblower protections)
- **Auracelle Orion** – Cybersecurity governance wargaming
- **Auracelle Lyra** – Multi-domain governance (nuclear, space, energy, biotech, AI)
- **Auracelle Delphi** – Cognitive warfare and neurotechnology diplomacy
- **Auracelle Polaris** – Space governance wargaming (this platform)
- **Auracelle Bach** – Multi-agent actor network (foundational research baseline)

---

## More Information

**Auracelle Platform**: https://auracelle.github.io/Auracelle-AI-Governance-Labs-Platform-Comms-Public

**Full Auracelle Suite**: https://auracelle.github.io/Auracelle-Suite-AI-Governance-Labs/

**LinkedIn**: https://www.linkedin.com/in/grace-alice-evans-5a9632a3

**Contact**: grace.evans@auracelle.ai

---

## License

Auracelle Polaris is proprietary software with academic and institutional use exceptions. See [LICENSE](LICENSE) for full terms.

## Citation

For academic publications and research, please cite Polaris using one of the formats in [CITATION.md](CITATION.md).

## Security & Responsible Disclosure

See [SECURITY.md](SECURITY.md) for security policy, responsible disclosure procedures, and privacy guarantees.

---

**Auracelle AI Governance Labs · Polaris UN-SPIDER Edition v2.0**  
*Wargaming the Governance Asynchronously™*

**Keynote**: Space is a new domain. It will require creative governance that does not yet exist. Polaris helps you design it.
