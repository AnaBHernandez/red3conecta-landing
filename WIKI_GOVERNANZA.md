# 🏛️ Guía de Trabajo: Red3Conecta

## 1. Reglas de Oro (Líneas Rojas) — IMPLEMENTADAS
* **CSS Puro:** ✅ Prohibido Tailwind/Bootstrap/Sass. Todo mediante CSS nativo + variables `:root`.
* **Cero Hardcoded:** ✅ Todo texto en `ca.json` y `es.json`. Sistema bilingüe funcional.
* **Estructura:** ✅ Cada componente en archivo `.astro` propio en `src/components/`.
* **i18n:** ✅ Importación: `import t from "../i18n/ca.json";` (y es.json).
* **WCAG AA:** ✅ Cumplimiento estricto. *Nota: Navbar mantiene fondo oscuro (identidad visual); contraste verificado para cumplir ratio AA*.
* **Git:** ✅ Prohibido push directo a `main`. Usar ramas `landing-page` y `styles-changes`.

---

## 2. Equipo y Asignaciones (Sprint 3 Actual)
| Responsable | Componentes | Sprint | Estado |
|---|---|---|---|
| **Ana Belén** (Scrum Master) | Layout, Navbar, Hero, QA (#32), Deploy (#27) | 1-3 | ✅/🔍 |
| **Cintia** | About, Footer, Mejoras estilos #31 | 1-3 | ✅ |
| **Paula** | Sec. 4, 5, 6, Marca #26, Mejoras estilos #31 | 2-3 | ✅/⏳ |
| **Jessica** | Sec. 7, 8, 9, Mejoras estilos #31 | 2-3 | ✅ |

---

## 3. Estado Actual (Rama `styles-changes`)

### ✅ Completado
* Sistema i18n bilingüe (ES/CA) funcional.
* Mejoras de estilos #31 aplicadas (Variables CSS, transiciones, Navbar 3D).
* Componente Navbar (#13) validado.

### ⏳ Pendiente
* Revisión del equipo en rama `styles-changes`.
* Merge a `landing-page`.
* Deploy en Netlify (#27).
* QA final (#32).

---

## 4. Git Flow (Rama Compartida)
`styles-changes` (revisión actual)

↓ [después de aprobación]

`landing-page` (compartida)

↓ [Ana mergea]

`dev` (integración)

↓ [Ana mergea]

`main` (producción)

---

## 5. Checklist de Entrega (DoD)
- [x] `npm run build` sin errores ✅
- [x] `npm run dev` renderiza en localhost:4321 ✅
- [x] Responsive: ≤375px, tablet, desktop ✅
- [x] WCAG AA: Contraste + navegación teclado ✅
- [x] Estados interactivos implementados (:hover, :focus, :active, :visited) ✅

---

*Última actualización: 17/06/2026 | Ana Belén (Scrum Master)*
*Status Sprint 3: DESARROLLO ESTILOS EN styles-changes*