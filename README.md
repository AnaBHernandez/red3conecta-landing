# 📊 Red3Conecta - Landing Page (ConnectaDona)

Infraestructura digital compartida construida con el tercer sector, para el tercer sector. Un proyecto impulsado por Factoría F5 y Fundació Formació i Treball, con el soporte de UNADA.

---

## 🛠️ Especificaciones Técnicas

* **Framework:** Astro v6 (SPA, sin `layouts/`).
* **Estilos:** CSS Nativo (`src/styles/global.css`) usando variables `:root`. PROHIBIDO: Tailwind, Bootstrap, Sass.
* **Internacionalización (i18n):** Bilingüe (Català / Castellano). Textos dinámicos en `src/i18n/ca.json` y `src/i18n/es.json`. Cero hardcoded strings.
* **Accesibilidad:** Estándar estricto WCAG AA (ARIA labels, focus visible, contraste 4.5:1).

## 🚀 Cómo empezar

1. **Clonar el repositorio:**
   `git clone https://github.com/AnaBHernandez/red3conecta-landing.git`

2. **Entrar en la carpeta:**
   `cd red3conecta-landing`

3. **Cambiar a la rama de trabajo:**
   `git checkout landing-page`

4. **Instalar todas las librerías necesarias:**
   `npm install`

5. **Ejecutar en modo desarrollo:**
   `npm run dev`

---

## 🌿 Flujo de Trabajo (Git Flow)

1. `main`: Producción (Bloqueado).
2. `dev`: Integración.
3. `landing-page`: Rama compartida de trabajo diario.

---

## 📋 Estado del Proyecto (Sprints)

### Sprint 1 ✅ TERMINADO
| ID | Componente | Estado |
|---|---|---|
| #12 | Layout + Base CSS | ✅ HECHO |
| #13 | Navbar.astro | ✅ HECHO |
| #14 | Footer.astro | ✅ HECHO |

### Sprint 2 ✅ COMPLETADO
| ID | Componente | Estado |
|---|---|---|
| #19 | Hero.astro | ✅ HECHO |
| #20 | About.astro | ✅ HECHO |
| #22 | Sectionfour.astro (Challenges) | ✅ HECHO |
| #21 | Sectionfive.astro (Ally) | ✅ HECHO |
| #29 | Sectionsix.astro (Impact) | ✅ HECHO |
| #24 | Sectioneight.astro (Ecosystem) | ✅ HECHO |
| #25 | Sectionseven.astro (Partners) | ✅ HECHO |
| #30 | Sectionnine.astro (Awards) | ✅ HECHO |

### Sprint 3 ✅ COMPLETADO
| ID | Tarea | Estado |
|---|---|---|
| #18 | Migración i18n (ca.json + es.json) | ✅ HECHO |
| #31 | Mejoras de Estilos Dinámicos | ✅ HECHO |
| #26 | Gestión de Recursos de Marca | ✅ HECHO |
| #27 | Git Merges + Deploy Vercel | ✅ HECHO |
| #32 | Estrategia de Calidad: QA, Accesibilidad y WCAG AA | ✅ HECHO |

---

## 🛡️ Líneas Rojas de Desarrollo

* Prohibido hacer `push` directo a `main`.
* Prohibido incluir comentarios metodológicos en el código visual.
* Obligatorio `npm run build` antes de cualquier `push`.
* **100% textos en archivos i18n** — Cero hardcoded.
* **CSS Puro** — Sin frameworks.
* **WCAG AA obligatorio** — Contraste 4.5:1 mínimo.

---

## 🔗 Enlaces

* **Wiki:** https://github.com/AnaBHernandez/red3conecta-landing/wiki
* **Projects:** https://github.com/users/AnaBHernandez/projects/13
* **Deploy:** https://red3conecta-landing.vercel.app/ 
* **Rama compartida:** `landing-page`

---

## 👥 Equipo


[Paula](https://github.com/paulova0121-alt) 
[Cynthia](https://github.com/Zebdon) 
[Ana Belén](https://github.com/AnaBHernandez) 
[Jessica](https://github.com/rodriguezjessika36-debug) 

**Última actualización:** 18/06/2026 | Ana Belén (Scrum Master)
