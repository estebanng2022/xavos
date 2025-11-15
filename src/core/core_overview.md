# Xavos — Core Overview

El core controla:
- configuración global del sistema
- carga de módulos (AI, wizard, templates, pipeline)
- registro de errores y logs
- autenticación local
- permisos de ejecución
- conexión entre los diferentes AIs

El core NO genera código.
El core NO habla directamente con proyectos externos.
El core solo coordina y valida todo.
