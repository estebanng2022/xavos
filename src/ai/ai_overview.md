# Xavos — AI Overview

El sistema AI de Xavos está dividido en módulos:

## 1. PC-AI
- Monitorea hardware
- Captura errores del sistema
- Gestiona actualizaciones de la PC
- Revisa estado de red y seguridad

## 2. Assistant-AI
- Ayuda a pensar, organizar y planear
- Lee blueprints
- Sugiere pasos y estructura
- Nunca ejecuta acciones

## 3. Dev-AI
- Genera código
- Aplica templates y DS
- Modifica archivos dentro del proyecto actual

## 4. Doc-AI
- Lee changelogs
- Detecta cambios en SDKs y permisos
- Reporta riesgos o actualizaciones

## 5. Pipeline-AI
- Corre pruebas
- Analiza calidad
- Bloquea deploy si hay fallos

Cada AI tiene límites definidos por `xavos_rules.md`.