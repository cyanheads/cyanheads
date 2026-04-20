<div align="center">

# Hi, I'm Casey 👋

[![Open to Work](https://img.shields.io/badge/Open_to_Work-green?style=for-the-badge)](mailto:casey@caseyjhand.com) [![Website](https://img.shields.io/badge/Website-caseyjhand.com-blue?style=for-the-badge)](https://caseyjhand.com)

I build open source tools that connect LLMs to things. Based in Seattle.

</div>

<table><tr><td>

### [mcp-ts-core](https://github.com/cyanheads/mcp-ts-core)

Agent-native TypeScript framework for building Model Context Protocol (MCP) servers. 

- Declarative tool definitions
- Pluggable auth
- Multi-backend storage
- OpenTelemetry
- Runs on Node.js and Cloudflare Workers

```bash
npx @cyanheads/mcp-ts-core init my-mcp-server
```

Start your coding agent in the scaffolded project and describe what you want to build. Ships with Agent Skills and framework docs built in.

Servers below are built on it.

</td></tr></table>
</div>

## MCP servers

| Server | Description | Hosted Server |
| ------ | ----------- | ------------- |
| **MCP Infrastructure** | | |
| [model-context-protocol-resources](https://github.com/cyanheads/model-context-protocol-resources) | MCP guides and examples | |
| [mcp-reporter](https://github.com/cyanheads/mcp-reporter) | Generate capability reports across your MCP server ecosystem | |
| [workflows-mcp-server](https://github.com/cyanheads/workflows-mcp-server) | Declarative multi-step workflow engine with YAML definitions | |
| **External Data Sources** | | |
| [arxiv-mcp-server](https://github.com/cyanheads/arxiv-mcp-server) | arXiv paper search and full-text reading | [/mcp](https://arxiv.caseyjhand.com/mcp) |
| [cdc-health-mcp-server](https://github.com/cyanheads/cdc-health-mcp-server) | 1,487+ CDC public health datasets — disease surveillance, mortality, vaccinations, and more | [/mcp](https://cdc.caseyjhand.com/mcp) |
| [clinicaltrialsgov-mcp-server](https://github.com/cyanheads/clinicaltrialsgov-mcp-server) | ClinicalTrials.gov trial search, study details and results, patient matching | [/mcp](https://clinicaltrials.caseyjhand.com/mcp) |
| [congressgov-mcp-server](https://github.com/cyanheads/congressgov-mcp-server) | U.S. congressional bills, votes, members, and committees | [/mcp](https://congressgov.caseyjhand.com/mcp) |
| [hn-mcp-server](https://github.com/cyanheads/hn-mcp-server) | Hacker News feeds, discussions, user profiles, and search | [/mcp](https://hn.caseyjhand.com/mcp) |
| [openfda-mcp-server](https://github.com/cyanheads/openfda-mcp-server) | FDA drugs, food, devices, and recalls via openFDA | [/mcp](https://openfda.caseyjhand.com/mcp) |
| [openalex-mcp-server](https://github.com/cyanheads/openalex-mcp-server) | 270M+ academic works, authors, and institutions via OpenAlex | [/mcp](https://openalex.caseyjhand.com/mcp) |
| [openfec-mcp-server](https://github.com/cyanheads/openfec-mcp-server) | FEC campaign finance data — candidates, committees, contributions, and filings | [/mcp](https://openfec.caseyjhand.com/mcp) |
| [protein-mcp-server](https://github.com/cyanheads/protein-mcp-server) | Protein structures (PDB, UniProt) | |
| [pubchem-mcp-server](https://github.com/cyanheads/pubchem-mcp-server) | Compound search, properties, safety data, and bioactivity via PubChem | [/mcp](https://pubchem.caseyjhand.com/mcp) |
| [pubmed-mcp-server](https://github.com/cyanheads/pubmed-mcp-server) | PubMed article search, full text, citations, and MeSH terms | [/mcp](https://pubmed.caseyjhand.com/mcp) |
| [nhtsa-vehicle-safety-mcp-server](https://github.com/cyanheads/nhtsa-vehicle-safety-mcp-server) | NHTSA vehicle safety — recalls, complaints, crash ratings, VIN decoding | [/mcp](https://nhtsa.caseyjhand.com/mcp) |
| [nws-weather-mcp-server](https://github.com/cyanheads/nws-weather-mcp-server) | Real-time US weather forecasts, alerts, and observations via National Weather Service | [/mcp](https://nws.caseyjhand.com/mcp) |
| [secedgar-mcp-server](https://github.com/cyanheads/secedgar-mcp-server) | SEC EDGAR filings, XBRL financials, and company data | [/mcp](https://secedgar.caseyjhand.com/mcp) |
| **Local & Workspace** | | |
| [atlas-mcp-server](https://github.com/cyanheads/atlas-mcp-server) | Neo4j task and knowledge graphs | |
| [calculator-mcp-server](https://github.com/cyanheads/calculator-mcp-server) | Math evaluation, simplification, derivatives | [/mcp](https://calculator.caseyjhand.com/mcp) |
| [filesystem-mcp-server](https://github.com/cyanheads/filesystem-mcp-server) | File and directory operations | |
| [git-mcp-server](https://github.com/cyanheads/git-mcp-server) | Git repository management — commits, branches, diffs, history, worktrees | |
| [obsidian-mcp-server](https://github.com/cyanheads/obsidian-mcp-server) | Obsidian vault notes, tags, frontmatter, and search via Local REST API | |
| [survey-mcp-server](https://github.com/cyanheads/survey-mcp-server) | Dynamic conversational surveys with skip logic and structured collection | |
| [toolkit-mcp-server](https://github.com/cyanheads/toolkit-mcp-server) | Network diagnostics, system monitoring, crypto utilities, QR codes | |
| **SaaS & Productivity** | | |
| [mailchimp-mcp-server](https://github.com/cyanheads/mailchimp-mcp-server) | Mailchimp email campaigns, audiences, subscribers, and post-send analytics | |
| **AI Services** | | |
| [mentor-mcp-server](https://github.com/cyanheads/mentor-mcp-server) | Code review, design critique, and writing feedback via Deepseek R1 | |
| [perplexity-mcp-server](https://github.com/cyanheads/perplexity-mcp-server) | Search-augmented queries and deep research via Perplexity API | |
| **Hardware & Notifications** | | |
| [ntfy-mcp-server](https://github.com/cyanheads/ntfy-mcp-server) | Push notifications via ntfy | |
| [pixoo-mcp-server](https://github.com/cyanheads/pixoo-mcp-server) | Pixel art, animations, and text on Divoom Pixoo LED matrices | |

## Other projects

| Project | Description |
| ------- | ----------- |
| <img src="https://img.shields.io/badge/-F7DF1E?logo=javascript&logoColor=black" alt="JavaScript" height="15"> [claude-sidebar-modifier](https://github.com/cyanheads/claude-sidebar-modifier) | Firefox extension to resize/hide the Claude.ai sidebar |
| <img src="https://img.shields.io/badge/-007ACC?logo=typescript&logoColor=white" alt="TypeScript" height="15"> [pixoo-toolkit](https://github.com/cyanheads/pixoo-toolkit) | Divoom Pixoo display SDK (16/32/64) |
| <img src="https://img.shields.io/badge/-3776AB?logo=python&logoColor=white" alt="Python" height="15"> [repo-map](https://github.com/cyanheads/repo-map) | AI-generated codebase summaries |
| <img src="https://img.shields.io/badge/-007ACC?logo=typescript&logoColor=white" alt="TypeScript" height="15"> [scripts-ts](https://github.com/cyanheads/scripts-ts) | Cross-platform dev utility scripts |
| <img src="https://img.shields.io/badge/-000080?logo=lua&logoColor=white" alt="Lua" height="15"> [TwilightAscensionRares](https://github.com/cyanheads/TwilightAscensionRares) | WoW addon for Twilight Highlands rare spawn tracking |

## Open to work

I build AI/LLM tooling and infrastructure. Looking for full-time or contract roles where I can keep doing that.

Available for:
- Full-time positions
- Contract and consulting
- Custom MCP server development ([view framework](https://github.com/cyanheads/mcp-ts-core))

<div align="center">

## Support

If any of this has been useful to you, I'd appreciate the support.

[![Buy Me A Coffee](https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png)](https://buymeacoffee.com/cyanheads)

Website: [caseyjhand.com](https://caseyjhand.com) | Email: [casey@caseyjhand.com](mailto:casey@caseyjhand.com)

---

_When we share knowledge, everyone benefits._

</div>