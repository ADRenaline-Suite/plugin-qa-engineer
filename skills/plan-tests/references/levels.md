# Level

<p align="right">Language:&emsp;<img alt="English" src="https://raw.githubusercontent.com/ADRenaline-Suite/.github/main/profile/lang-en-on.svg" align="middle" style="vertical-align:middle"> <a href="levels.es.md" style="vertical-align:middle"><img alt="Español" src="https://raw.githubusercontent.com/ADRenaline-Suite/.github/main/profile/lang-es-off.svg" align="middle" style="vertical-align:middle"></a></p>

[🏠 QA Engineer](../../../README.md)

Everything is called end-to-end, so a domain rule waits on a browser.

## Steps

1. Name one level. Component covers one unit with no infrastructure. Integration covers one boundary (database, HTTP, queue) without the whole product. System covers a flow through the deployed parts the person named. Acceptance covers the use case as the actor sees it.
2. Prefer the lowest level that can fail for this behavior. Say so.
3. If the project is an ice-cream cone, an hourglass, or an umbrella, name that shape and the level this scenario moves toward. Do not pretend the pyramid already exists.

## Rules

1. Do not add a browser test for a rule that has no UI.

## Template

## Use case

## Level

## Why this level

## Current shape

## Assumed

## Done

- [ ] The use case or the source this piece requires is named, or the file was not written.
- [ ] Every heading above is filled or marked as a gap. `proposed` when a gap remains.
- [ ] Nothing was invented: no field, no error, no date, no role, no legal basis.
- [ ] The subject folder and `STATUS.md` follow the skill.

Close the reply with what was written, where, and what is still a gap.
