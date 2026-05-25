# Cross-Domain Queries

The real power of MCP servers isn't any single data source — it's what happens when you connect them. With 40+ servers spanning government, science, economics, geography, security, and transit, an LLM can chase a question across domains in a single conversation.

No ETL pipeline. No data warehouse. Just questions that span domains, answered by following the data wherever it leads.

---

### Follow the money on a bill

> "Who benefits from this legislation, and are they paying for it?"

**Congress** → **OpenFEC** → **SEC EDGAR** → **OpenStates** → **Hacker News**

Trace a piece of legislation from introduction to the financial interests behind it. Cross-reference a bill's sponsors with their top donors, check whether those donors filed relevant 10-Ks, and see if matching bills appeared in state legislatures.

> **Real data:** Cantwell's top employer-donors — T-Mobile $99K, Microsoft $75K, Amazon $52K, Meta $20K — all with AI regulation stakes. 678 state-level AI bills active. 134-comment HN thread on a federal AI regulation ban.

---

### Drug safety investigation

> "What's the full story on this compound — from molecule to market failure?"

**PubChem** → **OpenFDA** → **ClinicalTrials.gov** → **PubMed** + **bioRxiv** → **SEC EDGAR** → **WHO**

Start from a chemical compound and follow the trail: what did the trials show, what adverse events were reported post-market, did the company disclose anything material, and what does the global health data say?

> **Real data — semaglutide (Ozempic):** 11,220 FDA nausea reports. 683 clinical trials, including Novo Nordisk's 600K-patient pancreatic cancer study. 603 PubMed safety papers. bioRxiv preprints showing it reduces fentanyl self-administration in rats and may protect against vascular dementia — neither on anyone's Ozempic radar. WHO global obesity context: US 42%, Japan 5.5%.

---

### CVE impact forensics

> "What actually happened after this vulnerability dropped?"

**NIST NVD** → **SEC EDGAR** → **Congress** → **arXiv** → **Hacker News**

Go beyond the CVSS score. Check whether the affected vendor disclosed a breach, whether the vulnerability triggered legislative action, what researchers published in response, and how the security community reacted.

> **Real data — Log4Shell (CVE-2021-44228):** CVSS 10.0. 447 SEC filings reference it — 19 8-Ks, 190 10-Ks, 238 10-Qs. Companies still citing it in 2025 filings. 9 arXiv papers on scanner behavior and mitigation. 698-point HN thread. The corporate disclosure footprint of a single CVE — hundreds of filings — is a number no vulnerability database tracks.

---

### Transit equity analysis

> "Who does the bus system actually serve?"

**OneBusAway** → **Census** → **OpenStreetMap** → **BLS** → **WSDOT** → **OpenStates**

Map transit service frequency against the demographics of the neighborhoods it serves. Overlay employment data, pedestrian infrastructure, and state-level funding decisions to build a picture of who benefits from public transit investment — and who doesn't.

> **Real data — Seattle's Rainier Beach:** 18 stops within 500m, all wheelchair-accessible. 23 cycleways within 1km (Chief Sealth Trail). 84 live toll rate entries across 5 express corridors that lower-income commuters can't afford. 1,827 WA state "transit funding" bills. The question isn't whether the data exists — it's that no one has connected it.

---

### Climate + biodiversity + economics

> "How is climate change reshaping this region's ecology and economy?"

**NOAA** → **GBIF** → **BrAPI** → **World Bank** → **Census** → **Earthquake** → **Eurostat**

Connect long-term climate data with biodiversity observations, agricultural output, and economic indicators. Track whether species ranges are shifting, whether crop yields are responding, and whether populations are moving in response.

---

### Historical event reconstruction

> "What did people know at the time, and what have we learned since?"

**Library of Congress** → **Wikipedia** → **Wikidata** → **OpenAlex** + **Crossref** → **OpenLibrary** → **Census**

Reconstruct an event from primary sources through modern scholarship. Read the newspaper coverage from the day it happened, cross-reference with structured data about the people and places involved, then trace the academic literature that followed.

---

### Pandemic signal detection

> "What early signals are converging right now?"

**WHO** → **CDC** → **bioRxiv** → **PubMed** → **ClinicalTrials.gov** → **GBIF** → **EIA** + **BLS**

Weak signals from different domains that individually mean nothing. WHO reports a bump in a respiratory illness indicator. A cluster of bioRxiv preprints appears. Clinical trials start registering. Vector species observations shift. Energy consumption patterns change. Convergence across independent data sources is the signal.

---

### "Should I move there?"

> "What does every public dataset say about this place?"

**Census** → **BLS** → **NWS** + **NOAA** → **Earthquake** → **OpenStreetMap** → **OneBusAway** → **Socrata** → **WSDOT**

Every dimension of livability, pulled from authoritative sources. Not a real estate listing's spin — the actual data on jobs, climate risk, transit, walkability, and neighborhood character.

---

### Research literature mapping

> "What's the state of this field — who's publishing, where, and what's not being studied?"

**OpenAlex** → **Crossref** → **PubMed** → **arXiv** → **bioRxiv** → **OpenLibrary** → **Wikidata**

Map an entire research landscape: who's publishing, who's funding it, which institutions dominate, where the citation clusters are, what's trending in preprints, and where the gaps are.

---

### Environmental justice audit

> "Is this community bearing a disproportionate burden?"

**Census** → **CDC** → **Socrata** → **NOAA** → **Earthquake** → **OpenStreetMap** → **OpenStates** → **WHO**

Cross-reference who lives near environmental hazards with health outcomes, income levels, and the legislative response. The data to identify environmental injustice already exists across these sources — the challenge has been connecting it.

---

## What makes this work

Each server exposes structured, queryable data through the [Model Context Protocol](https://modelcontextprotocol.io). An LLM with access to multiple servers can chain queries across them — no integration code, just questions that follow the data wherever it leads.

The numbers above aren't hypothetical. 447 SEC filings referencing Log4j, Cantwell's $75K from Microsoft employees, semaglutide preprints on opioid addiction — all from real queries across these servers in a single session.

Every server listed above is open source and built on [@cyanheads/mcp-ts-core](https://github.com/cyanheads/mcp-ts-core).
