# 🏛️ Guía de Gobernanza: Red3Conecta

## 1. Reglas de Oro (Líneas Rojas) — IMPLEMENTADAS
* **CSS Puro:** Prohibido Tailwind/Bootstrap/Sass. Todo mediante CSS nativo + variables `:root`.✅
* **Cero Hardcoded:** Todo texto en `ca.json` y `es.json`. Sistema bilingüe funcional.✅
* **Estructura:** Cada componente en archivo `.astro` propio en `src/components/`.✅
* **i18n:** Importación: `import t from "../i18n/ca.json";` (y es.json).✅
* **WCAG AA:** Cumplimiento estricto. *Nota: Navbar mantiene fondo oscuro (identidad visual); contraste verificado para cumplir ratio AA*.✅
* **Git:** Prohibido push directo a `main`. Usar ramas `landing-page` y `styles-changes`.✅

---

## 2. Equipo y Asignaciones (Sprint 3 Actual)
| Responsable | Componentes | Sprint | Estado |
|---|---|---|---|
| **Ana Belén** | Layout, Navbar, Hero, QA (#32), Deploy (#27) | 1-3 | ✅ |
| **Cintia** | About, Footer, Mejoras estilos #31 | 1-3 | ✅ |
| **Paula** | Sec. 4, 5, 6, Marca #26, Mejoras estilos #31 | 2-3 | ✅ |
| **Jessica** | Sec. 7, 8, 9, Mejoras estilos #31 | 2-3 | ✅ |

---

## 3. Estado Actual (Rama `dev`)

* **Sistema i18n bilingüe** (ES/CA) funcional.✅
* **Componente Navbar (#13)**: Refactorizado con Flexbox, selector de idiomas y layout optimizado.✅
* **Mejoras de estilos #31**: Variables CSS, transiciones 3D y animaciones.✅
* **QA Central (#32)**: Finalizado.✅
* **Merge final**: Integración de `landing-page` -> `dev`.✅
* **Deploy Vercel (#27)**: Despliegue en producción activo.✅

---

## 4. Git Flow
`landing-page` (trabajo diario) 
→ `dev` (integración continua) 
→ `main` (producción Vercel)

---


## 5. Checklist de Entrega (DoD)
* ** Build & Deploy: npm run build sin errores y despliegue validado en Vercel.✅
* ** i18n: Textos 100% extraídos en ca.json y es.json. Cero hardcoded strings.✅
* ** Layout & DOM: Estructura Navbar (Logo - Menú - GrupoDerecho) validada.✅
* ** Responsive: Alineación derecha en móvil (lang/toggle) y corrección de overflows (Tasks #34-36).✅
* ** [x] Accesibilidad (WCAG AA): Navegación por teclado, estados :hover/:focus y contraste verificado (4.5:1).✅
* ** [x] Integridad: PRODUCT_LOG.md y README.md sincronizados con el estado real del Board.✅


---

*Última actualización: 18/06/2026 | Ana Belén (Scrum Master)*