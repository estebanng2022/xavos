# Xavos — Configuración Base

## 1. Rutas principales
- Carpeta raíz de proyectos: `C:\Xavos\projects`
- Carpeta de logs: `C:\Xavos\logs`
- Carpeta de plantillas (templates): `C:\Xavos\templates`

*(Estas rutas son temporales, se ajustarán cuando la PC exista.)*

## 2. Control de AIs
- PC-AI: habilitado
- Assistant-AI: habilitado
- Dev-AI: habilitado
- Doc-AI: habilitado
- Pipeline-AI: habilitado

## 3. Seguridad
- Modos permitidos:
  - `read_only` (solo leer)
  - `safe_write` (escribir solo dentro de rutas Xavos)
- Modo actual: `safe_write`
- Requiere confirmación para:
  - instalar software
  - borrar archivos
  - ejecutar builds

## 4. Proyectos
- Stacks permitidos:
  - `flutter`
  - `android_native`
- DS por defecto: pendiente de definir
- Módulos por defecto:
  - auth: desactivado
  - gps: desactivado
  - scan: desactivado
  - docs: desactivado
  - notificaciones: desactivado
