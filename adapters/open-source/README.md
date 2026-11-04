# Adapter: open-source agent tools

Works with any tool that can read a prompt file and run on a schedule (e.g. Aider, OpenHands, Goose, LangGraph, CrewAI, a shell script around a local model).

## Roles → agents
| Role | Prompt file |
|---|---|
| Editor-in-Chief (lead) | `roles/editor-in-chief.md` |
| Intake | `roles/intake.md` |
| Researcher | `roles/researcher.md` |
| Writer | `roles/writer.md` |
| Editor | `roles/editor.md` |
| Packager | `roles/packager.md` |
| Reviewer | `roles/reviewer.md` |

Prompt = role file + skill file + `PRINCIPLES.md` + `AGREEMENTS.md`.

## Schedule
Translate `routines/schedule.yaml` to system crontab or a CI schedule (e.g. GitHub Actions `on: schedule`).
```
0 9 * * 4  ./run.sh editor skills/04-edit-and-polish/SKILL.md
```
## Handoffs
Files in `pipeline/<week>/` only. One commit per step.
## Human gates
Publish step checks `05-package.md` for "Human approved publish" ticked; otherwise it exits silently.
