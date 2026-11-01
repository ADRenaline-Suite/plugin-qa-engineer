---
name: qa-help
description: "ADRenaline. Help: catalog of plugin-qa-engineer (skills, rules, commands)."
---

# Help — ADRenaline QA Engineer

Print this catalog as the reply. Do not run any skill or command. Do not invent entries that are not listed. If a component was added to the plugin and is missing here, add one line from its frontmatter `description` and say the catalog was refreshed.

When this help command is the first command in the message, every command, skill, or rule named after it is the subject of the help. Do not run those names. Do not print the full catalog. For each name, in the order given, print its catalog line (the linked id and the sentence). When the README has a heading for that command, also print the paragraphs under that heading, up to the next heading. A skill name uses the skill's catalog line and the README group that names that skill, up to its first command heading. A name that is not in this catalog is one line: it is not in this plugin. Do not invent what it does, and do not write a file.

Write the sentences in the language of the request. Keep command names, file ids, and every URL unchanged. Every id is a markdown link to the GitHub URL on its line. Do not print a repository `name` as the visible label of a plugin.

Keep the section headings, in this order: Plugin, Commands, Skills, Rules, then Agents, Hooks, and MCP when the plugin has them, then Output, then Not in this plugin. The title and the Plugin line show `ADRenaline` plus the `displayName`, then one sentence on what the plugin does. Under Commands, group the lines by the skill named in the line. Each group opens with that skill name linked to its SKILL.md. One line per item: the linked id, then the sentence. Output links this plugin's GitHub repository under that same label. A plugin under Not in this plugin uses `ADRenaline` plus its short name, and links to `https://github.com/<owner>/<other-plugin>` only when that repository exists.

## Plugin

- [**ADRenaline QA Engineer**](https://github.com/ADRenaline-Suite/plugin-qa-engineer/blob/main/README.md) — Writes the scenario. The test code goes next to the code, in the project's existing style.

## Commands

- [**/qa-help**](https://github.com/ADRenaline-Suite/plugin-qa-engineer/blob/main/README.md) — This help (one-line catalog of the plugin).
- [**plan-tests**](https://github.com/ADRenaline-Suite/plugin-qa-engineer/blob/main/skills/plan-tests/SKILL.md) — Writes a test scenario for one use case, at one level and one type.
- [**/qa-scenario**](https://github.com/ADRenaline-Suite/plugin-qa-engineer/blob/main/skills/plan-tests/references/scenario.md) — Scenario: precondition, action, and expected result for one use case.
- [**/qa-level**](https://github.com/ADRenaline-Suite/plugin-qa-engineer/blob/main/skills/plan-tests/references/levels.md) — Level: component, integration, system, or acceptance, and where it sits in the pyramid.
- [**/qa-type**](https://github.com/ADRenaline-Suite/plugin-qa-engineer/blob/main/skills/plan-tests/references/types.md) — Type: functional, non-functional, structural, confirmation, or regression.

## Skills

- [**plan-tests**](https://github.com/ADRenaline-Suite/plugin-qa-engineer/blob/main/skills/plan-tests/SKILL.md) — Writes a test scenario for one use case, at one level and one type.

## Rules

- [**output-folder**](https://github.com/ADRenaline-Suite/plugin-qa-engineer/blob/main/rules/output-folder.mdc) — Every file goes in `adrenaline/qa-engineer/` (or in `outputDirs["plugin-qa-engineer"]` of `.cursor/adrenaline.json`). The artifact follows the language of the request.
- [**scenario-before-code**](https://github.com/ADRenaline-Suite/plugin-qa-engineer/blob/main/rules/scenario-before-code.mdc) — A test traces to a use case. Design review, WCAG, and model evaluation stay in their plugins.

## Output

- Repository: [**ADRenaline QA Engineer**](https://github.com/ADRenaline-Suite/plugin-qa-engineer).
- Folder: `adrenaline/qa-engineer/`. One named subject goes in `<subject>/`. `<NNN>` is monotonic across the whole folder.

## Not in this plugin

- Use case → ADRenaline plugin-project-manager.
- Design review → [**ADRenaline plugin-ui-ux-design**](https://github.com/ADRenaline-Suite/plugin-ui-ux-design).
- WCAG audit → ADRenaline plugin-accessibility.
- Model evaluation → ADRenaline plugin-ai-evaluation.
