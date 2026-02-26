# CLAUDE.md — AI Assistant Guide for Awesome-Hacking

## Project Overview

**Awesome-Hacking** is a curated collection of awesome lists for hackers, pentesters, and security researchers. It is maintained under the [Hack-with-Github](https://github.com/Hack-with-Github) organization. The repository itself contains no code — it is a community-driven directory of links to security-related GitHub repositories and resources.

- **License:** CC0 1.0 Universal (Public Domain)
- **Primary file:** `README.md` — the entire curated list lives here

## Repository Structure

```
.
├── .github/
│   └── workflows/
│       └── lock-threads.yml   # Auto-locks stale issues/PRs after 7 days of inactivity
├── awesome_hacking.jpg        # Banner image displayed at the top of README
├── contributing.md             # Contribution guidelines for new submissions
├── LICENSE                     # CC0 1.0 Universal license
└── README.md                  # The curated list of awesome security repositories
```

## README.md Structure

The README is organized into these sections (in order):

1. **Banner image** — `awesome_hacking.jpg`
2. **Title and badges** — Project title with a Twitter share badge
3. **Awesome Repositories** — Primary curated table of security-focused awesome lists (sorted alphabetically by name)
4. **Other Useful Repositories** — Secondary table of supplementary security resources (sorted alphabetically by name)
5. **Need More?** — Links to social media accounts (Twitter, Facebook)
6. **Contributions** — Link to `contributing.md`

Both tables use the format:

```markdown
Repository | Description
---- | ----
[Name](URL) | Short description
```

## Contribution Conventions

When editing this repository, follow these rules:

### Adding a new entry
- Add it to the appropriate table in `README.md` ("Awesome Repositories" for primary awesome lists, "Other Useful Repositories" for supplementary resources)
- **Maintain alphabetical order** within each table — this is explicitly required by `contributing.md`
- Use the established table row format: `[Repository Name](URL) | Brief description`
- Keep descriptions concise (one sentence)
- Ensure the linked repository is actively maintained and relevant to security/hacking

### Removing an entry
- Remove entries that return 404 or are no longer maintained
- Open an issue or PR to discuss removal if uncertain

### Formatting
- Do not add trailing whitespace
- Use consistent tab/space alignment matching existing rows (tabs between columns)
- Do not modify the table header format (`---- | ----`)

## CI/CD & Automation

- **Lock Threads Workflow** (`.github/workflows/lock-threads.yml`): Runs hourly via cron. Automatically locks issues and pull requests that have been inactive for 7 days. Uses `dessant/lock-threads@v5`.
- There are no build steps, tests, or linting configured — this is a documentation-only repository.

## Development Workflow

1. **No build process** — Changes are purely Markdown edits
2. **No tests** — Validate changes by visual inspection of Markdown rendering
3. **PRs are the primary contribution method** — All external changes come via pull requests
4. **Branch from `master`** — The default branch is `master` (not `main`)

## Key Reminders for AI Assistants

- This repository is **content-only** (Markdown + one image). There is no code to run, build, or test.
- Always keep entries in **alphabetical order** within their respective tables.
- When adding entries, pick the correct table: "Awesome Repositories" for curated awesome-lists, "Other Useful Repositories" for tools, references, and other resources.
- Verify that any new URLs point to real, active repositories before adding them.
- Respect the CC0 public domain license — no attribution is legally required, but the project appreciates contributor recognition in `contributing.md`.
- The repository uses `master` as the default branch.
