# Contributing to FOSS HEAVEN

## The One Rule

> **Deploy it. Break it. Fix it. Then tell us about it.**

If you haven't actually used a tool in production or serious testing, don't submit it. "I heard it's good" is not good enough. "The README looks impressive" is not good enough. "It has a lot of stars" is not good enough.

---

## What We're Looking For

### Tool Submissions

New tools should meet ALL of these criteria:

1. **Actually deployed by you** — not just read about
2. **100% free** — no premium tiers, no "open core" with paid features
3. **OSI-approved license** — MIT, Apache-2.0, GPL, AGPL, BSD, etc.
4. **Actively maintained** — commits in the last 6 months, responsive maintainers
5. **Self-hostable** — can run on your own infrastructure without vendor dependencies
6. **Honest assessment** — you must include what sucks about it

### Corrections & Updates

- Tool died or was abandoned
- License changed to something restrictive
- Better alternative exists
- Information is outdated or wrong
- Broken links

### Deployment Notes

Real-world deployment experiences are gold. We want:

- What worked
- What broke
- What configuration was needed
- Resource requirements (RAM, CPU, disk)
- Time to get running
- Ongoing maintenance burden

---

## What We're NOT Looking For

- ❌ Tools you haven't used
- ❌ Affiliate links or referral codes
- ❌ Sponsored entries
- ❌ Marketing copy ("revolutionary," "game-changing," "AI-powered")
- ❌ Proprietary software
- ❌ "Open core" tools with paid feature gates
- ❌ GitHub star counts as a quality metric
- ❌ README-driven recommendations

---

## Submission Format

### For New Tools

Use this exact format:

```markdown
### [Tool Name](https://github.com/org/repo)
- **License:** [SPDX identifier]
- **Language:** [Primary language]
- **Category:** [One of: Infrastructure, Databases, Backend, Frontend, AI/ML, Security, Monitoring, Project Management, Dev Tools, Communication]
- **Complexity:** [Beginner / Intermediate / Advanced / Masochist]
- **What it does:** [One clear sentence]
- **Why it matters:** [One sentence on significance]
- **What sucks:** [Required. Every tool has problems.]
- **Deployment notes:** [Your actual experience]
- **Resource requirements:** [RAM, CPU, disk if known]
- **Verified by:** [@your-github-handle]
- **Last verified:** [YYYY-MM-DD]
```

**Example:**

```markdown
### Coolify
- **License:** AGPL-3.0
- **Language:** PHP / TypeScript
- **Category:** Infrastructure
- **Complexity:** Beginner
- **What it does:** Self-hosted PaaS that lets you deploy apps with git push
- **Why it matters:** The closest thing to Heroku you can run yourself for free
- **What sucks:** UI can be slow with 50+ projects. Documentation is improving but still sparse for edge cases. SQLite default is fine for small setups but you'll want PostgreSQL for production.
- **Deployment notes:** Ran on a $6 Hetzner VPS for 6 months. Handles 15 projects without issues. SSL auto-renewal works. Backup to S3 needs manual setup.
- **Resource requirements:** 2GB RAM minimum, 1 CPU, 20GB disk
- **Verified by:** @yourname
- **Last verified:** 2026-05-04
```

### For Corrections

Open an issue with:

```markdown
**Tool:** [Name]
**Problem:** [What's wrong]
**Evidence:** [Link to source, commit, or license change]
**Suggested fix:** [If you have one]
```

---

## Pull Request Process

1. **Fork the repo**
2. **Create a branch:** `git checkout -b add-tool-name` or `fix-tool-name`
3. **Make your changes** following the format above
4. **Test your markdown** renders correctly
5. **Submit PR** with a clear description

### PR Checklist

- [ ] I have deployed this tool myself
- [ ] The tool has an OSI-approved license
- [ ] The tool has no premium tiers or feature gates
- [ ] I included "What sucks" for every tool added
- [ ] I verified links work
- [ ] I used the correct submission format

---

## Review Process

We review PRs when we can. This is not our job. Expect:

- **Simple fixes (typos, broken links):** 1-7 days
- **New tool submissions:** 1-4 weeks (we may test it ourselves)
- **Major changes:** Discussion required

We may reject submissions that:
- Don't meet the criteria
- Lack honest criticism
- Read like marketing copy
- Haven't been verified by deployment

---

## Code of Conduct

Don't be a jerk. That's it.

- No harassment
- No spam
- No demanding updates or features
- No arguing about license interpretations (consult a lawyer)
- Respect that maintainers have jobs and lives

---

## Questions?

Open an issue. Don't email us. We don't check email.
