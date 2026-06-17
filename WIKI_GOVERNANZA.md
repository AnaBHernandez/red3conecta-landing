# 🏛️ Guía de Gobernanza: Red3Conecta

## 1. Reglas de Oro (Líneas Rojas)
1. **CSS Puro:** Prohibido Tailwind/Bootstrap/Sass. Todo mediante CSS nativo + variables `:root`.
2. **Cero Hardcoded:** Todo texto en `ca.json` y `es.json`. Sistema bilingüe funcional.
3. **Estructura:** Cada componente en archivo `.astro` propio en `src/components/`.
4. **i18n:** Importación: `import t from "../i18n/ca.json";` (y es.json si aplica).
5. **WCAG AA:** Cumplimiento estricto (contraste 4.5:1, aria-label, navegación teclado).
6. **Git:** Prohibido push directo a `main`. Rama activa: `landing-page`.

---

## 2. Equipo y Asignaciones
| Responsable | Componentes | Estado |
|---|---|---|
| **Ana Belén** (Scrum Master) | Layout, Navbar, Hero, global.css, QA, Deploy, Merges | ✅ / 🔜 |
| **Cintia** | About, Footer | ✅ / 🔜 |
| **Paula** | Sectionfour, Sectionfive, Sectionsix, Recursos de Marca | ✅ / ⏳ |
| **Jessica** | Sectionseven, Sectioneight, Sectionnine | ✅ / 🔜 |

---

## 3. Stack Técnico Confirmado
- **Framework:** Astro v6.4.2
- **Lenguaje:** TypeScript nativo
- **Estilos:** CSS puro (sin Tailwind/Bootstrap/Sass)
- **i18n:** ca.json + es.json (sin hardcode en componentes)
- **Fuentes:** Cantarell + PT Sans (Google Fonts)
- **Gestor de paquetes:** npm
- **Comando dev:** `npm run dev` → localhost:4321

---

## 4. Git Flow
```
landing-page (rama activa de trabajo)
     ↓ [Ana Belén mergea tras revisión]
main (producción — intocable)
```
- Commits en `landing-page` únicamente
- Conventional commits: `feat:` `fix:` `style:` `docs:` `chore:`
- PR a Ana Belén antes de cualquier merge

---

## 5. Estado Sprint 3 (Jun 15–22)
| ID | Tarea | Asignado | Estado |
|---|---|---|---|
| #18 | Migración i18n (ca.json + es.json) | Equipo | ✅ HECHO |
| #31 | Mejoras de Estilos Dinámicos | Equipo | ✅ HECHO |
| #27 | Git Merges + Deploy Netlify | Ana Belén | ✅ HECHO |
| #32 | QA, Accesibilidad y WCAG AA | Ana Belén | ✅ HECHO |
| #26 | Gestión de Recursos de Marca | Paula | ⏳ REVISIÓN |
| #33 | Responsive: Media Queries por componente | Equipo | 🔜 TODO |
| #34 | Fix: Overflow horizontal en global.css | Ana Belén | 🔜 TODO |
| #35 | Fix: footer__glow en Footer.astro | Cintia | 🔜 TODO |
| #36 | Fix: carousel-track en Sectionnine.astro | Jessica | 🔜 TODO |

---

## 6. Bugs Detectados en QA Móvil
| Bug | Causa | Archivo | Responsable |
|---|---|---|---|
| Scroll horizontal | `.carousel-track` 2576px | Sectionnine.astro | Jessica (#36) |
| Scroll horizontal | `.footer__glow` 800px | Footer.astro | Cintia (#35) |
| Overflow global | Sin `overflow-x: hidden` en html/body | global.css | Ana Belén (#34) |

---

## 7. Breakpoints Responsive
⚠️ A consensuar en daily antes de iniciar tarea #33.  
Propuesta para validar en equipo:
- Móvil base: ≤375px (sin media query — estilos por defecto)
- Tablet: `min-width: 768px`
- Desktop: `min-width: 1024px`
- Desktop XL: `min-width: 1280px`

---

## 8. Checklist DoD (Definition of Done)
- [ ] Móvil ≤375px sin scroll horizontal
- [ ] Tablet 768px funciona
- [ ] Desktop 1024px funciona
- [ ] WCAG AA: contraste 4.5:1 + navegación teclado
- [ ] 100% textos en ca.json y es.json
- [ ] CSS puro sin frameworks
- [ ] Estados :hover :focus :visited :active explícitos
- [ ] `npm run build` sin errores
- [ ] PR enviada a Ana Belén para merge

---

*Última actualización: 17/06/2026 | Ana Belén Hernández (Scrum Master)*
*Astro v6.4.2 confirmado · Deploy activo en Netlify*