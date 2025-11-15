# Xavos — Commands Overview v1

## Objetivo
Definir el formato básico de las órdenes que el usuario le da a Xavos.

## Formato general

```text
<target>:
<acción en una frase>
<opciones adicionales>

Ejemplos

1) Orden a PC-AI

pc-ai:
revisar estado actual de la pc
detalle: corto

2) Orden al Wizard

wizard:
preparar blueprint de app flutter ligera
nombre: HarmoniaTest

3) Orden a Dev-AI

dev-ai:
generar estructura base del proyecto actual
modo: solo carpetas

Reglas

Siempre debe existir un target (pc-ai, assistant-ai, dev-ai, doc-ai, pipeline-ai, wizard).

La primera línea después de target: debe ser una acción clara.

Opciones adicionales son líneas tipo clave: valor.

Xavos siempre responde con un resumen y pide confirmación antes de ejecutar algo que cambie archivos o ejecute procesos.
