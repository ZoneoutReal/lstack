# Adapter: Grok bots

## Roles → bots
One Grok bot per role. Bot instructions = role file; add the step's `SKILL.md` as a skill.

| Role | Instructions |
|---|---|
| Chet, the Editor-in-Chief (lead) | `roles/editor-in-chief.md` |
| Penny, the Intake | `roles/intake.md` |
| Rhett, the Researcher | `roles/researcher.md` |
| Wade, the Writer | `roles/writer.md` |
| Edie, the Editor | `roles/editor.md` |
| Pax, the Packager | `roles/packager.md` |
| Vera, the Reviewer | `roles/reviewer.md` |

## Schedule
Create one routine per entry in `routines/schedule.yaml`, using the same cron and timezone. Set each routine to stay silent when its input file is missing or not done.
## Handoffs
Bots share this repo (clone on the box). Each writes only its step's file.
## Human gates
The lead bot messages a human only for the topic pick, the publish approval, and failures.
