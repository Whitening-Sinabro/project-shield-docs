# Project Shield

> Security scanner for MCP servers and AI-generated code.

One command to security-grade your MCP server.

## What it detects

| Layer | What | How |
|-------|------|-----|
| 🔑 **Secrets** | API keys, tokens, credentials | Regex + entropy + context analysis |
| 👤 **PII** | Email, phone, SSN | Pattern matching + checksum validation |
| 💉 **Prompt Injection** | Attacks in MCP tool descriptions | Heuristic + pattern detection |
| 🛡️ **MCP Misconfig** | Missing auth, open permissions, no logging | Config rule engine |

## Security Grades

| Grade | Meaning |
|-------|---------|
| A | Excellent — ship with confidence |
| B | Good — minor improvements suggested |
| C | Clean — some issues to address |
| D | Warning — fix before deploy |
| E | Warning — significant issues found |
| F | **Locked** — deployment blocked until fixed |

## Quick Start

```bash
npx project-shield scan .
```

## MCP Server Config

```json
{
  "mcpServers": {
    "project-shield": {
      "command": "npx",
      "args": ["-y", "project-shield", "scan", "."]
    }
  }
}
```

## Features

- **275+ detection rules** across 4 security layers
- **A-F grading system** with automatic deploy lock on F
- **Evidence Packs** — SHA-256 hashed, tamper-proof scan results
- **Fix-it guides** — actionable remediation for every finding
- **Badge system** — verifiable security badges for your projects

## Pricing

| Plan | Price | Scans | Features |
|------|-------|-------|----------|
| Free | $0 | 5/month | Basic reporting |
| Pro | $29/month | 50/month | PDF reports, Evidence Packs |
| Team | $99/month | Unlimited (5 users) | CI/CD integration |
| Enterprise | $299+/month | Custom | SSO, audit trails |

## Links

- **Website**: [shield.codemeant.dev](https://shield.codemeant.dev)
- **npm**: [project-shield](https://www.npmjs.com/package/project-shield)

## License

Proprietary — see [shield.codemeant.dev](https://shield.codemeant.dev) for terms.
