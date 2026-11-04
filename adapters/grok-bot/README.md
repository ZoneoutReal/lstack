# Adapter: Grok bots

## Roles → bots
One Grok bot per role. Bot instructions = role file; add the step's `SKILL.md` as a skill.

| Role | Instructions |
|---|---|
| Chet, the Editor-in-Chief (lead) | `roles/editor-in-chief.md` |
| Intake | `roles/intake.md` |
| Researcher | `roles/researcher.md` |
| Writer | `roles/writer.md` |
| Editor | `roles/editor.md` |
| Packager | `roles/packager.md` |
| Reviewer | `roles/reviewer.md` |

## Schedule
Create one routine per entry in `routines/schedule.yaml`, using the same cron and timezone. Set each routine to stay silent when its input file is missing or not done.
## Handoffs
Bots share this repo (clone on the box). Each writes only its step's file.
## Human gates
The lead bot messages a human only for the topic pick, the publish approval, and failures.
