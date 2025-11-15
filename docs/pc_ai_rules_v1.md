# Xavos — PC-AI Reglas v1

## 1. Alcance
PC-AI solo puede:
- Leer estado de hardware (CPU, RAM, disco, temperatura).
- Leer estado de red (online/offline).
- Leer logs del sistema de Xavos.

PC-AI NO puede:
- Borrar archivos fuera de carpetas de Xavos.
- Instalar o desinstalar programas.
- Apagar o reiniciar la PC sin confirmación.

## 2. Tareas básicas
- Registrar cada hora:
  - uso de CPU
  - uso de RAM
  - espacio en disco
- Registrar errores críticos que detecte.
- Generar un resumen diario de estado.

## 3. Confirmación obligatoria
Cualquier acción que cambie algo en el sistema (ej: limpiar espacio, cerrar procesos) requiere confirmación manual del usuario.
