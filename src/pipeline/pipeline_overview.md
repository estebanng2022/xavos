# Xavos — Pipeline Overview

El Pipeline es el sistema de calidad de Xavos.

## Etapas del Pipeline

1. Análisis estático
   - lint
   - formateo
   - estructura básica

2. Arquitectura
   - capas correctas
   - dependencias permitidas
   - sin lógica de negocio en la UI

3. Design System
   - sin colores hardcode
   - sin tipografías sueltas
   - uso correcto de componentes

4. Tests
   - unit tests
   - widget/UI tests
   - integración básica

5. Checklist final
   - versión incrementada
   - changelog
   - listo para build

Si alguna etapa falla, el deploy se bloquea.