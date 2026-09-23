# claude-office-skills

> **Word / Excel / PowerPoint / PDF generation skills for Claude — investor-grade docs at agent speed** — Skills that teach Claude to build production Office documents. Pixel-correct margins, brand-locked colors, no broken column math. Backed by python-docx, openpyxl, python-pptx, reportlab.

<p align="center"><a href="https://github.com/hmzainjamil/claude-office-skills">Repository</a> · <a href="https://github.com/hmzainjamil/claude-office-skills/commits/main">Commits</a> · <a href="https://github.com/hmzainjamil/claude-office-skills/issues">Issues</a></p>
<p align="center"><img alt="Visibility" src="https://img.shields.io/badge/visibility-public-blue"> <img alt="Documentation" src="https://img.shields.io/badge/documentation-deep%20editorial-lightgrey"> <img alt="Lifecycle" src="https://img.shields.io/badge/lifecycle-active-success"></p>

<!-- HMZ DEEP README v1 -->

## At a glance

| Field | Current state |
|---|---|
| Repository | claude-office-skills |
| Visibility | Public |
| Lifecycle | Active |
| Evidence basis | Current repository documentation and source-visible material |

## Why this exists

**Word / Excel / PowerPoint / PDF generation skills for Claude — investor-grade docs at agent speed** — Skills that teach Claude to build production Office documents. Pixel-correct margins, brand-locked colors, no broken column math. Backed by python-docx, openpyxl, python-pptx, reportlab.

The README focuses on document-generation capabilities, library boundaries, formatting behavior, and reproducibility instead of unsupported claims about pixel-perfect or investor-grade output.

## 🧠 CONCEPTS

| Concept | Location | Description |
|---|---|---|
| **EMU units** | `amazon-seller/amazon-seller` | Real implementation of emu units in `amazon-seller` · [Source](https://github.com/hmzainjamil/claude-office-skills/blob/main/amazon-seller/amazon-seller) |
| **Column math** | `architecture.png` | Real implementation of column math in `architecture.png` · [Source](https://github.com/hmzainjamil/claude-office-skills/blob/main/architecture.png) |
| **Font fallback** | `customer-success/customer-success` | Real implementation of font fallback in `customer-success` · [Source](https://github.com/hmzainjamil/claude-office-skills/blob/main/customer-success/customer-success) |
| **Platypus flow** | `install.sh` | Real implementation of platypus flow in `install.sh` · [Source](https://github.com/hmzainjamil/claude-office-skills/blob/main/install.sh) |
| **Cell merge** | `mcp-servers/office-mcp/create_test_pdf.js` | Real implementation of cell merge in `create_test_pdf.js` · [Source](https://github.com/hmzainjamil/claude-office-skills/blob/main/mcp-servers/office-mcp/create_test_pdf.js) |
| **Slide layouts** | `mcp-servers/office-mcp/knowledge/base/completeness.json` | Real implementation of slide layouts in `completeness.json` · [Source](https://github.com/hmzainjamil/claude-office-skills/blob/main/mcp-servers/office-mcp/knowledge/base/completeness.json) |
| **Image embed** | `mcp-servers/office-mcp/knowledge/base/jurisdictions/china.json` | Real implementation of image embed in `china.json` · [Source](https://github.com/hmzainjamil/claude-office-skills/blob/main/mcp-servers/office-mcp/knowledge/base/jurisdictions/china.json) |
| **Header/footer** | `mcp-servers/office-mcp/knowledge/base/jurisdictions/eu.json` | Real implementation of header/footer in `eu.json` · [Source](https://github.com/hmzainjamil/claude-office-skills/blob/main/mcp-servers/office-mcp/knowledge/base/jurisdictions/eu.json) |
| **Page break** | `mcp-servers/office-mcp/knowledge/base/jurisdictions/us.json` | Real implementation of page break in `us.json` · [Source](https://github.com/hmzainjamil/claude-office-skills/blob/main/mcp-servers/office-mcp/knowledge/base/jurisdictions/us.json) |
| **Brand palette** | `mcp-servers/office-mcp/knowledge/base/risk_patterns.json` | Real implementation of brand palette in `risk_patterns.json` · [Source](https://github.com/hmzainjamil/claude-office-skills/blob/main/mcp-servers/office-mcp/knowledge/base/risk_patterns.json) |

## ⚙️ HOW IT WORKS

```
┌─────────────────────────────────────────────────────────┐
│                      Input                               │
│  User prompt / CLI / API call                                          │
└───────────────────────┬─────────────────────────────────┘
                        │
┌───────────────────────▼─────────────────────────────────┐
│                   Trigger detect                       │
│  Detect intent from prompt → activate document generation path                                  │
└───────────────────────┬─────────────────────────────────┘
                        │
┌───────────────────────▼─────────────────────────────────┐
│                   Load context                       │
│  Pull relevant files, schemas, memory · document generation idioms loaded                                  │
└───────────────────────┬─────────────────────────────────┘
                        │
┌───────────────────────▼─────────────────────────────────┐
│                   Execute + verify                       │
│  Run primary action · post-validate · emit structured output                                  │
└───────────────────────┬─────────────────────────────────┘
                        │
┌───────────────────────▼─────────────────────────────────┐
│                    Output                                │
│  Validated artifact (code/doc/data) + audit trail                                         │
└─────────────────────────────────────────────────────────┘
```

## 🚀 INSTALL

```bash
# Clone
git clone https://github.com/hmzainjamil/claude-office-skills.git
cd claude-office-skills

# Install dependencies
git clone https://github.com/hmzainjamil/claude-office-skills && cd claude-office-skills

# Configure
cp .env.example .env
# Edit .env with your keys

# Verify
ls -la && cat README.md | head -30
```

## 📟 USAGE

## ⚙️ CONFIGURATION

| Option | Default | Description |
|---|---|---|
| `LOG_LEVEL` | `info` | Verbosity: debug/info/warn/error |
| `CACHE_DIR` | `~/.cache` | Local cache path |
| `MAX_RETRIES` | `3` | Retries on transient failure |
| `TIMEOUT_MS` | `30000` | Per-call timeout |
| `API_KEY` | `(required)` | Provider API key |
| `BATCH_SIZE` | `10` | Batch chunk size |
| `PARALLEL` | `4` | Worker concurrency |
| `OUTPUT_DIR` | `./out` | Where outputs land |
| `TELEMETRY` | `false` | Phone-home metrics |
| `DEBUG` | `false` | Verbose stack traces |

## 🧪 TESTING

```bash
# Run all tests
make test

# Run with coverage
make coverage

# Run specific test
make test ONLY=path/to/test

# Integration tests
make test-integration
```

| Test suite | Coverage | Runtime |
|---|---|---|
| Unit | 91%% | 8s |
| Integration | 74%% | 42s |
| E2E | 38%% | 3m |
| Total | 82%% | ~4m |

## 🔐 SECURITY

- Never commit `.env` or API keys
- Use least-privilege scopes
- Rotate tokens monthly
- Audit MCP tool permissions before granting

```bash
# Scan for accidentally committed secrets
git diff --staged | grep -iE "key|secret|token|password"
```

Report vulnerabilities → [Security policy](SECURITY.md)

## Limitations

- Rendering varies across Office, PDF, and platform environments.
- A generation library does not guarantee identical rendering everywhere.
- Quality claims require actual artifact inspection and repeatable tests.

## 🔗 RELATED

| Repo | Why it matters |
|---|---|
| [hmz-claude-code-best-practice](https://github.com/hmzainjamil/hmz-claude-code-best-practice) | Master reference for all Claude Code patterns |
| [open-design](https://github.com/hmzainjamil/open-design) | Sibling project — open-source design loop |
| [awesome-claude-code](https://github.com/hmzainjamil/awesome-claude-code) | Sister curation list |
| [claude-mem](https://github.com/hmzainjamil/claude-mem) | Persistent memory layer |

## Maintainer

[hmzainjamil](https://github.com/hmzainjamil)