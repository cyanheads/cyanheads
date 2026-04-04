# cyanheads/cyanheads

GitHub profile repository. The [README.md](README.md) renders as the public profile page at github.com/cyanheads.

## Repo structure

This is a content-only repo — no source code, no build steps, no dependencies.

```
README.md              # The profile page (this is the entire point of the repo)
.github/FUNDING.yml    # GitHub Sponsors / Buy Me a Coffee config
.gitignore
```

## README structure

The README follows this layout:

1. **Header** — centered intro with badges (Open to Work, Website)
2. **mcp-ts-core callout** — framework intro with `npx init` scaffold command
3. **MCP project tables** — organized into categories:
   - Core infrastructure
   - Data and research
   - Development and system utilities
   - AI and external services
4. **Other projects** — non-MCP repos
5. **Open to work** — availability and contact
6. **Support** — centered Buy Me a Coffee button, website, email

Each project row uses an inline language badge (`<img>` tag), a linked project name, and a one-line description. Some include live endpoint links to deployed Cloudflare Workers endpoints.

## Editing guidelines

- Keep descriptions to a single line per project — this is a profile page, not documentation
- Preserve the existing table format: `| badge [name](url) | description |`
- Language badges use shields.io inline images at height 15
- New MCP servers built on mcp-ts-core go in the appropriate category table
- Non-MCP projects go in "Other projects"
- The centered `<div>` blocks at top and bottom must stay balanced
- Link format for live endpoints: `[/mcp](https://<subdomain>.caseyjhand.com/mcp)`
