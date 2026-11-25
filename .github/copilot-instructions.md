# Agent skills

This repo has a set of engineering skills in `.github/skills/`. Type `/skill-name` to run one. Run `/ask-skills` if you do not know which skill fits.

## First step in a new repo

Run `/setup-skills` once. It records the issue tracker and the domain doc layout in `docs/agents/`. Most planning skills read those files.

## Skills you run by hand

| Command | Use |
|---|---|
| `/ask-skills` | Find the skill that fits your situation. |
| `/setup-skills` | One-time repo setup. |
| `/probe-me` | Interview about a plan. Saves nothing. |
| `/probe-with-docs` | Interview that also updates `GLOSSARY.md` and ADRs. |
| `/to-spec` | Turn the conversation into a spec. |
| `/to-tickets` | Split a spec into tickets with blocking edges. |
| `/implement` | Build a spec or a ticket with TDD, then review. |
| `/plan-big` | Plan very large work as a map of decision tickets. |
| `/improve-codebase-architecture` | Find deepening opportunities in the code. |
| `/retro` | Suggest improvements to the agent environment. |

## Skills that you or Copilot can load

`probing`, `domain-modeling`, `codebase-design`, `tdd`, `diagnosing-bugs`, `code-review`, `pr`, `prototype`, `research`, `wizard`, `writing-for-agents`.

## Custom agents

The folder `.github/agents/` holds three read-only or narrow agents: `standards-reviewer`, `spec-reviewer`, and `researcher`. The `code-review`, `research`, and `plan-big` skills use them for sub-agent work.

## Project vocabulary

- If `GLOSSARY.md` exists, use its terms in code, tickets, and replies.
- If `docs/adr/` exists, read the ADRs that touch the area you change.
- If your work contradicts an ADR, say so before you continue.
