# Arquitectura de la Base de Conocimientos (KB) Paperclip

Esta KB tiene como objetivo capturar la memoria total de la compañía, transformando el flujo de trabajo en un activo documental estructurado.

## Estructura de Directorios

### 1. `/past` (El Pasado)
**Propósito:** Registro histórico y síntesis de lo logrado.
- **Contenido:** Documentos de cierre de hitos, resúmenes de issues completados, decisiones arquitectónicas ya implementadas.
- **Formato:** `YYYY-MM-DD_nombre-del-hito.md`

### 2. `/present` (El Presente)
**Propósito:** Captura en tiempo real de la operación.
- **Contenido:** Estado de los issues `in_progress`, actas de decisiones actuales, logs de razonamiento del CEO/CTO sobre problemas activos.
- **Formato:** `issue-ID_estado-actual.md`

### 3. `/future` (El Futuro)
**Propósito:** Planificación y visión.
- **Contenido:** Roadmap, backlog estratégico, hipótesis a validar, decisiones pendientes de definición.
- **Formato:** `vision_nombre-del-modulo.md` o `decision-pendiente_ID.md`

### 4. `/meta` (Metadatos y Gobernanza)
**Propósito:** Reglas del sistema.
- **Contenido:** Esta guía de arquitectura, índice general (`INDEX.md`), glosario de términos.

## Flujo de Sincronización
Toda la información sintetizada en el flujo de trabajo de Paperclip debe terminar reflejada aquí. El agente Documentalista es el responsable de mover la información de `/present` $\rightarrow$ `/past` una vez que el issue asociado pase a estado `done`.
