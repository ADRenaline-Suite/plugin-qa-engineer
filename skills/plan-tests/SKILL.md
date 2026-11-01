---
name: plan-tests
description: Writes a test scenario for one use case, at one level and one type.
---

<p align="right">Language:&emsp;<img alt="English" src="https://raw.githubusercontent.com/ADRenaline-Suite/.github/main/profile/lang-en-on.svg" align="middle" style="vertical-align:middle"> <a href="SKILL.es.md" style="vertical-align:middle"><img alt="Español" src="https://raw.githubusercontent.com/ADRenaline-Suite/.github/main/profile/lang-es-off.svg" align="middle" style="vertical-align:middle"></a></p>

[🏠 QA Engineer](../../README.md)

# Writes a test scenario for one use case, at one level and one type

One scenario says the precondition, the action, and the result. The level says how wide the harness is. The type says what kind of check it is.

Source: ISTQB Foundation levels and types. ISTQB CT-TAS v1.0 (November 2024) for the pyramid, the ice-cream cone, the hourglass, and the umbrella. Arrange-Act-Assert as Fowler records it.

## Before writing

1. Read only the reference this command names: [scenario](references/scenario.md), [levels](references/levels.md), or [types](references/types.md).
2. The use case is required. Without it, write nothing.

References: [scenario](references/scenario.md), [levels](references/levels.md), [types](references/types.md).

## Delivery

The scenario file goes in the output folder. The automated test goes in the project's test tree. Angular projects that already use `*.spec.ts` keep that suffix. .NET projects that already use `*Tests.cs` keep that suffix. Do not rename the project's tests.

Every file this skill writes goes in `adrenaline/qa-engineer/`, or in `outputDirs["plugin-qa-engineer"]` when `.cursor/adrenaline.json` gives a valid relative path. If `adrenaline/qa-engineer/` does not exist yet and `qa-engineer/` at the project root already has this plugin's `ORIGIN.json` or `STATUS.md`, keep writing there and say so.

When the person names one project, app, service, or domain, put that subject's file in `<subject>/`. A file about the whole product stays at the output root. `<NNN>` is the next free number in the whole output folder. The `archivo` cell is `<subject>/<file>` when there is a subject (`doc/arch/adr-008-asunto-subcarpeta.md`).

Write `ORIGIN.json` beside `STATUS.md` when the folder is created, and again only if it is missing or a field differs. Fields: `suite` `ADRenaline-Suite`, `plugin` `plugin-qa-engineer`, `repository` `https://github.com/ADRenaline-Suite/plugin-qa-engineer`, `convention` `adr-001`. It is not an `<NNN>` file and it has no row in `STATUS.md`.

Do not invent a fact the person did not give. A required heading with no fact stays a gap and the file stays `proposed`. "None." fills a heading.

## Done

- [ ] Only the reference for this command was applied.
- [ ] The output folder, the subject subfolder, `ORIGIN.json`, and `STATUS.md` match the delivery rules.
- [ ] A missing required fact is a gap. The file stays `proposed`.

## Example

A request that names the piece and its source writes one file. A request missing that source writes nothing and names the gap.
