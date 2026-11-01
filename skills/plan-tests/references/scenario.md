# Scenario

<p align="right">Language:&emsp;<img alt="English" src="https://raw.githubusercontent.com/ADRenaline-Suite/.github/main/profile/lang-en-on.svg" align="middle" style="vertical-align:middle"> <a href="scenario.es.md" style="vertical-align:middle"><img alt="Español" src="https://raw.githubusercontent.com/ADRenaline-Suite/.github/main/profile/lang-es-off.svg" align="middle" style="vertical-align:middle"></a></p>

[🏠 QA Engineer](../../../README.md)

A test exists that no use case asked for, or the expected result is 'it works'.

## Steps

1. Copy the actor's goal. The expected result is the postcondition of the use case, or of one named extension.
2. Write arrange, act, assert in that order. One scenario, one behavior.
3. When the behavior checks who is calling, add one negative: missing credential, or a role the person named that must not pass.
4. Do not invent a product outcome.

## Rules

1. The negative row is `None.` when the behavior does not check identity or permission.

## Template

## Use case

## Level

## Type

## Arrange

## Act

## Assert

## Negative

## Assumed

## Done

- [ ] The use case or the source this piece requires is named, or the file was not written.
- [ ] Every heading above is filled or marked as a gap. `proposed` when a gap remains.
- [ ] Nothing was invented: no field, no error, no date, no role, no legal basis.
- [ ] The subject folder and `STATUS.md` follow the skill.

Close the reply with what was written, where, and what is still a gap.
