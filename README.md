# 📊 Red3Conecta - Landing Page (ConnectaDona)

Infraestructura digital compartida construida con el tercer sector, para el tercer sector. Un proyecto impulsado por Factoría F5 y Fundació Formació i Treball, con el soporte de UNADA.

## 🛠️ Especificaciones Técnicas
- **Framework:** Astro v4 (SPA, sin `layouts/`).
- **Estilos:** CSS Nativo (`src/styles/global.css`) usando variables `:root`. **PROHIBIDO:** Tailwind, Bootstrap, Sass.
- **Internacionalización (i18n):** Catalán exclusivo (Català). Textos dinámicos en `src/i18n/ca.json`. Cero hardcoded strings.
- **Accesibilidad:** Estándar estricto WCAG AA (ARIA labels, focus visible, contraste 4.5:1).

## 🌿 Flujo de Trabajo (Git Flow)
1. `main`: Producción (Bloqueado).
2. `dev`: Integración.
3. `landing-page`: Rama compartida de trabajo diario.

## 📋 Estado del Proyecto (Sprints)
- **Sprint 1 (Jun 01-07):** Layout, Base CSS, Navbar, Footer (#12, #13, #14).
- **Sprint 2:** Hero, About, Challenges, Ally, QA Central (#19, #20, #21, #22, #23).
- **Sprint 3:** Ecosystem, Partners, Final Deploy (#24, #25, #26, #27).

## 🛡️ Líneas Rojas de Desarrollo
- Prohibido hacer `push` directo a `main`.
- Prohibido incluir comentarios metodológicos en el código visual.
- Obligatorio `npm run build` antes de cualquier `push`.