# 🏛️ Guía de Trabajo: Red3Conecta

## 1. Reglas de Oro
1. **CSS Puro:** Prohibido Tailwind/Bootstrap/Sass.
2. **Sin Hardcoded:** 100% textos en `src/i18n/ca.json`.
3. **Componentes:** Cada uno en archivo `.astro` propio en `src/components/`.
4. **i18n:** Siempre importar `import t from "../i18n/ca.json";`
5. **WCAG AA:** Contraste 4.5:1 mínimo, aria-label en interactivos.

---

## 2. Equipo y Asignaciones

| Responsable | Componentes | Sprint |
|---|---|---|
| **Ana Belén** (Scrum Master) | Layout, Navbar, Hero, QA, Deploy | 1-3 |
| **Cintia** | About, Footer, Mejoras estilos #31 | 1-3 |
| **Paula** | Sectionfour (Challenges), Sectionfive (Ally), Sectionsix (Impact), Marca #26, Mejoras estilos #31 | 2-3 |
| **Jessica** | Sectionseven (Partners), Sectioneight (Ecosystem), Sectionnine (Awards), Mejoras estilos #31 | 2-3 |

---

## 3. Git Flow (Rama Compartida)

landing-page (compartida)
↓ [push cada uno su trabajo]
↓ [Ana revisa + mergea]
dev (actualizada)
↓ [merge final Ana]
main (protegida, deploy)

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

**Workflow Ana (Merge):**
```bash
git checkout landing-page && git pull
npm run build && npm run dev
# [revisa código y tests]
git checkout dev && git merge landing-page && git push origin dev
# [después de QA]
git checkout main && git merge dev && git push origin main
```

---

## 4. Estándares de Código

### HTML
- Semántico: `<section>`, `<article>`, `<nav>`, `<footer>`
- Accesibilidad: `aria-label`, `aria-labelledby`, roles claros
- Sin divitis innecesarios

### CSS
- Variables :root para colores, espacios, tipografía
- Mobile-first (media queries mínimas)
- Flexbox/Grid nativos
- Sin !important

### i18n
1. Identifica textos en tu componente
2. Agrégalos a `src/i18n/ca.json` con estructura clara
3. Importa: `import t from "../i18n/ca.json";`
4. Usa: `{t.seccion.clave}`

**Ejemplo:**
```astro
---
import t from "../i18n/ca.json";
---
<h2>{t.about.title}</h2>
```

---

## 5. Checklist por Componente

Antes de mergear:

- [ ] `npm run build` sin errores
- [ ] `npm run dev` renderiza bien en localhost:4321
- [ ] Responsive: móvil ≤375px, tablet, desktop
- [ ] WCAG AA: contraste, navegación teclado, aria-labels
- [ ] 100% textos en ca.json (sin hardcoded)
- [ ] CSS Puro (sin Tailwind)
- [ ] Archivo único `.astro` en `src/components/`
- [ ] Estados: :hover, :focus, :visited, :active

---

## 6. Proceso de Review (Ana)

1. **Pull desde landing-page**
2. **npm run build** — compila sin errores
3. **npm run dev** — visualiza en localhost
4. **Revisa código:**
   - HTML semántico
   - CSS puro
   - i18n correcto
   - Sin hardcoded
5. **Merge a dev** si está OK
6. **Documente en GitHub Projects**

---

## 7. Rama landing-page

- **Propósito:** Rama compartida para Sprint 1-3
- **Protección:** Solo Ana puede mergear a dev
- **Política:** No se borra hasta final
- **Sincronización:** Diaria con origin

---

*Última actualización: 10/06/2026 | Ana Belén (Scrum Master)*

spec.md
markdown# 📋 Especificación de Componentes: Red3Conecta

## Status Actual
- **Sprint 1-2:** ✅ COMPLETADO
- **Sprint 3:** ⏳ EN CURSO (Mejoras + Deploy)

---

## Sprint 1 ✅

### Layout + Base CSS (#12)
- Grid principal 12 columnas
- Variables CSS :root (colores, espacios, tipografía)
- Reset CSS normalizado
- Mobile-first responsivo
- **Status:** HECHO

### Navbar.astro (#13)
- Navegación semántica con `<nav>`
- Links a secciones con `id` anclas
- Responsive: hamburgesa en móvil
- WCAG AA: navegación teclado
- **Status:** HECHO

### Footer.astro (#14)
- `<footer>` semántico
- Créditos institucionales desde i18n
- Links de navegación secundaria
- Responsive: columnas → stack
- **Status:** HECHO

---

## Sprint 2 ✅

### Hero.astro (#19)
- Sección destacada con CTA
- Imagen responsiva (srcset)
- Tipografía jerárquica (h1)
- Gradiente o color sólido
- **Status:** HECHO

### About.astro (#20)
- Grid 2 columnas (texto + imagen)
- Badge de categoría
- 3 párrafos explicativos
- Responsive: stack en móvil
- **Status:** HECHO

### Sectionfour.astro (#22 / Challenges)
- Grid de tarjetas (3+ columnas)
- Iconos o números destacados
- Textos desde ca.json
- Hover effects suaves
- **Status:** HECHO

### Sectionfive.astro (#21 / Ally)
- Estructura modular de contenido
- Títulos y descripciones
- Layout flexible Flexbox
- Responsive apilado
- **Status:** HECHO

### Sectionsix.astro (#29 / Impact)
- KPIs cuantitativos destacados
- Números grandes + etiquetas
- Grid de estadísticas
- Responsive: stack en móvil
- **Status:** HECHO

### Sectionseven.astro (#25 / Partners)
- Grid de logos institucionales
- `object-fit: contain` para SVGs
- Hover con cambio de escala
- WCAG AA: aria-label en cada logo
- **Status:** HECHO

### Sectioneight.astro (#24 / Ecosystem)
- Red colaborativa descrita
- Bloques A (Profesionales) y B (Personas)
- Grid o Flexbox responsivo
- Textos modulares desde i18n
- **Status:** HECHO

### Sectionnine.astro (/ Awards)
- Bloque de reconocimientos (awards)
- Bloque de financiadores (funders)
- Listas semánticas (`<dl>`, `<dt>`, `<dd>`)
- Responsive: columnas → stack
- **Status:** HECHO

---

## Sprint 3 ⏳

### #26 Gestión de Recursos de Marca (Paula)
- Compilar assets de marca (logos, paleta, tipografía)
- Documentar uso de colores en ca.json
- Verificar calidad visual (contraste, consistencia)
- Testing visual en todos los navegadores
- **Asignado:** Paula
- **Status:** POR HACER

### #28 Mejoras de Estilos Dinámicos (Equipo)
- Variables CSS mejoradas (colores, tamaños, espacios)
- Transiciones suaves (0.3s ease)
- Animaciones de entrada (fade-in, slide)
- Mejoras de hover/focus states
- Responsive: 3+ breakpoints claros
- **Asignado:** Equipo
- **Status:** POR HACER

### #27 Git Merges + Deploy Netlify (Ana)
- Mergear landing-page → dev
- Mergear dev → main
- Conectar repo a Netlify
- Configurar build: `npm run build` → `dist`
- Deploy automático en push a main
- Verificar URL en vivo
- **Asignado:** Ana Belén
- **Status:** POR HACER

---

## Criterios DoD Globales (Todos)

✅ Responsive: ≤375px (móvil), 768px (tablet), ≥1024px (desktop)  
✅ WCAG AA: Contraste 4.5:1, navegación teclado, aria-labels  
✅ i18n: 100% textos desde `ca.json`, sin hardcoded  
✅ CSS Puro: Sin Tailwind/Bootstrap/Sass  
✅ HTML5: Semántico, accesible  
✅ Build: `npm run build` sin errores  
✅ Performance: Lighthouse 90+  

---

*Última actualización: 10/06/2026 | Ana Belén*