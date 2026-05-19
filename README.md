# audit-code-quality

Audit codebase for quality issues that break AI tools. Checks file sizes, god components, duplicated logic, naming, separation of concerns, dead code, function complexity, and hardcoded values.

## Import into Lovable

1. Go to **Settings → Skills**
2. Click **Add → Import from GitHub**
3. Paste: `https://github.com/vulk-corp/audit-code-quality`

## Or copy-paste

Open [SKILL.md](SKILL.md) and paste the content into your AI builder tool (Lovable, Bolt, v0, Replit).

## How it works

1. Import or paste the skill into your AI builder
2. It audits your project and reports findings by severity
3. For each finding: what's wrong, what could happen, how to fix it, what could break
4. Nothing gets modified until you say so

## Part of the production-audit collection

| Skill | What it audits |
|-------|---------------|
| [audit-secrets](https://github.com/vulk-corp/audit-secrets) | API keys in client code, database security rules, data over-exposure |
| [audit-access](https://github.com/vulk-corp/audit-access) | Authentication, unprotected routes, IDOR, input validation, roles |
| [audit-costs](https://github.com/vulk-corp/audit-costs) | AI spending caps, hosting limits, per-user rate limits, spam protection |
| [audit-monitoring](https://github.com/vulk-corp/audit-monitoring) | Error handling, monitoring, uptime alerts, backups, version control |
| [audit-legal](https://github.com/vulk-corp/audit-legal) | Privacy policy, code ownership, copyleft dependencies |
| [audit-code-quality](https://github.com/vulk-corp/audit-code-quality) | File sizes, god components, duplicated logic, naming, structure |

## Want continuous monitoring?

These prompts are a one-time check. [BWORLDS](https://www.bworlds.co) runs these checks automatically, continuously, and fixes what it finds.

## License

MIT
