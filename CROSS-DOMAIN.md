# Cross-Domain Queries

The power of MCP servers isn't any single data source — it's what happens when you connect them. With more than 60 servers spanning federal and state government, scientific and legal literature, genomics and chemistry, macroeconomics, geospatial data, cybersecurity, and public health, an agent can chase a question across domains in one conversation. No ETL, no warehouse, no integration code — just a question, followed wherever the data leads.

An agent *can* hit any of these APIs directly: read the docs, register a key, hand-roll the requests, paginate, reshape the JSON. Do that six times in a single investigation and the context window is gone before the question gets answered. Each MCP server collapses a source to one structured tool call, and the fleet is self-describing — a search for "campaign finance" surfaces OpenFEC, "known vulnerabilities" surfaces OSV. The agent finds the right server by concept, calls it, and gets structured data back. The chains below thread four to seven sources in a single conversation, joined on the identifiers that pass from one server to the next.

---

### Follow the money on a bill

> "Who's behind this bill — and is the government already paying them?"

**Congress** → **OpenFEC** → **USAspending** → **SEC EDGAR** → **OpenStates**

Start with a bill in Congress and its sponsor, then aggregate that sponsor's campaign contributions by employer in OpenFEC. Take the top corporate names and ask USAspending whether those same companies hold federal contracts — campaign donor on one side of the ledger, federal vendor on the other. Cross-check each company's 10-K risk factors in SEC EDGAR for what the bill would cost or save them, then sweep OpenStates to see how many states are running the same legislation in parallel.

> **Real data — AI regulation, through Sen. Cantwell (D-WA):** she sits on the Senate Commerce Committee, the panel that writes tech policy. Her 2024 campaign's top employer-affiliated donors were T-Mobile ($99.3K), Microsoft ($75.4K), and Amazon ($52.6K). Microsoft also shows up in USAspending as a federal contractor with $459.8M in obligations — donor and vendor at once. 3,471 state bills reference "artificial intelligence." The campaign-finance and procurement sides of one company never sit in the same database — until you join them on the company name.

---

### Drug safety investigation

> "What's the full story on this compound — from molecule to market signal?"

**PubChem** → **OpenFDA** → **ClinicalTrials.gov** → **PubMed** + **bioRxiv** → **SEC EDGAR** → **WHO**

Resolve a compound to its PubChem CID and pull its structure, targets, and safety flags. Cross to OpenFDA for post-market adverse-event counts — the full report set spills to a SQL canvas you can group by reaction. Pull the trial history from ClinicalTrials.gov by NCT ID, the peer-reviewed record from PubMed, and the preprint frontier from bioRxiv. Check the manufacturer's SEC filings for what they've disclosed as material, and set the whole picture against WHO's global prevalence data.

> **Real data — semaglutide (Ozempic):** 12,089 openFDA reports pairing the drug with nausea. 701 registered trials. 1,253 PubMed papers on its safety. bioRxiv preprints probing effects well outside the obesity indication — addiction, neuroprotection — research signals that never reach the official label. WHO context for the demand: ~42% adult obesity in the US against ~5% in Japan.

---

### CVE impact forensics

> "What actually happened after this vulnerability dropped?"

**OSV** → **NIST NVD** → **SEC EDGAR** → **Congress** → **arXiv**

Start at the package, not the score. Query OSV for an affected library version and you get the whole advisory cascade; chain the CVE aliases into NVD for CVSS, CWE classification, the CISA KEV deadline, and the affected-product matrix. Then leave the security domain entirely: search SEC EDGAR's full-text index for the corporate disclosure footprint, check Congress for the oversight response, and arXiv for what researchers published.

> **Real data — Log4Shell (CVE-2021-44228):** one vulnerable version of log4j-core returns 7 OSV advisories — the original RCE plus the incomplete-fix follow-ups (CVE-2021-45046, -45105, -44832). NVD scores it CVSS 10.0, and its CISA KEV entry gave federal agencies a hard remediation deadline; the affected-product list runs from Siemens industrial controllers to Cisco gear to Apple Xcode. SEC EDGAR full-text returns 582 filings naming "Log4j" — 186 10-Ks, 237 10-Qs, 18 8-Ks — companies still citing it years later. 25 arXiv papers. No vulnerability database tracks that corporate-disclosure blast radius; the chain reconstructs it.

---

### Transit equity analysis

> "Who does the bus network actually serve?"

**OneBusAway** → **Census** → **OpenStreetMap** → **FCC** → **BLS** → **WSDOT** → **OpenStates**

Map real-time service frequency from OneBusAway against neighborhood demographics from the Census, then layer the physical environment from OpenStreetMap — sidewalks, crossings, bike infrastructure — and the digital one from the FCC's broadband coverage data, since transit access and internet access tend to track the same dividing lines. Add BLS employment, WSDOT tolling and travel times for the car alternative, and OpenStates for the funding decisions behind it all.

> **Real data — Seattle's Rainier Beach:** 18 transit stops within 500m, all wheelchair-accessible; 23 cycleways within 1km along the Chief Sealth Trail; 84 live toll entries across 5 express corridors a lower-income commuter can't use. The data to weigh service against who's being served exists in five separate places — the work has always been connecting it.

---

### Climate + biodiversity + economics

> "How is a changing climate reshaping this region's ecology and economy?"

**NOAA** + **Open-Meteo** → **GBIF** → **USGS Water** → **BrAPI** → **World Bank** + **IMF** → **Census**

Pull the long-run climate record from NOAA and Open-Meteo's ERA5 reanalysis, back to 1940. Track whether species ranges are shifting in GBIF occurrence records, whether rivers are running low against USGS streamflow percentiles, and whether crop trials in BrAPI show yields responding. Then connect the ecology to the economy: World Bank and IMF for macro indicators, Census for whether people are moving. Climate, biodiversity, hydrology, agriculture, and economics — five domains that each hold one piece of the same trend.

---

### Historical event reconstruction

> "What did people know at the time — and what have we learned since?"

**Library of Congress** → **Smithsonian** → **Wikipedia** → **Wikidata** → **OpenAlex** + **Crossref** → **OpenLibrary**

Begin with primary sources: Library of Congress newspaper pages from the week it happened, Smithsonian objects and photographs from the period. Pin down the people and places with Wikipedia for narrative and Wikidata for structured identifiers, then trace the scholarship that followed — OpenAlex and Crossref for the academic record, OpenLibrary for the books. The arc runs from the front page printed that morning to the citation network built over the decades since.

---

### Pandemic signal detection

> "What weak signals are converging right now?"

**WHO** → **CDC** → **GDELT** → **bioRxiv** → **PubMed** → **ClinicalTrials.gov** → **GBIF** → **EIA** + **BLS**

No single feed means anything on its own. WHO surveillance indicators tick up. CDC's domestic datasets show a regional bump. GDELT registers a coverage spike in the same place. A cluster of bioRxiv preprints appears, PubMed follows, new trials register on ClinicalTrials.gov. GBIF occurrence data shows a vector species shifting range; EIA energy load and BLS data drift in ways that track people staying home. Convergence across independent sources — surveillance, media, literature, ecology, economic activity — is the signal none of them carries alone.

---

### "Should I move there?"

> "What does every public dataset say about this place?"

**Census** → **BLS** → **NWS** + **Open-Meteo** → **Earthquake** → **FCC** → **OpenStreetMap** → **OneBusAway** → **Socrata**

Every dimension of livability from authoritative sources, not a listing's spin. Census demographics and BLS jobs. NWS forecasts plus Open-Meteo's air-quality and historical climate data. Seismic risk from the Earthquake feed, broadband availability from the FCC, walkability and amenities from OpenStreetMap, real transit access from OneBusAway, and whatever the city itself publishes — permits, crime, 311 — through Socrata. The actual data on whether a place fits, pulled in one conversation.

---

### Research literature mapping

> "What's the state of this field — who's publishing, who's funding it, and what's not being studied?"

**OpenAlex** → **ORCID** → **Crossref** → **PubMed** + **arXiv** + **bioRxiv** → **Wikidata**

Map a research landscape quantitatively. OpenAlex for the citation graph and publication trends over time — group results by year, institution, or topic. ORCID to disambiguate the authors and build dossiers; Crossref for the funder records behind the work. Pull the domain literature from PubMed, arXiv, and bioRxiv in parallel, then resolve entities to stable identifiers in Wikidata. The output is a field map: who dominates, where the citation clusters are, what's surging in preprints, and which questions no one is funding.

---

### Environmental justice audit

> "Is this community carrying a disproportionate share of the burden?"

**Census** → **CDC** → **Open-Meteo** → **USGS Water** → **FEMA** → **OpenStreetMap** → **Socrata** → **OpenStates**

Cross-reference who lives where (Census) with health outcomes (CDC) and the hazards themselves: modeled air quality from Open-Meteo, streamflow and water data from USGS, flood and disaster exposure from FEMA. Locate the physical sources — highways, industrial sites — in OpenStreetMap, pull local environmental records through Socrata, and check OpenStates for the legislative response, or its absence. The pieces to prove an environmental-justice claim already exist in public data; the burden has always been assembling them.

---

## What makes this work

Each server exposes structured, queryable data through the [Model Context Protocol](https://modelcontextprotocol.io). An agent with several connected can chain across them with no integration code — and two things make that chaining actually hold together:

**Shared identifiers are join keys.** A DOI from ORCID is a lookup in Crossref or PubMed. A CVE alias from OSV is the query key in NVD. A federal disaster number ties FEMA's housing and public-assistance tools together; a company name bridges OpenFEC donations and USAspending contracts. The agent carries an ID out of one server and straight into the next.

**Large results stay queryable.** When a pull is too big for a context window — decades of FX rates, every adverse-event report for a drug, a full XBRL financial history — these servers spill the result to a DuckDB canvas and hand back a table you query with SQL, instead of truncating it.

The numbers in this document came from real queries across these servers: 582 SEC filings naming Log4j, Microsoft as both a Cantwell donor and a $459.8M federal contractor, 12,089 adverse-event reports for a single drug. Not hypothetical — just questions followed across domains.

Every server here is open source and built on [@cyanheads/mcp-ts-core](https://github.com/cyanheads/mcp-ts-core).
