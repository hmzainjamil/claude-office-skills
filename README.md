# Claude Office Skills

A collection of Claude-oriented skill folders, shared reference material, and an Office MCP server project. Skills are primarily Markdown guidance; the repository also contains executable code under `mcp-servers/office-mcp` and helper scripts. Read the relevant skill and tool implementation before use.

The [skills index](SKILLS_INDEX.md) lists categories and examples. Its count describes the index and may not reflect active, complete, or verified skills.

## Repository map

| Path | Purpose |
|---|---|
| [SKILLS_INDEX.md](SKILLS_INDEX.md) | Skill catalog and category index |
| [contract-review/](contract-review/) | Contract review skill and guide |
| [invoice-generator/](invoice-generator/) | Invoice drafting skill and guide |
| [resume-tailor/](resume-tailor/) | Resume tailoring skill and guide |
| [official-skills/](official-skills/) | References and guides to separately maintained skills |
| [mcp-servers/office-mcp/](mcp-servers/office-mcp/) | Office document MCP server source, package scripts, and dependencies |
| [CONTRIBUTING.md](CONTRIBUTING.md) | Contribution format and skill template guidance |
| [LICENSE](LICENSE) | Root MIT license; check individual materials for additional terms |

Examples in this repository do not establish professional, legal, financial, tax, or employment advice. Review generated documents against source materials and qualified human judgment.

## Using a skill

Open the selected folder's `SKILL.md` and README. Many skills are plain instructions that can be copied into an assistant conversation. The MCP server is a separate software component with its own dependencies and commands. This repository does not define one root package installation command for all content.

Before using the Office MCP server, follow its own [package documentation](mcp-servers/office-mcp/README.md) and inspect its tools and dependencies. Do not supply confidential documents or credentials until you understand where processing occurs and what gets stored or transmitted.

## Document review

Generated Word, Excel, PowerPoint, and PDF files can contain calculation, formatting, citation, and compatibility errors. Check calculations independently, confirm source references, and inspect exported files in the intended application before delivery. No claim of pixel-perfect rendering or error-free output is made.

## Security and privacy

Skills may handle contracts, resumes, invoices, financial data, and other sensitive documents. See [SECURITY.md](SECURITY.md) before using them. Use synthetic examples for initial trials and keep credentials and client data out of commits and logs.

