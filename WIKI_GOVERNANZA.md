# 🏛️ Guía de Trabajo: Red3Conecta

## 1. Reglas de Oro (Líneas Rojas) — IMPLEMENTADAS
1. **CSS Puro:** ✅ Prohibido Tailwind/Bootstrap/Sass. Todo mediante CSS nativo + variables `:root`.
2. **Cero Hardcoded:** ✅ Todo texto en `ca.json` y `es.json`. Sistema bilingüe funcional.
3. **Estructura:** ✅ Cada componente en archivo `.astro` propio en `src/components/`.
4. **i18n:** ✅ Importación: `import t from "../i18n/ca.json";` (y es.json si aplica).
5. **WCAG AA:** ✅ Cumplimiento estricto (contraste 4.5:1, aria-label, navegación teclado).
6. **Git:** ✅ Prohibido push directo a `main`. Usar rama `landing-page`.

---

## 2. Equipo y Asignaciones (Sprint 3 Actual)
| Responsable | Componentes | Sprint | Estado |
|---|---|---|---|
| **Ana Belén** (Scrum Master) | Layout, Navbar, Hero, QA (#32), Deploy (#27) | 1-3 | ✅/🔍 |
| **Cintia** | About, Footer, Mejoras estilos #31 | 1-3 | ✅ |
| **Paula** | Sec. 4, 5, 6, Marca #26, Mejoras estilos #31 | 2-3 | ✅/⏳ |
| **Jessica** | Sec. 7, 8, 9, Mejoras estilos #31 | 2-3 | ✅ |

---

## 3. Estado Actual (Rama stable-backup)

### ✅ Completado
- Sistema i18n bilingüe (ES/CA) funcional
- Todas las mejoras de estilos aplicadas
- Variables CSS globales en :root
- Transiciones 0.3s en interactivos
- Correcciones de layouts
- Arreglos de errores runtime
- Build: ✅ 4 páginas sin errores

### ⏳ Pendiente
- Revisión del equipo en stable-backup
- Merge a landing-page
- Deploy en Netlify (#27)
- QA final (#32)

---

## 4. Git Flow (Rama Compartida)
stable-backup (revisión actual)

↓ [después de aprobación]

landing-page (compartida)

↓ [Ana mergea]

dev (integración)

↓ [Ana mergea]

main (producción)

---

## 5. Estándares de Código — APLICADOS
**HTML:** ✅ Semántico (`<section>`, `<article>`, `<nav>`, `<footer>`)
**CSS:** ✅ Variables `:root`, mobile-first, Flexbox/Grid nativos
**i18n:** ✅ Dinámico `{t.seccion.clave}` en 100% de componentes
**Accesibilidad:** ✅ WCAG AA + navegación teclado
**Responsividad:** ✅ ≤375px, tablet (768px), desktop (≥1024px)

---

## 6. Checklist de Entrega (DoD) — CUMPLIDO
- [x] `npm run build` sin errores ✅
- [x] `npm run dev` renderiza en localhost:4321 ✅
- [x] Responsive: ≤375px, tablet, desktop ✅
- [x] WCAG AA: Contraste + navegación teclado ✅
- [x] 100% textos en ca.json y es.json ✅
- [x] CSS Puro sin frameworks ✅
- [x] Estados: :hover, :focus, :active, :visited ✅
- [x] Variables CSS globales aplicadas ✅

---

## 7. Proceso de Review — FASE ACTUAL
1. **Equipo revisa** rama `stable-backup`
2. **Feedback** a Ana Belén
3. **Merge** a `landing-page` (si aprobado)
4. **Integración** a `dev`
5. **Deploy** a Netlify

---

## 📌 Próximos Pasos (Backlog)
- [ ] Revisión equipo en stable-backup
- [ ] Merge a landing-page
- [ ] Deploy a Netlify
- [ ] Test final con lector de pantalla (NVDA/VoiceOver)
- [ ] Scroll Reveal animations (post-MVP)

---

*Última actualización: 13/06/2026 | Ana Belén (Scrum Master)*
*Status Sprint 3: IMPLEMENTACIÓN COMPLETA EN stable-backup*