---
name: error-experience-learner
description: Capture errors, failed commands, user corrections, outdated knowledge, missing capabilities, and better recurring approaches so future agent runs avoid repeating the same mistakes. Mapped from the public `self-improvement` skill pattern.
metadata:
  source_status: "mapped-from-public-skill"
  mapped_from: "self-improvement, self-improving-agent"
  source_url: "https://github.com/sundial-org/awesome-openclaw-skills/blob/main/skills/self-improvement/SKILL.md"
  aliases: "self-improvement, self-improving-agent, learning-log"
---

# Error Experience Learner

Use this skill to turn mistakes and corrections into reusable operational memory. The agent should log learnings immediately after failures or user corrections, then review them before major work.

## When to use

Use this skill when:

- A command, script, build, deployment, API call, browser action, or download fails unexpectedly.
- The user corrects the agent.
- The agent discovers that a previous assumption was outdated or wrong.
- A missing capability or missing skill is discovered.
- A better approach is found for a task that may recur.
- A tool has a non-obvious gotcha, authentication requirement, rate limit, or environment issue.

## Workspace files

Create a `.learnings/` directory in the active project or OpenClaw workspace:

```text
.learnings/
├── LEARNINGS.md
├── ERRORS.md
└── FEATURE_REQUESTS.md
```

## Logging rules

### Error entry

Append to `.learnings/ERRORS.md`:

```markdown
## [ERR-YYYYMMDD-XXX] short-error-name

**Logged**: ISO-8601 timestamp
**Priority**: low | medium | high | critical
**Status**: pending | resolved | promoted
**Area**: frontend | backend | infra | tests | docs | config | browser | data | marketing

### Summary
What failed in one sentence.

### Error
```text
Exact error message or relevant output.
```

### Context
- Task attempted:
- Command/tool/API:
- Inputs:
- Environment:

### Suspected Cause

### Suggested Fix

### Metadata
- Reproducible: yes | no | unknown
- Related files:
- Tags:
```

### Learning entry

Append to `.learnings/LEARNINGS.md`:

```markdown
## [LRN-YYYYMMDD-XXX] category

**Logged**: ISO-8601 timestamp
**Priority**: low | medium | high | critical
**Status**: pending | resolved | promoted
**Area**: frontend | backend | infra | tests | docs | config | browser | data | marketing

### Summary
What should be remembered.

### Details
What happened, what was wrong, and what is correct.

### Rule for Future Runs
State the reusable rule plainly.

### Metadata
- Source: conversation | error | user_feedback | investigation
- Related files:
- Tags:
```

### Feature request entry

Append to `.learnings/FEATURE_REQUESTS.md`:

```markdown
## [FEAT-YYYYMMDD-XXX] capability-name

**Logged**: ISO-8601 timestamp
**Priority**: low | medium | high | critical
**Status**: pending | planned | shipped | declined

### Requested Capability

### User Context

### Suggested Implementation

### Dependencies
```

## Promotion rules

Promote learnings that are broadly useful:

- Project convention → `CLAUDE.md`, `AGENTS.md`, or equivalent project memory.
- Workflow rule → `AGENTS.md`.
- Tool gotcha → `TOOLS.md` or project docs.
- Repeated issue → convert to a reusable skill or checklist.

## Review checklist before major tasks

- Search `.learnings/` for the project, tool, API, framework, and task name.
- Read unresolved high-priority errors first.
- Apply promoted rules before running tools.
- Update status when a fix is verified.
