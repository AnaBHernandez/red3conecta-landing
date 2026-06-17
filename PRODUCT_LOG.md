# PRODUCT_LOG.md — Bitácora de Proyecto: Red3Conecta

## Sprint 1 — ✅ Completado (Jun 01–07)
- ✅ #12 Layout + Base CSS
- ✅ #13 Navbar
- ✅ #14 Footer (Cintia)
- ✅ Estabilización de entorno (Astro v6.4.2, TypeScript, CSS puro)

## Sprint 2 — ✅ Completado (Jun 08–14)
- ✅ #19 Hero (Ana Belén)
- ✅ #20 About (Cintia)
- ✅ #21 Sectionfive — Ally (Paula)
- ✅ #22 Sectionfour — Challenges (Paula)
- ✅ #29 Sectionsix — Impact (Paula)
- ✅ #24 Sectioneight — Ecosystem (Jessica)
- ✅ #25 Sectionseven — Partners (Jessica)
- ✅ #30 Sectionnine — Awards (Jessica)
- ✅ Correcciones de accesibilidad (WCAG AA)

## Sprint 3 — 🔄 En Curso (Jun 15–22)
- ✅ #18 Migración i18n (ca.json + es.json) — 100% funcional
- ✅ #31 Mejoras de Estilos — Variables CSS :root + transiciones
- ✅ #27 Git Merges + Deploy Netlify
- ✅ #32 Estrategia de Calidad: QA, Accesibilidad y WCAG AA
- ⏳ #26 Gestión de Recursos de Marca (Paula — en revisión)
- 🔜 #33 Responsive: Media Queries por componente (Equipo — breakpoints a consensuar en daily)
- 🔜 #34 Fix: Overflow horizontal global en global.css (Ana Belén)
- 🔜 #35 Fix: footer__glow overflow en Footer.astro (Cintia)
- 🔜 #36 Fix: carousel-track overflow en Sectionnine.astro (Jessica)

---

## Decisiones Técnicas
- Framework: Astro v6.4.2 (corregido de v4 a v6 real)
- Stack: TypeScript nativo + CSS puro (sin Tailwind/Bootstrap/Sass)
- i18n: ca.json + es.json (sin hardcode en componentes)
- Rama activa: `landing-page` · Rama sagrada: `main`
- Merges: responsabilidad de Ana Belén (Scrum Master)
- Bugs detectados: overflow horizontal causado por `.carousel-track` (2576px) y `.footer__glow` (800px)

---

*Astro versión confirmada: 6.4.2*
*QA validado: tsc --noEmit + npm run build sin errores*
*Última actualización: Junio 2026 — Ana Belén Hernández (Scrum Master)*