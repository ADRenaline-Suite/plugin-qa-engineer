---
name: plan-tests
description: Escribe un escenario de prueba para un caso de uso, en un nivel y un tipo.
---

<p align="right">Idioma:&emsp;<a href="SKILL.md" style="vertical-align:middle"><img alt="English" src="https://raw.githubusercontent.com/ADRenaline-Suite/.github/main/profile/lang-en-off.svg" align="middle" style="vertical-align:middle"></a> <img alt="Español" src="https://raw.githubusercontent.com/ADRenaline-Suite/.github/main/profile/lang-es-on.svg" align="middle" style="vertical-align:middle"></p>

[🏠 QA Engineer](../../README.md)

# Escribe un escenario de prueba para un caso de uso, en un nivel y un tipo

Un escenario dice la precondición, la acción y el resultado. El nivel dice qué tan amplio es el arnés. El tipo dice qué clase de comprobación es.

Source: Niveles y tipos de ISTQB Foundation. ISTQB CT-TAS v1.0 (noviembre de 2024) para la pirámide, el cono de helado, el reloj de arena y el paraguas. Arrange-Act-Assert como lo registra Fowler.

## Antes de escribir

1. Lee solo la referencia que nombra este command: [scenario](references/scenario.md), [levels](references/levels.md) o [types](references/types.md).
2. El caso de uso es obligatorio. Sin él, no escribas nada.

References: [scenario](references/scenario.md), [levels](references/levels.md), [types](references/types.md).

## Entrega

El archivo del escenario va en la carpeta de salida. La prueba automatizada va en el árbol de pruebas del proyecto. Los proyectos Angular que ya usan `*.spec.ts` conservan ese sufijo. Los proyectos .NET que ya usan `*Tests.cs` conservan ese sufijo. No renombres las pruebas del proyecto.

Cada archivo de este skill va en `adrenaline/qa-engineer/`, o en `outputDirs["plugin-qa-engineer"]` si `.cursor/adrenaline.json` da una ruta relativa válida. Si `adrenaline/qa-engineer/` aún no existe y `qa-engineer/` en la raíz del proyecto ya tiene el `ORIGIN.json` o el `STATUS.md` de este plugin, sigue escribiendo ahí y dilo.

Si la persona nombra un proyecto, una app, un servicio o un dominio, el archivo de ese asunto va en `<subject>/`. Un archivo de todo el producto se queda en la raíz de la salida. `<NNN>` es el siguiente número libre en toda la carpeta. La celda `archivo` es `<subject>/<file>` cuando hay asunto (`doc/arch/adr-008-asunto-subcarpeta.md`).

Escribe `ORIGIN.json` junto a `STATUS.md` al crear la carpeta, y otra vez solo si falta o un campo difiere. Campos: `suite` `ADRenaline-Suite`, `plugin` `plugin-qa-engineer`, `repository` `https://github.com/ADRenaline-Suite/plugin-qa-engineer`, `convention` `adr-001`. No es un archivo `<NNN>` y no tiene fila en `STATUS.md`.

No inventes un dato que la persona no dio. Un título obligatorio sin dato queda como hueco y el archivo sigue `proposed`. "None." llena un título.

## Done

- [ ] Solo se aplicó la referencia de este command.
- [ ] La carpeta de salida, la subcarpeta del asunto, `ORIGIN.json` y `STATUS.md` coinciden con las reglas de entrega.
- [ ] Un dato obligatorio que falta es un hueco. El archivo sigue `proposed`.

## Example

Un pedido que nombra la pieza y su fuente escribe un archivo. Un pedido sin esa fuente no escribe nada y nombra el hueco.
