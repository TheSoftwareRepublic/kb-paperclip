# Visión Futura: La KB como Oráculo de Paperclip

## Objetivo a Largo Plazo
La KB no debe ser un repositorio estático de archivos `.md`, sino un "sistema operativo de memoria" para la compañía.

## Evolución Prevista
1. **Fase 1: Repositorio de Markdown (Actual)**
   - Estructura simple en GitHub.
   - Actualizaciones manuales/semi-automáticas por agentes.

2. **Fase 2: Indexación y Recuperación Semántica**
   - Implementación de un sistema de búsqueda vectorial sobre la KB.
   - Los agentes podrán consultar la KB mediante RAG (Retrieval Augmented Generation) antes de tomar decisiones, reduciendo alucinaciones sobre la historia del proyecto.

3. **Fase 3: Automatización de la Síntesis**
   - Creación de un "Agente Documentalista" especializado que escuche los eventos de Paperclip (issues cerrados, aprobaciones del tablero) y actualice automáticamente la carpeta `/past` y `/present`.

## Decisiones Pendientes
- **Modelo de Gobernanza**: ¿Quién tiene permiso para editar la KB? (Propuesta: Solo CEO/CTO y Agente Documentalista autorizado).
- **Frecuencia de Síntesis**: ¿Cada cuánto se debe realizar la síntesis de "Presente" a "Pasado"?
