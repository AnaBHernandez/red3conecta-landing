# 🏛️ Guía de Trabajo: Red3Conecta

## 1. Reglas de Oro (Líneas Rojas)
1. **CSS Puro:** Prohibido Tailwind, Bootstrap o Sass. Todo mediante CSS nativo + variables `:root`.
2. **Cero Hardcoded:** Todo texto en `src/i18n/ca.json` y `src/i18n/es.json`.
3. **Estructura:** Cada componente en su archivo `.astro` propio dentro de `src/components/`.
4. **i18n:** Importar obligatoriamente: `import t from "../i18n/ca.json";` y `import es from "../i18n/es.json";`.
5. **WCAG AA:** Cumplimiento estricto (contraste 4.5:1, aria-label, navegación teclado).
6. **Git:** Prohibido push directo a `main`. Usar rama `landing-page` siempre.

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
landing-page (compartida)

↓ [cada uno hace push]

↓ [Ana revisa + mergea]

dev (actualizada)

↓ [merge final Ana]

main (protegida, despliegue)

**Workflow Compañeras:**
```bash
git checkout landing-page
git pull origin landing-page
# [edita tu componente]
npm run build && npm run dev
git add .
git commit -m "feat: descripción"
git push origin landing-page
# FIN — Ana hace el merge
```

---

## 4. Estándares de Código
**HTML:** Semántico (`<section>`, `<article>`, `<nav>`, `<footer>`)  
**CSS:** Variables `:root`, mobile-first, Flexbox/Grid nativos  
**i18n:** Dinámico `{t.seccion.clave}` en componentes  

---

## 5. Checklist de Entrega (DoD)
- [ ] `npm run build` sin errores
- [ ] `npm run dev` renderiza en localhost:4321
- [ ] Responsive: ≤375px, tablet, desktop
- [ ] WCAG AA: Contraste + navegación teclado
- [ ] 100% textos en ca.json y es.json (bilingüe)
- [ ] CSS Puro sin frameworks
- [ ] Estados: :hover, :focus, :active, :visited

---

## 6. Proceso de Review (Ana)
1. **Pull** desde landing-page
2. **Validación:** npm run build + npm run dev
3. **Auditoría:** HTML semántico, i18n bilingüe, CSS puro
4. **Merge** a dev si está OK
5. **Registro** en GitHub Projects

---

*Última actualización: 13/06/2026 | Ana Belén (Scrum Master)*