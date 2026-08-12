# Project Shield

[한국어](README.ko.md)

Security scanner for AI coders and MCP users. It checks projects and AI-agent configuration for exposed secrets, PII, insecure MCP settings, prompt injection, and risky Claude Code hooks.

[![npm version](https://img.shields.io/npm/v/project-shield)](https://www.npmjs.com/package/project-shield)

## Run the free scan

```bash
npx project-shield scan ./my-project
```

Project Shield v2.0.0 runs locally and includes security grading, fix guidance, and AI-agent environment auditing.

## Free and Pro

| Feature | Free | Pro |
|---|---:|---:|
| Project scans | 5/month | 50/month |
| Environment audits | 3/month | 20/month |
| Fix-it guidance | Top 3 summaries | All guides with code and references |
| Badge | Watermarked | Clean badge with UUID and verification URL |
| Evidence Pack | Not included | JSON + PDF with integrity seal |
| PII findings | Count only | File and line details |

Project Shield Pro is **$29/month** and is delivered through an automated Polar license-key benefit.

The Polar checkout displays **Clouvel**, the publisher account for Project Shield. Taxes, when applicable, are calculated by Polar from the buyer's billing address and shown before payment.

- [See Project Shield](https://shield.codemeant.dev)
- [Get Project Shield Pro for $29/month](https://buy.polar.sh/polar_cl_eiXDc9bwtIpz99P8tjt3K1NZgS8oJN9WCwYIO1pgBDt)
- [View the npm package](https://www.npmjs.com/package/project-shield)

## Commands

```bash
# Scan a project
npx project-shield scan ./my-project

# Audit the local AI coding environment
npx project-shield audit

# Activate a Polar-issued Pro license
project-shield activate PSH-XXXX-XXXX-XXXX-XXXX

# Check license status
project-shield status
```

## What Pro unlocks

- Full fix-it guides with code examples and references
- JSON and PDF Evidence Packs
- Clean badges with UUID and verification URL
- Full Claude Code environment checks and hooks analysis
- Higher monthly scan and audit limits

## Security notes

- Run scans only on projects you own or are authorized to inspect.
- Review findings before changing code or configuration.
- Never paste secrets or customer data into public issues.

## License

MIT
