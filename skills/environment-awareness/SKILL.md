---
name: environment-awareness
description: Inspect the current project, runtime, operating system, package manager, framework, environment variables, ports, deployment target, and available tools before making build, website, or deployment changes.
metadata:
  source_status: "custom-gap-fill"
  aliases: "project-environment-check, runtime-awareness"
---

# Environment Awareness

Use this skill before running commands, editing project structure, installing dependencies, starting servers, or deploying a website.

## When to use

Use when the agent is about to:

- Modify an existing codebase.
- Run package manager commands.
- Start or stop servers.
- Add environment variables.
- Change build, CI/CD, or deployment configuration.
- Generate a website in an unknown stack.
- Troubleshoot errors that may depend on OS, shell, runtime, or package manager.

## Inspection checklist

```markdown
## Environment Snapshot
- OS / shell:
- Working directory:
- Git status:
- Package manager:
- Runtime versions:
- Framework:
- Build tool:
- Test command:
- Dev server command:
- Deployment target:
- Existing env files:
- Ports in use:
```

## Workflow

1. Read project files: `package.json`, lockfiles, config files, README, `.env.example`, deployment config.
2. Identify package manager from lockfile.
3. Identify framework and build commands.
4. Check git status before edits.
5. Avoid overwriting user changes.
6. Prefer minimal changes that fit the existing project.
7. Record environment gotchas in `.learnings/ERRORS.md` or `.learnings/LEARNINGS.md`.

## Output format

```markdown
# Environment Assessment

## Detected Stack

## Safe Commands
| Task | Command | Notes |
|---|---|---|

## Risks

## Recommended Next Step
```

## Guardrails

- Do not delete files or reset git state without explicit permission.
- Do not replace package managers.
- Do not assume `npm` if `pnpm-lock.yaml`, `yarn.lock`, or `bun.lockb` exists.
- Do not expose secret values from `.env` files.
