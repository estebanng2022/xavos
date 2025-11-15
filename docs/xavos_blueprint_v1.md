# Xavos — Blueprint v1

## 1. Visión

Xavos es mi programa local para crear y mantener:
- apps mobile
- programas de PC
- y más adelante páginas web

Siempre usando:
- plantillas propias
- reglas de calidad
- herramientas que yo realmente domino.

## 2. Objetivo principal

Que al presionar **“New Project”** en Xavos:
- aparezca un **wizard** con preguntas claras
- pueda elegir:
  - proyecto basado en plantilla (pre-hecho)
  - proyecto personalizado
- y el resultado siempre sea un proyecto organizado y premium.

## 3. Piezas principales del programa

### 3.1 Wizard de proyectos

- Preguntas clave:
  - tipo de proyecto (app mobile, programa PC, web futura)
  - stack (Flutter / Android nativo, etc.)
  - módulos a incluir (auth, gps, scan, docs, notificaciones…)
- Opción de usar plantillas ya hechas.
- Opción de proyecto 100% personalizado.
- Siempre muestra un **resumen final** antes de crear nada.
- Nada se genera sin confirmación explícita.

### 3.2 Editor integrado (sencillo)

- Editor de código básico dentro de Xavos.
- No compite con VSCode / Android Studio:
  - sirve para cambios rápidos
  - revisar archivos clave
- Permite:
  - ver y editar archivos de proyecto
  - hacer pequeños ajustes sin salir del programa.

### 3.3 Modo visual tipo “Figma”

- Vista visual de la pantalla (no solo código).
- Elementos principales:
  - lista de widgets disponibles
  - zona central de diseño
  - panel de propiedades (scroll, padding, opciones del scaffold, etc.)
- Flujo:
  - coloco widgets visualmente
  - ajusto propiedades
  - confirmo cambios
  - Xavos actualiza el código real de forma ordenada.

### 3.4 Theme y Design System propios

- Xavos tendrá un **DS y theme base** definidos por nosotros.
- El usuario podrá personalizar:
  - colores (ej: cambiar tono de verde)
  - algunos parámetros visuales
- Siempre bajo reglas:
  - nada de colores locos fuera del sistema
  - nada que rompa la organización
- Si un proyecto trae su propio DS:
  - Xavos respeta el DS del proyecto.

#### 3.4.1 Modelo de DS maestro + copia por cliente

- Xavos tendrá un **Design System maestro** (mi DS base) que vive fuera de los proyectos de clientes.
- Cuando se crea un proyecto para un cliente:
  - Xavos genera una **copia/snapshot** del DS maestro dentro del repo del cliente.
  - Esa copia se puede adaptar (colores, tamaños, algunos componentes) sin romper el DS maestro.
- La app del cliente:
  - siempre compila sola, sin necesitar Xavos.
  - siempre incluye su propio DS dentro del proyecto.
- Frase correcta:
  - “La app incluye una copia adaptada de mi DS maestro”
  - NO: “La app depende de Xavos para su DS”.

### 3.5 Biblioteca de widgets y templates

- Widgets base premium:
  - AppScaffold
  - Buttons
  - TextFields
  - List items
  - Cards
  - Navigation, etc.
- Pantallas tipo:
  - auth
  - dashboard
  - lista
  - detalle
  - settings
- Módulos listos para usar:
  - auth, gps, scan, docs, notificaciones (futuro)
- Integración con el modo visual:
  - al elegir un widget/plantilla, se puede insertar en la pantalla actual
  - el código se genera/actualiza siguiendo el DS.

### 3.6 AI Control Room (equipo de AIs)

- Xavos tendrá una pantalla donde se vean los AIs como “perfiles": 
  - nombre
  - rol (Dev-AI, Doc-AI, Pipeline-AI, Wizard, Commander, etc.)
  - estado (activo / pausado)
  - alcance (qué puede tocar y qué no)
- Desde esta pantalla se podrá:
  - cambiar nombre
  - ajustar reglas y alcance
  - activar/pausar AIs
- Habrá un **único Commander-AI**:
  - lee estado del proyecto y tareas
  - decide qué módulo (Dev-AI, Doc-AI, Pipeline-AI…) debe actuar
  - nunca escribe código directo, solo coordina.

### 3.7 AI Help (botón flotante dentro de Xavos)

- Un botón flotante dentro del programa que abre un “AI de ayuda” interno.
- Este AI ve:
  - en qué parte de Xavos estoy (wizard, editor, visual, pipeline, etc.)
  - qué proyecto/archivo está activo
- Puede:
  - explicar qué está pasando
  - sugerir el siguiente paso
  - señalar errores de configuración
- No ejecuta cambios sin confirmación:
  - solo propone, yo decido.

### 3.8 Tasks, recordatorios y calendario

- Sistema interno de tareas por proyecto:
  - tareas simples (pendiente / en progreso / hecho)
  - ligado a proyectos y módulos.
- Recordatorios:
  - “revisar proyecto X”
  - “SDK tal se vuelve obsoleto en tal fecha”
- Vista tipo calendario:
  - ver las tareas y mantenimientos distribuidos en el tiempo.
- Todo manejado desde Xavos, sin depender de apps externas.

### 3.9 Component & DS Library Screen

- Pantalla especial para ver los **recursos disponibles por lenguaje**.

Separado por lenguaje:
- Tabs:
  - `Flutter`
  - `Android Native`
  - (futuro) `Web`

Dentro de cada tab:
- **Widgets globales**
  - Buttons, TextFields, AppScaffold, listas, cards, etc.
- **Theme**
  - paleta de colores, tipografía, spacing, elevation.
- **Design System**
  - tokens
  - patrones
  - componentes premium.

Estructura de la pantalla:
- Panel izquierdo:
  - categorías / folders (Buttons, Layout, Inputs, Navigation…)
- Panel central:
  - lista de widgets / componentes / tokens
- Panel derecho:
  - documentación corta
  - props importantes
  - ejemplo de uso
  - (más adelante) en qué proyectos está usado.

Funciones:
- Click en un widget:
  - “Ver ejemplo de código”
  - “Inserción en pantalla actual (modo visual)”
- Todo bien documentado y separado por lenguaje.

### 3.10 Project Screen & Canvas Views

#### 3.10.1 Project Screen (Home)

- Pantalla principal del proyecto (ej: “Copilot Road”).
- Muestra:
  - nombre del proyecto y estado (Exploración / Diseño / Desarrollo / Mantenimiento)
  - porcentaje de avance
  - fase actual y próximo paso importante
  - lista de pasos/fases con checklist (qué está hecho y qué falta)
- Incluye acceso directo a:
  - Documentos del proyecto (blueprints, notas, changelog)
  - Canvas del proyecto (UI y lógica)

#### 3.10.2 UI Canvas (modo visual de pantallas)

- Vista tipo Figma para construir pantallas.
- Elementos:
  - área central con la pantalla
  - lista de widgets disponibles
  - panel de propiedades (scroll, padding, opciones del scaffold, etc.)
- Flujo:
  - arrastrar y colocar widgets
  - ajustar propiedades
  - confirmar cambios
  - Xavos actualiza el código real manteniendo la estructura limpia.

#### 3.10.3 Logic Canvas (System Map)

- Vista lógica del proyecto (no de diseño visual).
- Se usa para ver:
  - pantallas y navegación entre ellas
  - módulos (auth, gps, scan, docs, notificaciones)
  - conexiones con backend / APIs / DB / otros sistemas
- Usa cajas, iconos y flechas para mostrar el flujo.
- Soporta varios niveles de zoom:
  - vista ecosistema (usuario, dispositivo, backend)
  - vista sistema (módulos y capas)
  - vista zona (solo un módulo o parte de la app)
- Cada caja está vinculada a rutas reales del proyecto (folders, archivos, pantallas), y desde aquí se puede abrir el código en el editor integrado.

## 4. Filosofía

- Todo bajo reglas claras (nada mágico sin control).
- Organización primero, visual después.
- Xavos usa lo que yo domino:
  - si no domino una herramienta, no se fuerza.
- El programa se construye por fases, sin prisa pero sin romper calidad.