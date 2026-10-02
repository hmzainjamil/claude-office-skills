# Contract Review Skill

Analyze contracts for risks, check completeness, and get actionable recommendations.

## Quick Start

**Copy and paste the [SKILL.md](./SKILL.md) content into Claude, then upload your contract.**

Or use the direct link:
```
Please use this skill: https://raw.githubusercontent.com/claude-office-skills/all-in-one-skills/main/contract-review/SKILL.md

Then review my contract: [upload file]
```

## What It Does

- Identifies 15+ common risk patterns
- Checks for missing contract elements
- Provides specific negotiation recommendations
- References the jurisdictions documented in the skill resources; confirm current jurisdiction coverage before relying on it
- Works with English and Chinese contracts

## Example Output

**You**: Review this NDA. Identify the key risks.

**Claude** will provide:

```markdown
## Risk Assessment

### 🔴 High Risk Items

#### 1. Unlimited Liability for Breach (Section 6.2)
- **Issue**: No cap on liability for breach of confidentiality
- **Impact**: Unlimited financial exposure in case of inadvertent disclosure
- **Recommendation**: Add a liability cap (e.g., direct damages only, capped at $1M)

### 🟡 Medium Risk Items

#### 1. Vague Return/Destruction Requirements (Section 4.1)
- **Issue**: "Reasonable efforts" standard is subjective
- **Recommendation**: Specify concrete timeframe (30 days) and certification

## Key Terms Summary

| Term | Value | Risk |
|------|-------|------|
| Confidentiality Period | 2 years + 3 years survival | 🟢 Low |
| Liability Cap | None specified | 🔴 High |
| Governing Law | Delaware | 🟢 Low |

## Recommendations

### Must Fix (before signing):
- Add liability cap for breach damages
- Narrow confidentiality definition with standard exclusions
```

## Limits

This skill produces informational issue spotting and draft recommendations, not legal advice or a compliance determination. Jurisdiction coverage and the law can change. Check current primary sources and have qualified counsel review the contract and any proposed changes.

## See Also

- [Full MCP Server version](https://github.com/claude-office-skills/contract-review-skill) - For power users who want API access
