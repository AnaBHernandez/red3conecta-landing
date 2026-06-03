# 🌿 Wiki de Gobernanza - Red3Conecta Landing Page

Este documento actúa como la fuente única de verdad para el desarrollo, estándares de código y políticas de integración del equipo.

## 👥 Equipo y Matriz de Roles Híbrida (Multi-IA)
- **Ana Belén (Scrum Master):** Facilitadora, controladora del flujo de Git y propietaria de las decisiones lógicas.
- **Paula (Gestora de Proyecto):** Coordinación general, diseño conceptual y plazos de entrega.
- **Cynthia & Jessica (Desarrolladoras Frontend):** Maquetación semántica y CSS puro.
- **Gemini (Nube):** Arquitecto Senior y Mentor (Validación de lógica, Specs y Red Teaming).
- **Claude (Nube):** Especialista en Refactorización Avanzada y Accesibilidad (WCAG AA).
- **Ollama (Local en VS Code):** Ejecutor atómico (Generación de código repetitivo, autocompletado y ahorro de tokens).

## 🛑 Líneas Rojas del Desarrollo
1. **Protección de Ramas:** Queda prohibido hacer push directo a `main`. Todo el trabajo de Sprints se integra en `dev`.
2. **CSS Puro Obligatorio:** Prohibido el uso de Tailwind, Bootstrap o Sass. Todo el diseño se estructura con CSS nativo usando variables globales en `:root` dentro de `src/styles/global.css`.
3. **Estrategia i18n Unilingüe:** Por decisión unánime del equipo (validada por el correo de Jesús Rivera), la landing se maquetará exclusivamente en **Catalán**. No se escribirán textos fijos (`hardcoded`) en el chasis; todos se consumirán desde `src/i18n/ca.json`.
4. **Layouts de Astro:** Siguiendo las directrices del Notion de Paula, al ser una landing page informativa de sección única (SPA), se prescinde de la carpeta `layouts/`. El archivo `src/pages/index.astro` actúa como el chasis HTML5 directo.

## 📋 Estándares de Trazabilidad y Documentación Técnica

Para mantener el repositorio limpio y garantizar que cualquier desarrolladora nueva entienda el histórico del proyecto, aplicamos un sistema de tres capas:

1. **`spec.md` (El Plano Presente):** - Define el contrato técnico exclusivo de la tarea del micro-paso actual (máx. 10 líneas).
   - Es efímero: solo vive en la rama de integración activa `dev` y se sobreescribe al terminar la funcionalidad. No acumula pasado.
2. **`Git Log` (El Pasado Técnico):**
   - Registra de forma automatizada los cambios exactos de código mediante comandos de terminal de Ubuntu. 
   - Se exige el uso de la convención de mensajes claros antes de realizar cualquier integración en `dev`.
3. **`PRODUCT_LOG.md` (La Bitácora Comercial):**
   - Registra de forma acumulativa los hitos completados (Problema, MVP y validación de QA).
   - Se exige su actualización obligatoria al finalizar cada funcionalidad para control de la Scrum Master y TPO.

   ## 📋 Política de Trazabilidad y Gestión de Documentos

El equipo aplica una separación estricta de responsabilidades para la documentación técnica y el progreso del producto:

1. **`spec.md` (El Plano Presente):**
   - Es un contrato técnico de corta duración (máximo 10 líneas) para guiar la tarea actual.
   - Es efímero: solo vive en la rama de integración activa `dev` y se sobreescribe o elimina al terminar la funcionalidad para no acumular basura. No guarda histórico.
2. **`Git Log` (El Pasado Técnico):**
   - Es el registro automático del código. No escribimos a mano qué archivos cambiaron; delegamos esta tarea en Git mediante mensajes de commit claros y estructurados en la terminal de Ubuntu.
3. **`PRODUCT_LOG.md` (La Bitácora Comercial):**
   - Es el diario acumulativo que recoge los hitos del proyecto (Problema, MVP entregado y validación de QA) para que la Gestora de Proyecto y los stakeholders entiendan la evolución del negocio sin leer código.