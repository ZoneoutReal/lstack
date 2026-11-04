# Adapter: Claude

## Roles → agents
Create one Claude Project (or Claude Code subagent in `.claude/agents/<role>.md`) per role. System prompt = the role file + its skill file + `PRINCIPLES.md` + `AGREEMENTS.md`.

| Role | Prompt source |
|---|---|
| Editor-in-Chief (lead) | `roles/editor-in-chief.md` |
| Intake | `roles/intake.md` |
| Researcher | `roles/researcher.md` |
| Writer | `roles/writer.md` |
| Editor | `roles/editor.md` |
| Packager | `roles/packager.md` |
| Reviewer | `roles/reviewer.md` |

## Schedule
Run each step from cron using `routines/schedule.yaml`, e.g.:
```
0 9 * * 2  cd ~/lstack && claude -p "Act as roles/researcher.md. Run skills/02-research-pass/SKILL.md for this week." 
```
## Handoffs
Agents read and write only `pipeline/<week>/`. Commit after each step.
## Human gates
Lead pick and publish approval: the lead agent opens a PR or writes `APPROVAL_NEEDED.md`; a human merges.
