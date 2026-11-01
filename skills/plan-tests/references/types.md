# Type

<p align="right">Language:&emsp;<img alt="English" src="https://raw.githubusercontent.com/ADRenaline-Suite/.github/main/profile/lang-en-on.svg" align="middle" style="vertical-align:middle"> <a href="types.es.md" style="vertical-align:middle"><img alt="Español" src="https://raw.githubusercontent.com/ADRenaline-Suite/.github/main/profile/lang-es-off.svg" align="middle" style="vertical-align:middle"></a></p>

[🏠 QA Engineer](../../../README.md)

A bug fix has no test that would have caught it, or a performance hope is written as a functional case.

## Steps

1. Functional checks the use case result. Non-functional checks a measure the person gave (time, rate). If they gave no number, the measure is a gap.
2. Structural checks a path inside the code the person pointed at. Confirmation checks that a named fix holds. Regression checks that a named older behavior still holds.
3. Do not mark a test as all five types.

## Rules

1. A non-functional measure without a number stays a gap.

## Template

## Use case

## Type

## What it checks

## Measure

## Assumed

## Done

- [ ] The use case or the source this piece requires is named, or the file was not written.
- [ ] Every heading above is filled or marked as a gap. `proposed` when a gap remains.
- [ ] Nothing was invented: no field, no error, no date, no role, no legal basis.
- [ ] The subject folder and `STATUS.md` follow the skill.

Close the reply with what was written, where, and what is still a gap.
