<div align="center">

# Hi, I'm Casey 👋

[![Open to Work](https://img.shields.io/badge/Open_to_Work-green?style=for-the-badge)](mailto:casey@caseyjhand.com) [![Website](https://img.shields.io/badge/Website-caseyjhand.com-blue?style=for-the-badge)](https://caseyjhand.com) 

[![@cyanheads/mcp-ts-core](https://img.shields.io/badge/@cyanheads%2Fmcp--ts--core-67E8F9?style=for-the-badge)](https://github.com/cyanheads/mcp-ts-core) [![Bun](https://img.shields.io/badge/Bun-FBF0DF?style=for-the-badge&logo=bun&logoColor=black)](https://bun.sh) [![Model Context Protocol](https://img.shields.io/badge/Model_Context_Protocol-1A1A1A?style=for-the-badge)](https://modelcontextprotocol.io)

I'm exploring ways to connect LLMs to the real world. Based in Seattle.

</div>

### [@cyanheads/mcp-ts-core](https://github.com/cyanheads/mcp-ts-core)

Agent-native TypeScript framework for building Model Context Protocol (MCP) servers.

- Declarative tool definitions
- Pluggable auth
- OpenTelemetry
- Runs on Node.js and Cloudflare Workers

```bash
bunx @cyanheads/mcp-ts-core init my-mcp-server
```

Start your coding agent in the scaffolded project and describe what you want to build. 

Ships with Agent Skills and framework docs built in.

## MCP servers

> **[Cross-domain queries](CROSS-DOMAIN.md)** — what happens when you connect 40+ data sources in one conversation.

### MCP infrastructure

<table>
<tr>
<td><a href="https://github.com/cyanheads/model-context-protocol-resources">model-context-protocol-resources</a></td>
<td><a href="https://github.com/cyanheads/mcp-reporter">mcp-reporter</a></td>
<td><a href="https://github.com/cyanheads/workflows-mcp-server">workflows-mcp-server</a></td>
</tr>
</table>

### External data

<table>
<tr>
<td><a href="https://github.com/cyanheads/arxiv-mcp-server">arxiv-mcp-server</a> • <a href="https://arxiv.caseyjhand.com/">/mcp</a></td>
<td><a href="https://github.com/cyanheads/brapi-mcp-server">brapi-mcp-server</a> • <a href="https://brapi.caseyjhand.com/">/mcp</a></td>
<td><a href="https://github.com/cyanheads/cdc-health-mcp-server">cdc-health-mcp-server</a> • <a href="https://cdc.caseyjhand.com/">/mcp</a></td>
</tr>
<tr>
<td><a href="https://github.com/cyanheads/clinicaltrialsgov-mcp-server">clinicaltrialsgov-mcp-server</a> • <a href="https://clinicaltrials.caseyjhand.com/">/mcp</a></td>
<td><a href="https://github.com/cyanheads/congressgov-mcp-server">congressgov-mcp-server</a> • <a href="https://congressgov.caseyjhand.com/">/mcp</a></td>
<td><a href="https://github.com/cyanheads/hn-mcp-server">hn-mcp-server</a> • <a href="https://hn.caseyjhand.com/">/mcp</a></td>
</tr>
<tr>
<td><a href="https://github.com/cyanheads/openfda-mcp-server">openfda-mcp-server</a> • <a href="https://openfda.caseyjhand.com/">/mcp</a></td>
<td><a href="https://github.com/cyanheads/openalex-mcp-server">openalex-mcp-server</a> • <a href="https://openalex.caseyjhand.com/">/mcp</a></td>
<td><a href="https://github.com/cyanheads/openfec-mcp-server">openfec-mcp-server</a> • <a href="https://openfec.caseyjhand.com/">/mcp</a></td>
</tr>
<tr>
<td><a href="https://github.com/cyanheads/protein-mcp-server">protein-mcp-server</a></td>
<td><a href="https://github.com/cyanheads/pubchem-mcp-server">pubchem-mcp-server</a> • <a href="https://pubchem.caseyjhand.com/">/mcp</a></td>
<td><a href="https://github.com/cyanheads/pubmed-mcp-server">pubmed-mcp-server</a> • <a href="https://pubmed.caseyjhand.com/">/mcp</a></td>
</tr>
<tr>
<td><a href="https://github.com/cyanheads/nhtsa-vehicle-safety-mcp-server">nhtsa-vehicle-safety-mcp-server</a> • <a href="https://nhtsa.caseyjhand.com/">/mcp</a></td>
<td><a href="https://github.com/cyanheads/nws-weather-mcp-server">nws-weather-mcp-server</a> • <a href="https://nws.caseyjhand.com/">/mcp</a></td>
<td><a href="https://github.com/cyanheads/secedgar-mcp-server">secedgar-mcp-server</a> • <a href="https://secedgar.caseyjhand.com/">/mcp</a></td>
</tr>
<tr>
<td><a href="https://github.com/cyanheads/biorxiv-mcp-server">biorxiv-mcp-server</a> • <a href="https://biorxiv.caseyjhand.com/">/mcp</a></td>
<td><a href="https://github.com/cyanheads/bls-labor-mcp-server">bls-labor-mcp-server</a> • <a href="https://bls-labor.caseyjhand.com/">/mcp</a></td>
<td><a href="https://github.com/cyanheads/crossref-mcp-server">crossref-mcp-server</a> • <a href="https://crossref.caseyjhand.com/">/mcp</a></td>
</tr>
<tr>
<td><a href="https://github.com/cyanheads/eia-energy-mcp-server">eia-energy-mcp-server</a> • <a href="https://eia-energy.caseyjhand.com/">/mcp</a></td>
<td><a href="https://github.com/cyanheads/federal-reserve-mcp-server">federal-reserve-mcp-server</a></td>
<td><a href="https://github.com/cyanheads/onebusaway-mcp-server">onebusaway-mcp-server</a> • <a href="https://onebusaway.caseyjhand.com/">/mcp</a></td>
</tr>
<tr>
<td><a href="https://github.com/cyanheads/openstates-mcp-server">openstates-mcp-server</a> • <a href="https://openstates.caseyjhand.com/">/mcp</a></td>
<td><a href="https://github.com/cyanheads/socrata-mcp-server">socrata-mcp-server</a> • <a href="https://socrata.caseyjhand.com/">/mcp</a></td>
<td><a href="https://github.com/cyanheads/wsdot-mcp-server">wsdot-mcp-server</a> • <a href="https://wsdot.caseyjhand.com/">/mcp</a></td>
</tr>
<tr>
<td><a href="https://github.com/cyanheads/earthquake-mcp-server">earthquake-mcp-server</a> • <a href="https://earthquake.caseyjhand.com/">/mcp</a></td>
<td><a href="https://github.com/cyanheads/eurostat-mcp-server">eurostat-mcp-server</a> • <a href="https://eurostat.caseyjhand.com/">/mcp</a></td>
<td><a href="https://github.com/cyanheads/gbif-biodiversity-mcp-server">gbif-biodiversity-mcp-server</a> • <a href="https://gbif-biodiversity.caseyjhand.com/">/mcp</a></td>
</tr>
<tr>
<td><a href="https://github.com/cyanheads/noaa-cdo-mcp-server">noaa-cdo-mcp-server</a> • <a href="https://noaa-cdo.caseyjhand.com/">/mcp</a></td>
<td><a href="https://github.com/cyanheads/openstreetmap-mcp-server">openstreetmap-mcp-server</a> • <a href="https://openstreetmap.caseyjhand.com/">/mcp</a></td>
<td><a href="https://github.com/cyanheads/openlibrary-mcp-server">openlibrary-mcp-server</a> • <a href="https://openlibrary.caseyjhand.com/">/mcp</a></td>
</tr>
<tr>
<td><a href="https://github.com/cyanheads/reliefweb-mcp-server">reliefweb-mcp-server</a></td>
<td><a href="https://github.com/cyanheads/who-gho-mcp-server">who-gho-mcp-server</a> • <a href="https://who-gho.caseyjhand.com/">/mcp</a></td>
<td><a href="https://github.com/cyanheads/wikidata-mcp-server">wikidata-mcp-server</a> • <a href="https://wikidata.caseyjhand.com/">/mcp</a></td>
</tr>
<tr>
<td><a href="https://github.com/cyanheads/worldbank-mcp-server">worldbank-mcp-server</a> • <a href="https://worldbank.caseyjhand.com/">/mcp</a></td>
<td><a href="https://github.com/cyanheads/census-mcp-server">census-mcp-server</a> • <a href="https://census.caseyjhand.com/">/mcp</a></td>
<td><a href="https://github.com/cyanheads/libofcongress-mcp-server">libofcongress-mcp-server</a> • <a href="https://libofcongress.caseyjhand.com/">/mcp</a></td>
</tr>
<tr>
<td><a href="https://github.com/cyanheads/nist-nvd-mcp-server">nist-nvd-mcp-server</a> • <a href="https://nist-nvd.caseyjhand.com/">/mcp</a></td>
<td><a href="https://github.com/cyanheads/reference-data-mcp-server">reference-data-mcp-server</a> • <a href="https://reference-data.caseyjhand.com/">/mcp</a></td>
<td><a href="https://github.com/cyanheads/usda-mcp-server">usda-mcp-server</a></td>
</tr>
<tr>
<td><a href="https://github.com/cyanheads/wikipedia-mcp-server">wikipedia-mcp-server</a> • <a href="https://wikipedia.caseyjhand.com/">/mcp</a></td>
</tr>
</table>

### Local & workspace

<table>
<tr>
<td><a href="https://github.com/cyanheads/atlas-mcp-server">atlas-mcp-server</a></td>
<td><a href="https://github.com/cyanheads/calculator-mcp-server">calculator-mcp-server</a> • <a href="https://calculator.caseyjhand.com/">/mcp</a></td>
<td><a href="https://github.com/cyanheads/filesystem-mcp-server">filesystem-mcp-server</a></td>
</tr>
<tr>
<td><a href="https://github.com/cyanheads/git-mcp-server">git-mcp-server</a></td>
<td><a href="https://github.com/cyanheads/obsidian-mcp-server">obsidian-mcp-server</a></td>
<td><a href="https://github.com/cyanheads/survey-mcp-server">survey-mcp-server</a></td>
</tr>
<tr>
<td><a href="https://github.com/cyanheads/toolkit-mcp-server">toolkit-mcp-server</a></td>
</tr>
</table>

### SaaS & productivity

<table>
<tr>
<td><a href="https://github.com/cyanheads/mailchimp-mcp-server">mailchimp-mcp-server</a></td>
</tr>
</table>

### AI services

<table>
<tr>
<td><a href="https://github.com/cyanheads/mentor-mcp-server">mentor-mcp-server</a></td>
<td><a href="https://github.com/cyanheads/perplexity-mcp-server">perplexity-mcp-server</a></td>
</tr>
</table>

### Hardware & notifications

<table>
<tr>
<td><a href="https://github.com/cyanheads/clipboard-mcp-server">clipboard-mcp-server</a></td>
<td><a href="https://github.com/cyanheads/macos-mcp-server">macos-mcp-server</a></td>
<td><a href="https://github.com/cyanheads/ntfy-mcp-server">ntfy-mcp-server</a></td>
</tr>
<tr>
<td><a href="https://github.com/cyanheads/pixoo-mcp-server">pixoo-mcp-server</a></td>
</tr>
</table>

## Other projects

<table>
<tr>
<td><img src="https://img.shields.io/badge/-F7DF1E?logo=javascript&logoColor=black" alt="JavaScript" height="15"> <a href="https://github.com/cyanheads/claude-sidebar-modifier">claude-sidebar-modifier</a></td>
<td><img src="https://img.shields.io/badge/-007ACC?logo=typescript&logoColor=white" alt="TypeScript" height="15"> <a href="https://github.com/cyanheads/pixoo-toolkit">pixoo-toolkit</a></td>
<td><img src="https://img.shields.io/badge/-3776AB?logo=python&logoColor=white" alt="Python" height="15"> <a href="https://github.com/cyanheads/repo-map">repo-map</a></td>
</tr>
<tr>
<td><img src="https://img.shields.io/badge/-007ACC?logo=typescript&logoColor=white" alt="TypeScript" height="15"> <a href="https://github.com/cyanheads/scripts-ts">scripts-ts</a></td>
<td><img src="https://img.shields.io/badge/-000080?logo=lua&logoColor=white" alt="Lua" height="15"> <a href="https://github.com/cyanheads/TwilightAscensionRares">TwilightAscensionRares</a></td>
</tr>
</table>

## Open to work

I build AI/LLM tooling and infrastructure. Looking for full-time or contract roles where I can keep doing that.

Available for:
- Full-time positions
- Contract and consulting
- Custom MCP server development

<div align="center">

## Support

If any of my projects have been useful to you, I'd appreciate any support you're able to provide.

<a href="https://github.com/sponsors/cyanheads"><img src="https://img.shields.io/badge/Sponsor_on_GitHub-EA4AAA?style=for-the-badge&logo=github-sponsors&logoColor=white" alt="GitHub Sponsors" height="40"></a> <a href="https://buymeacoffee.com/cyanheads"><img src="https://img.shields.io/badge/Buy_Me_A_Coffee-FFDD00?style=for-the-badge&logo=buymeacoffee&logoColor=black" alt="Buy Me A Coffee" height="40"></a>

Website: [caseyjhand.com](https://caseyjhand.com) | Email: [casey@caseyjhand.com](mailto:casey@caseyjhand.com)

---

_When we share knowledge, everyone benefits._

</div>
