<div align="center">

# Hi, I'm Casey

[![Open to Work](https://img.shields.io/badge/Open_to_Work-green?style=for-the-badge)](mailto:casey@caseyjhand.com) [![Website](https://img.shields.io/badge/Website-caseyjhand.com-blue?style=for-the-badge)](https://caseyjhand.com)

![TypeScript](https://img.shields.io/badge/TypeScript-007ACC?style=flat-square&logo=typescript&logoColor=white) ![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white) ![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white) ![Bun](https://img.shields.io/badge/Bun-000?style=flat-square&logo=bun&logoColor=white) ![React](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black) ![Cloudflare Workers](https://img.shields.io/badge/Cloudflare_Workers-F38020?style=flat-square&logo=cloudflareworkers&logoColor=white) ![MCP](https://img.shields.io/badge/MCP-black?style=flat-square)

Software engineer in Seattle. I build open source tools, mostly around the Model Context Protocol (MCP) — giving LLMs structured ways to use external services, data sources, and system APIs.

</div>

## What I'm building with MCP

All of these are built on my [mcp-ts-template](https://github.com/cyanheads/mcp-ts-template), a TypeScript starter for MCP servers with DI, pluggable auth, abstracted storage, and Cloudflare Workers support.

### Core infrastructure

| Project | Description |
| ------- | ----------- |
| <img src="https://img.shields.io/badge/-007ACC?logo=typescript&logoColor=white" alt="TypeScript" height="15"> [mcp-ts-template](https://github.com/cyanheads/mcp-ts-template) | Template for building MCP servers in TypeScript. Declarative tools, elicitation, auth, storage, and OpenTelemetry. |
| <img src="https://img.shields.io/badge/-007ACC?logo=typescript&logoColor=white" alt="TypeScript" height="15"> [model-context-protocol-resources](https://github.com/cyanheads/model-context-protocol-resources) | Guides, utilities, and example server implementations for MCP. |
| <img src="https://img.shields.io/badge/-007ACC?logo=typescript&logoColor=white" alt="TypeScript" height="15"> [workflows-mcp-server](https://github.com/cyanheads/workflows-mcp-server) | Runs multi-step workflows defined in YAML files. Gives agents a structured way to execute complex task sequences. |
| <img src="https://img.shields.io/badge/-007ACC?logo=typescript&logoColor=white" alt="TypeScript" height="15"> [mcp-reporter](https://github.com/cyanheads/mcp-reporter) | Generates human-readable capability reports for MCP servers — what tools are available, what they do, how to call them. |

### Data and research

| Project | Description |
| ------- | ----------- |
| <img src="https://img.shields.io/badge/-007ACC?logo=typescript&logoColor=white" alt="TypeScript" height="15"> [atlas-mcp-server](https://github.com/cyanheads/atlas-mcp-server) | Neo4j-backed task management for LLM agents. Three-tier model: projects, tasks, and knowledge nodes. Includes deep research capabilities. |
| <img src="https://img.shields.io/badge/-007ACC?logo=typescript&logoColor=white" alt="TypeScript" height="15"> [protein-mcp-server](https://github.com/cyanheads/protein-mcp-server) | Access to 3D protein structure data from RCSB PDB, PDBe, and UniProt. Search, retrieve, and analyze structural records. |
| <img src="https://img.shields.io/badge/-007ACC?logo=typescript&logoColor=white" alt="TypeScript" height="15"> [clinicaltrialsgov-mcp-server](https://github.com/cyanheads/clinicaltrialsgov-mcp-server) | Search and analyze clinical trials from ClinicalTrials.gov. Includes patient eligibility matching and trend analysis. [Try it live.](https://clinicaltrials.caseyjhand.com/mcp) |
| <img src="https://img.shields.io/badge/-007ACC?logo=typescript&logoColor=white" alt="TypeScript" height="15"> [pubmed-mcp-server](https://github.com/cyanheads/pubmed-mcp-server) | Search and retrieve biomedical literature from PubMed. Includes a research agent scaffold for multi-step literature workflows. |
| <img src="https://img.shields.io/badge/-007ACC?logo=typescript&logoColor=white" alt="TypeScript" height="15"> [pubchem-mcp-server](https://github.com/cyanheads/pubchem-mcp-server) | LLM tools for the PubChem PUG REST API — chemical compound lookups, bioassay data, and substance search. |
| <img src="https://img.shields.io/badge/-007ACC?logo=typescript&logoColor=white" alt="TypeScript" height="15"> [survey-mcp-server](https://github.com/cyanheads/survey-mcp-server) | Lets LLMs conduct conversational surveys with conditional logic and structured data collection. |

### Development and system utilities

| Project | Description |
| ------- | ----------- |
| <img src="https://img.shields.io/badge/-007ACC?logo=typescript&logoColor=white" alt="TypeScript" height="15"> [git-mcp-server](https://github.com/cyanheads/git-mcp-server) | Git operations for LLM agents — commits, branches, diffs, logs, and more. |
| <img src="https://img.shields.io/badge/-007ACC?logo=typescript&logoColor=white" alt="TypeScript" height="15"> [filesystem-mcp-server](https://github.com/cyanheads/filesystem-mcp-server) | File and directory management: read, write, search/replace, and directory traversal. |
| <img src="https://img.shields.io/badge/-007ACC?logo=typescript&logoColor=white" alt="TypeScript" height="15"> [obsidian-mcp-server](https://github.com/cyanheads/obsidian-mcp-server) | Interact with an Obsidian vault via the Local REST API plugin. Read, write, and search notes. |
| <img src="https://img.shields.io/badge/-007ACC?logo=typescript&logoColor=white" alt="TypeScript" height="15"> [toolkit-mcp-server](https://github.com/cyanheads/toolkit-mcp-server) | System utilities for LLM agents: network diagnostics, system info, and monitoring. |
| <img src="https://img.shields.io/badge/-007ACC?logo=typescript&logoColor=white" alt="TypeScript" height="15"> [ntfy-mcp-server](https://github.com/cyanheads/ntfy-mcp-server) | Send push notifications via ntfy from an LLM agent. |
| <img src="https://img.shields.io/badge/-007ACC?logo=typescript&logoColor=white" alt="TypeScript" height="15"> [pixoo-mcp-server](https://github.com/cyanheads/pixoo-mcp-server) | Push pixel art, animations, and text to Divoom Pixoo LED matrices. Supports layered scenes, multi-frame animation, and device control. |

### AI and external services

| Project | Description |
| ------- | ----------- |
| <img src="https://img.shields.io/badge/-007ACC?logo=typescript&logoColor=white" alt="TypeScript" height="15"> [perplexity-mcp-server](https://github.com/cyanheads/perplexity-mcp-server) | Search-augmented AI via the Perplexity API, with citation support. |
| <img src="https://img.shields.io/badge/-007ACC?logo=typescript&logoColor=white" alt="TypeScript" height="15"> [mentor-mcp-server](https://github.com/cyanheads/mentor-mcp-server) | Second-opinion code reviews and design critiques via the Deepseek API. |
| <img src="https://img.shields.io/badge/-007ACC?logo=typescript&logoColor=white" alt="TypeScript" height="15"> [github-mcp-server](https://github.com/cyanheads/github-mcp-server) | [DEPRECATED] — Use the [official GitHub MCP Server](https://github.com/github/github-mcp-server?tab=readme-ov-file#remote-github-mcp-server). |

## Other projects

| Project | Description |
| ------- | ----------- |
| <img src="https://img.shields.io/badge/-007ACC?logo=typescript&logoColor=white" alt="TypeScript" height="15"> [pixoo-toolkit](https://github.com/cyanheads/pixoo-toolkit) | TypeScript toolkit for Divoom Pixoo displays (16, 32, 64). Pixel rendering, animations, and device control over local HTTP. |
| <img src="https://img.shields.io/badge/-3776AB?logo=python&logoColor=white" alt="Python" height="15"> [repo-map](https://github.com/cyanheads/repo-map) | Generates visual summaries of codebases using AI. Caches results, supports multiple languages, respects gitignore. |
| <img src="https://img.shields.io/badge/-F7DF1E?logo=javascript&logoColor=black" alt="JavaScript" height="15"> [claude-sidebar-modifier](https://github.com/cyanheads/claude-sidebar-modifier) | Firefox extension that disables or resizes the Claude.ai sidebar. |
| <img src="https://img.shields.io/badge/-007ACC?logo=typescript&logoColor=white" alt="TypeScript" height="15"> [scripts-ts](https://github.com/cyanheads/scripts-ts) | Cross-platform TypeScript utility scripts for common dev tasks. |
| <img src="https://img.shields.io/badge/-000080?logo=lua&logoColor=white" alt="Lua" height="15"> [TwilightAscensionRares](https://github.com/cyanheads/TwilightAscensionRares) | WoW addon for tracking Twilight Highlands rare spawns (Two Minutes to Midnight achievement). Live schedule, countdown timers, waypoints, and raid/chat sharing. |

## Open to work

I'm looking for full-time and contract roles in AI/LLM tooling and infrastructure. I've spent the last year building autonomous agents and MCP servers, and I want to keep going.

Available for:
- Full-time positions
- Contract and consulting
- Custom MCP server development ([view template](https://github.com/cyanheads/mcp-ts-template))

<div align="center">

## Support

If any of this has been useful to you, I'd appreciate the support.

[![Buy Me A Coffee](https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png)](https://buymeacoffee.com/cyanheads)

Website: [caseyjhand.com](https://caseyjhand.com) | Email: [casey@caseyjhand.com](mailto:casey@caseyjhand.com)

</div>