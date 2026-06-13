# 🏛️ Guía de Trabajo: Red3Conecta

## 1. Reglas de Oro (Líneas Rojas)
1. **CSS Puro:** Prohibido Tailwind, Bootstrap o Sass. Todo el diseño debe gestionarse mediante archivos `.css` nativos y variables `:root`.
2. **Cero Hardcoded:** Todo texto visible debe residir en `src/i18n/ca.json`.
3. **Estructura:** Cada componente debe residir en su propio archivo `.astro` dentro de `src/components/`.
4. **i18n:** Es obligatorio importar el diccionario en cada componente: `import t from "../i18n/ca.json";`.
5. **WCAG AA:** Cumplimiento estricto de accesibilidad (contraste 4.5:1, etiquetas `aria-label` en elementos interactivos).

---

## 2. Equipo y Asignaciones
| Responsable | Componentes | Sprint |
|---|---|---|
| **Ana Belén** (Scrum Master) | Layout, Navbar, Hero, QA (#32), Deploy (#27) | 1-3 |
| **Cintia** | About, Footer, Mejoras estilos #31 | 1-3 |
| **Paula** | Sec. 4, 5, 6, Marca #26, Mejoras estilos #31 | 2-3 |
| **Jessica** | Sec. 7, 8, 9, Mejoras estilos #31 | 2-3 |

---

## 3. Git Flow (Rama Compartida)
* **Rama de trabajo:** `landing-page` (compartida por todo el equipo).
* **Flujo:** `landing-page` → [Merge Ana] → `dev` → `main` (Despliegue).
* **Política:** Queda prohibido hacer push directo a `main`. Tras el merge final a `main` y la verificación de deploy, la rama `landing-page` será archivada al finalizar el Sprint 3.

---

## 4. Estándares de Código
* **HTML:** Semántico (uso correcto de `<section>`, `<article>`, `<nav>`, `<footer>`).
* **CSS:** Uso de variables `:root` para colores y espacios. Diseño *mobile-first*.
* **i18n:** Uso dinámico `{t.seccion.clave}`.

---

## 5. Checklist de Entrega (DoD)
Antes de solicitar un merge a Ana Belén, cada componente debe cumplir:
- [ ] `npm run build` ejecutado sin errores.
- [ ] `npm run dev` renderiza correctamente en localhost:4321.
- [ ] Responsive: Adaptado a ≤375px, tablet y desktop.
- [ ] WCAG AA: Contraste verificado y navegación por teclado operativa.
- [ ] 100% de los textos migrados a `ca.json` (cero hardcoded).
- [ ] CSS Puro (sin Tailwind ni frameworks).
- [ ] Estados de interacción definidos: `:hover`, `:focus`, `:active`.

---

## 6. Proceso de Review
1. **Pull:** Ana realiza `pull` de la rama `landing-page`.
2. **Validación:** Ejecución de `npm run build` y test de renderizado.
3. **Auditoría:** Revisión de HTML semántico, validación de i18n y calidad de CSS.
4. **Merge:** Si el código es conforme, se integra a `dev`.
5. **Registro:** Actualización del estado en GitHub Projects.

---
*Última actualización: 12/06/2026 | Ana Belén (Scrum Master)*