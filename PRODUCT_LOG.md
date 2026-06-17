# PRODUCT_LOG.md — Bitácora de Proyecto: Red3Conecta

## Sprint 1 — ✅ Completado (Jun 01–07)
- ✅ #12 Layout + Base CSS
- ✅ #13 Navbar
- ✅ #14 Footer (Cintia)
- ✅ Estabilización de entorno (Astro v6.4.2, TypeScript, CSS puro)

## Sprint 2 - Actualización de Navegación y Merge (Jun 17, 2026)
* **Refactor**: Reestructuración del componente `Navbar.astro` (división lógica mediante `navbar__right-group`).
* **Corrección**: Resuelto error de sintaxis CSS en `.navbar__title` tras conflicto de fusión en rama `styles-changes`.
* **UX/UI**: Unificado selector de idiomas (`CA | ES`) fuera del flujo del menú hamburguesa para persistencia de estado.
* **Layout**: Ajustada distribución de espacio mediante Flexbox en escritorio y móvil, optimizando la alineación del menú en una línea.
* **Integración**: Merge completado de `landing-page` a `styles-changes` tras resolución de conflictos.

## Sprint 3 En Curso (Jun 15-22)
- ☑ #18 Migración i18n (ES/CA) — 100% funcional.
- ☑ #31 Mejoras de Estilos — Variables CSS :root + transiciones.
- ☑ #13 Navbar — Refactorizado (estilo 3D, responsive, accesibilidad).
- 🔍 #32 QA Central (En revisión en rama `stable-backup`).
- ⏳ #27 Deploy Netlify (Pendiente).

---
*Rama de trabajo actual: styles-changes*
*Hash del último commit: [ae8f219]*
*QA-IA: Validado mediante tsc --noEmit y build estático.*