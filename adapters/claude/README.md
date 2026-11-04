# Adapter: Claude

## Roles → agents
Create one Claude Project (or Claude Code subagent in `.claude/agents/<role>.md`) per role. System prompt = the role file + its skill file + `PRINCIPLES.md` + `AGREEMENTS.md`.

| Role | Prompt source |
|---|---|
| Chet, the Editor-in-Chief (lead) | `roles/editor-in-chief.md` |
| Penny, the Intake | `roles/intake.md` |
| Rhett, the Researcher | `roles/researcher.md` |
| Wade, the Writer | `roles/writer.md` |
| Edie, the Editor | `roles/editor.md` |
| Pax, the Packager | `roles/packager.md` |
| Vera, the Reviewer | `roles/reviewer.md` |

## Schedule
Run each step from cron using `routines/schedule.yaml`, e.g.:
```
0 9 * * 2  cd ~/lstack && claude -p "Act as roles/researcher.md. Run skills/02-research-pass/SKILL.md for this week." 
```
## Handoffs
Agents read and write only `pipeline/<week>/`. Commit after each step.
## Human gates
Lead pick and publish approval: the lead agent opens a PR or writes `APPROVAL_NEEDED.md`; a human merges.
