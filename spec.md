# 📝 Especificación de Componentes: Red3Conecta

---

## 🔵 PLANTILLA — Para Nuevos Componentes

**Componente:** [Nombre]  
**Ruta:** `src/components/[nombre].astro`  
**Asignado a:** [Nombre]  
**Sprint:** [1/2/3]  
**Rama:** `landing-page`

### 📋 Requisitos

**Datos:**
- [ ] 100% textos desde `src/i18n/ca.json`
- [ ] Importar: `import t from "../i18n/ca.json";`
- [ ] Sin hardcoded

**Estilos:**
- [ ] CSS Puro (Flexbox/Grid)
- [ ] Sin Tailwind/Bootstrap/Sass
- [ ] Variables :root para colores/espacios
- [ ] Responsive: ≤375px, 768px, ≥1024px
- [ ] Estados: :hover, :focus, :visited, :active

**Accesibilidad (WCAG AA):**
- [ ] HTML5 semántico
- [ ] Contraste 4.5:1 mínimo
- [ ] aria-label/aria-labelledby en interactivos
- [ ] Navegación teclado funcional
- [ ] Encabezados jerárquicos (h1-h3)

**Build:**
- [ ] `npm run build` sin errores
- [ ] `npm run dev` en localhost:4321
- [ ] Sincronizado con `landing-page`

---

## ✅ COMPONENTES COMPLETADOS

### Sprint 1 (HECHO)

#### Layout + Base CSS (#12)
- Grid principal, variables :root, reset CSS
- Mobile-first, responsive
- Status: ✅ HECHO

#### Navbar.astro (#13)
- Nav semántica, navegación por secciones
- Hamburgesa en móvil
- WCAG AA: teclado + aria-labels
- Status: ✅ HECHO

#### Footer.astro (#14)
- Footer semántico, créditos desde i18n
- Responsive: columnas → stack
- Status: ✅ HECHO

---

### Sprint 2 (HECHO)

#### Hero.astro (#19)
- Sección destacada + CTA
- Imagen responsiva
- Tipografía jerárquica
- Status: ✅ HECHO

#### About.astro (#20)
- Grid 2 col (texto + imagen)
- Badge + 3 párrafos
- Stack en móvil
- Status: ✅ HECHO

#### Sectionfour.astro (#22 — Challenges)
- Grid de tarjetas 3+ columnas
- Iconos/números destacados
- Hover effects
- Status: ✅ HECHO

#### Sectionfive.astro (#21 — Ally)
- Contenido modular
- Flexbox responsivo
- Stack en móvil
- Status: ✅ HECHO

#### Sectionsix.astro (#29 — Impact)
- KPIs cuantitativos
- Números grandes
- Grid responsivo
- Status: ✅ HECHO

#### Sectionseven.astro (#25 — Partners)
- Grid logos institucionales
- object-fit: contain (SVGs)
- Hover + aria-labels
- Status: ✅ HECHO

#### Sectioneight.astro (#24 — Ecosystem)
- Red colaborativa
- Bloques A (Profesionales) + B (Personas)
- Grid responsivo
- Status: ✅ HECHO

#### Sectionnine.astro (#30 — Awards)
- Bloque awards + bloque funders
- Listas semánticas (<dl>)
- Stack en móvil
- Status: ✅ HECHO

---

### Sprint 3 (EN CURSO)

#### #18 Migración i18n (Equipo)
- Extraer textos de componentes Sprint 2
- Agregar a `src/i18n/ca.json`
- 100% sin hardcoded
- Status: ⏳ EN CURSO
- Asignado: Equipo

#### #31 Mejoras de Estilos Dinámicos (Equipo)
- Variables CSS :root mejoradas (colores, espacios, tipografía)
- Transiciones suaves (0.3s ease)
- Animaciones entrada (fade-in, slide)
- Hover/focus states optimizados
- 3+ breakpoints: ≤375px, 768px, ≥1024px
- **Cintia:** About + Footer
- **Paula:** Section4, 5, 6
- **Jessica:** Section7, 8, 9
- **Ana:** Hero + coordinación
- Status: ⏳ EN CURSO
- Asignado: Equipo

#### #26 Gestión de Recursos de Marca (Paula)
- Assets de marca compilados
- Paleta + tipografía documentadas
- Testing visual cross-browser
- Status: ⏳ POR HACER
- Asignado: Paula

#### #27 Git Merges + Deploy Netlify (Ana)
- Merges landing-page → dev → main
- Netlify conectado
- Build settings: npm run build → dist
- Deploy automático en push a main
- URL en vivo verificada
- Status: ⏳ POR HACER
- Asignado: Ana Belén

#### #32 Estrategia de Calidad: QA, Accesibilidad y WCAG AA (Ana)
- Validación WCAG AA (contraste, teclado, aria-labels)
- Testing responsive (≤375px, 768px, ≥1024px)
- Testing Lighthouse
- Testing cross-browser
- Status: 🔍 EN REVISIÓN
- Asignado: Ana Belén

---

## ✅ Criterios DoD (Todos los Componentes)

- [ ] Responsive: ≤375px (móvil), 768px (tablet), ≥1024px (desktop)
- [ ] WCAG AA: Contraste 4.5:1, navegación teclado, aria-labels
- [ ] i18n: 100% desde ca.json, sin hardcoded
- [ ] CSS Puro: Flexbox/Grid, sin frameworks
- [ ] HTML5 semántico: <section>, <article>, <nav>, etc.
- [ ] npm run build sin errores
- [ ] npm run dev funciona en localhost:4321
- [ ] Estados: :hover, :focus, :visited, :active
- [ ] Lighthouse 90+ (performance)

---

## 📚 Referencias Rápidas

**i18n:**
```astro
---
import t from "../i18n/ca.json";
---
<h2>{t.seccion.titulo}</h2>
```

**Responsive Mobile-First:**
```css
/* Móvil ≤375px */
.elemento { width: 100%; }

/* Tablet 768px */
@media (min-width: 768px) { .elemento { width: 50%; } }

/* Desktop ≥1024px */
@media (min-width: 1024px) { .elemento { width: 33.33%; } }
```

**WCAG AA:**
- Contraste mínimo: 4.5:1
- aria-label en iconos/botones
- Navegación teclado: Tab, Enter, Escape
- Encabezados claros: h1 → h2 → h3

---

*Última actualización: 10/06/2026 | Ana Belén (Scrum Master)*