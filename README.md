# Project Shield

> Security scanner for MCP servers and AI-generated code.

One command to security-grade your MCP server.

## Installation

```bash
npm install -g project-shield
```

Or use directly with npx:

```bash
npx project-shield scan .
```

## MCP Server Configuration

Add to your MCP client config:

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

## Tools

### scan
Security scan a directory or MCP server project. Returns A-F grade with detailed findings.

**Parameters:**
- `path` (string, required) - Directory to scan
- `format` (string, optional) - Output format: `text`, `json`, `badge`

### grade
Get the security grade for a project without full report.

### evidence
Generate a tamper-proof Evidence Pack with SHA-256 hashed scan results.

## What it detects

| Layer | What | How |
|-------|------|-----|
| **Secrets** | API keys, tokens, credentials | Regex + entropy + context analysis |
| **PII** | Email, phone, SSN | Pattern matching + checksum validation |
| **Prompt Injection** | Attacks in MCP tool descriptions | Heuristic + pattern detection |
| **MCP Misconfig** | Missing auth, open permissions, no logging | Config rule engine |

## Security Grades

| Grade | Meaning |
|-------|---------|
| A | Excellent - ship with confidence |
| B | Good - minor improvements suggested |
| C | Clean - some issues to address |
| D | Warning - fix before deploy |
| E | Warning - significant issues found |
| F | **Locked** - deployment blocked until fixed |

## Features

- **275+ detection rules** across 4 security layers
- **A-F grading system** with automatic deploy lock on F
- **Evidence Packs** - SHA-256 hashed, tamper-proof scan results
- **Fix-it guides** - actionable remediation for every finding
- **Badge system** - verifiable security badges for your projects
- **MCP-native** - scans MCP protocol-level security, not just code

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
- **Product Hunt**: [Project Shield](https://www.producthunt.com/products/project-shield)

## License

MIT
