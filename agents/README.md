# Claude Office agent instructions

This directory contains five Markdown role definitions. Each `AGENT.md` file has role metadata, prompt instructions, and references to skills, tools, or knowledge paths.

| Role | Definition |
|---|---|
| Legal Specialist | [AGENT.md](legal-specialist/AGENT.md) |
| Data Analyst | [AGENT.md](data-analyst/AGENT.md) |
| Admin Assistant | [AGENT.md](admin-assistant/AGENT.md) |
| Research Analyst | [AGENT.md](research-analyst/AGENT.md) |
| Content Creator | [AGENT.md](content-creator/AGENT.md) |

These files are instructions, not a packaged agent runtime. This directory contains no platform adapters or deployment configuration. Host support, referenced skills, MCP tools, and knowledge paths must be verified in the target environment before use.

Read the complete role definition and inspect its tool and data references before providing documents, credentials, or account access. See the [repository README](../README.md) for repository scope, document-handling limits, and security guidance.
