<p align="right">Language:&emsp;<img alt="English" src="https://raw.githubusercontent.com/ADRenaline-Suite/.github/main/profile/lang-en-on.svg" align="middle" style="vertical-align:middle"> <a href="README.es.md" style="vertical-align:middle"><img alt="Español" src="https://raw.githubusercontent.com/ADRenaline-Suite/.github/main/profile/lang-es-off.svg" align="middle" style="vertical-align:middle"></a></p>

# QA Engineer (`plugin-qa-engineer`)

Writes a test scenario for one use case, at one level and one type. The automated test goes in the project's existing test tree.

The instructions are in English. The file the plugin saves follows the language of the request. Files go in `adrenaline/qa-engineer/`.

## /qa-scenario

Precondition, action, and expected result. Arrange, act, assert. One negative when the behavior checks who is calling.

## /qa-level

Component, integration, system, or acceptance, and where that sits against the pyramid.

## /qa-type

Functional, non-functional, structural, confirmation, or regression. A measure without a number stays a gap.

## Help

## /qa-help

The catalog of this plugin. It does not write a file.

## Who it is for

Someone who wants a check that traces to a use case. The use case stays with `plugin-project-manager`. A design review stays with `plugin-ui-ux-design`. A WCAG audit stays with `plugin-accessibility`. Model behavior stays with `plugin-ai-evaluation`. This plugin does not copy their skills.

## What it includes

Portable, for any agent that follows [Agent Skills](https://agentskills.io/specification):

- `plan-tests` writes the scenario, the level, and the type.

Cursor and Claude Code: the commands above. In Cursor, `/qa-scenario`. In Claude Code, `/plugin-qa-engineer:qa-scenario`.

Cursor only: rules `output-folder`, `scenario-before-code`. Claude Code does not load rules. The same restrictions are in the skills.

## Install

In Cursor, install the plugin from this repository in Customize.

In Claude Code:

```text
claude plugin marketplace add ADRenaline-Suite/plugin-qa-engineer
claude plugin install plugin-qa-engineer@plugin-qa-engineer
```

To try a local copy, start Claude Code with `claude --plugin-dir <path to this repository>`.

## Example

Ask `/qa-scenario` and name the use case. The file is the scenario. If you also ask to automate it, the test file uses the suffix the project already uses (`*.spec.ts` or `*Tests.cs`).

## Configuration

The scenario goes in `adrenaline/qa-engineer/`. The test code stays next to the project's code. One named app goes in `<subject>/`.

## License

MIT. Copyright (c) 2026 Ricardo Plascencia.

