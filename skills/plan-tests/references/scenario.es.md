# Escenario

<p align="right">Idioma:&emsp;<a href="scenario.md" style="vertical-align:middle"><img alt="English" src="https://raw.githubusercontent.com/ADRenaline-Suite/.github/main/profile/lang-en-off.svg" align="middle" style="vertical-align:middle"></a> <img alt="Español" src="https://raw.githubusercontent.com/ADRenaline-Suite/.github/main/profile/lang-es-on.svg" align="middle" style="vertical-align:middle"></p>

[🏠 QA Engineer](../../../README.md)

Existe una prueba que ningún caso de uso pidió, o el resultado esperado es 'funciona'.

## Pasos

1. Copia el objetivo del actor. El resultado esperado es la postcondición del caso de uso, o de una extensión nombrada.
2. Escribe arrange, act, assert en ese orden. Un escenario, un comportamiento.
3. Cuando el comportamiento comprueba quién llama, añade uno negativo: credencial ausente, o un rol que la persona nombró y que no debe pasar.
4. No inventes un resultado de producto.

## Reglas

1. La fila negativa es `None.` cuando el comportamiento no comprueba identidad ni permiso.

## Plantilla

## Caso de uso

## Nivel

## Tipo

## Arrange

## Act

## Assert

## Negativo

## Assumed

## Done

- [ ] El caso de uso o la fuente que esta pieza pide está nombrada, o el archivo no se escribió.
- [ ] Cada título de arriba está lleno o marcado como hueco. `proposed` si queda un hueco.
- [ ] No se inventó nada: ni un campo, ni un error, ni una fecha, ni un rol, ni una base legal.
- [ ] La subcarpeta del asunto y `STATUS.md` siguen el skill.

Cierra la respuesta con qué se escribió, dónde, y qué sigue siendo un hueco.
