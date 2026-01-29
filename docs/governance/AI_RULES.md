# AI Rules for SageGap (Repo Safety)

## Non-Negotiables
1. **No direct pushes to `main`.** All changes must be via branch + PR.
2. **Small, reviewable PRs.** One intent per PR whenever possible.
3. **No secrets.** Never commit API keys, tokens, passwords, private URLs, or personal data.
4. **PII/PHI safety.** Never commit real student/family medical or education records.
5. **Explain changes.** Every PR must include what changed, why, and how to test.

## What AI Can Do
- Draft documentation, schemas, and ADRs
- Create scaffolding code and tests
- Refactor safely (small increments)
- Improve clarity and consistency
- Propose data models (privacy-aware)

## What Requires Explicit Human Approval
- Authentication/authorization changes
- Data storage/encryption decisions
- Any ingestion of emails, PDFs, medical/education records
- Anything affecting compliance posture (FERPA/HIPAA)
- Database migrations
- Production deployment workflows

## PR Requirements (AI must include)
- **Summary:** 3–6 bullets
- **Risk:** low/medium/high + why
- **Testing:** commands or steps
- **Privacy check:** confirm no PII/PHI/secrets included

## Commit Message Style
Use: `Area: short action`
Examples:
- `Docs: add Canonical Egg overview`
- `Infra: add CI lint workflow`
- `Schema: draft v0 child record types`

