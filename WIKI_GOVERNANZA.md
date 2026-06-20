# 🏛️ Guía de Gobernanza: Red3Conecta

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
| **Ana Belén** | Layout, Navbar, Hero, QA (#32), Deploy (#27) | 1-3 | ✅/🔍 |
| **Cintia** | About, Footer, Mejoras estilos #31 | 1-3 | ✅ |
| **Paula** | Sec. 4, 5, 6, Marca #26, Mejoras estilos #31 | 2-3 | ✅/⏳ |
| **Jessica** | Sec. 7, 8, 9, Mejoras estilos #31 | 2-3 | ✅ |

---

## 3. Estado Actual (Rama `styles-changes`)

### ✅ Completado
* **Sistema i18n bilingüe** (ES/CA) funcional.
* **Componente Navbar (#13)**: Refactorizado con estructura Flexbox robusta, selector de idiomas independiente y layout optimizado.
* **Mejoras de estilos #31**: Variables CSS, transiciones 3D en botones y animaciones *shimmer*.
* **QA Central (#32)**: Ejecución en rama `stable-backup`.
* **Merge final**: Integración de `styles-changes` -> `landing-page`.
* **Deploy Netlify (#27)**: Pendiente de validación QA.

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
- [x] Estructura DOM Navbar: Layout corregido (Logo - Menú - GrupoDerecho) ✅
- [x] Responsive: Alineación derecha en móvil (lang/toggle) ✅
- [x] WCAG AA: Navegación teclado y estados `:hover/:focus` ✅
- [x] Estados interactivos implementados ✅

---

*Última actualización: 17/06/2026 | Ana Belén (Scrum Master)*
*Status Sprint 3: DESARROLLO ESTILOS EN styles-changes*