<p align="right">Idioma:&emsp;<a href="README.md" style="vertical-align:middle"><img alt="English" src="https://raw.githubusercontent.com/ADRenaline-Suite/.github/main/profile/lang-en-off.svg" align="middle" style="vertical-align:middle"></a> <img alt="Español" src="https://raw.githubusercontent.com/ADRenaline-Suite/.github/main/profile/lang-es-on.svg" align="middle" style="vertical-align:middle"></p>

# QA (`plugin-qa-engineer`)

Escribe un escenario de prueba para un caso de uso, en un nivel y un tipo. La prueba automatizada va en el árbol de pruebas que el proyecto ya tiene.

Las instrucciones están en inglés. El archivo que guarda el plugin sigue el idioma del pedido. Los archivos van en `adrenaline/qa-engineer/`.

## /qa-scenario

Precondición, acción y resultado esperado. Arrange, act, assert. Un negativo cuando el comportamiento comprueba quién llama.

## /qa-level

Componente, integración, sistema o aceptación, y dónde queda eso frente a la pirámide.

## /qa-type

Funcional, no funcional, estructural, confirmación o regresión. Una medida sin número queda en hueco.

## Ayuda

## /qa-help

El catálogo de este plugin. No escribe un archivo.

## Para quién es

Quien quiere una comprobación trazada a un caso de uso. El caso de uso queda en `plugin-project-manager`. Una revisión de diseño queda en `plugin-ui-ux-design`. Una auditoría WCAG queda en `plugin-accessibility`. El comportamiento de un modelo queda en `plugin-ai-evaluation`. Este plugin no copia sus skills.

## Qué incluye

Portable, para cualquier agente que siga [Agent Skills](https://agentskills.io/specification):

- `plan-tests` escribe el escenario, el nivel y el tipo.

Cursor y Claude Code: los commands de arriba. En Cursor, `/qa-scenario`. En Claude Code, `/plugin-qa-engineer:qa-scenario`.

Solo Cursor: las rules `output-folder`, `scenario-before-code`. Claude Code no carga rules. Las mismas restricciones están en los skills.

## Instalar

En Cursor, instala el plugin desde este repositorio en Customize.

En Claude Code:

```text
claude plugin marketplace add ADRenaline-Suite/plugin-qa-engineer
claude plugin install plugin-qa-engineer@plugin-qa-engineer
```

Para probar una copia local, arranca Claude Code con `claude --plugin-dir <ruta de este repositorio>`.

## Ejemplo

Pide `/qa-scenario` y nombra el caso de uso. El archivo es el escenario. Si además pides automatizarlo, el archivo de prueba usa el sufijo que el proyecto ya usa (`*.spec.ts` o `*Tests.cs`).

## Configuración

El escenario va en `adrenaline/qa-engineer/`. El código de prueba se queda junto al código del proyecto. Una app nombrada va en `<subject>/`.

## Licencia

MIT. Copyright (c) 2026 Ricardo Plascencia.

