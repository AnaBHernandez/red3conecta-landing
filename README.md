# Red3Conecta — Landing Page

Infraestructura digital compartida construida con el tercer sector, para el tercer sector.  
Proyecto impulsado por **Factoría F5** y **Fundació Formació i Treball**, con el apoyo de **UNADA · Aigües de Barcelona**.

---

## 🛠️ Stack Técnico

| | |
|---|---|
| **Framework** | Astro v6.4.2 (SPA, sin `layouts/`) |
| **Lenguaje** | TypeScript nativo |
| **Estilos** | CSS puro · variables `:root` · sin Tailwind/Bootstrap/Sass |
| **i18n** | Bilingüe català/castellano · `ca.json` + `es.json` · cero hardcoding |
| **Accesibilidad** | WCAG AA · ARIA labels · contraste 4.5:1 · navegación teclado |
| **Gestor paquetes** | npm |

---

## 🚀 Inicio Rápido

```bash
# 1. Clonar el repositorio
git clone https://github.com/AnaBHernandez/red3conecta-astro-landing.git

# 2. Entrar en la carpeta
cd red3conecta-astro-landing

# 3. Cambiar a la rama de trabajo
git checkout landing-page

# 4. Instalar dependencias
npm install

# 5. Arrancar en desarrollo
npm run dev
# → http://localhost:4321
```

---

## 🌿 Git Flow

| Rama | Uso |
|---|---|
| `main` | Producción — **intocable** |
| `landing-page` | Rama activa de trabajo diario |
| `stable-backup` | Copia de seguridad — sincronizada con `landing-page` |

**Conventional commits:** `feat:` `fix:` `style:` `docs:` `chore:`  
**Merges:** responsabilidad exclusiva de Ana Belén (Scrum Master)

---

## 📋 Estado del Proyecto

### Sprint 1 ✅
| ID | Componente | Asignado |
|---|---|---|
| #12 | Layout + Base CSS | Ana Belén |
| #13 | Navbar.astro | Ana Belén |
| #14 | Footer.astro | Cintia |

### Sprint 2 ✅
| ID | Componente | Asignado |
|---|---|---|
| #19 | Hero.astro | Ana Belén |
| #20 | About.astro | Cintia |
| #21 | Sectionfive.astro | Paula |
| #22 | Sectionfour.astro | Paula |
| #29 | Sectionsix.astro | Paula |
| #24 | Sectioneight.astro | Jessica |
| #25 | Sectionseven.astro | Jessica |
| #30 | Sectionnine.astro | Jessica |

### Sprint 3 ✅
| ID | Tarea | Asignado |
|---|---|---|
| #18 | Migración i18n (ca.json + es.json) | Equipo | 
| #31 | Mejoras de Estilos Dinámicos | Equipo | 
| #27 | Git Merges + Deploy Netlify | Ana Belén | 
| #32 | QA, Accesibilidad y WCAG AA | Ana Belén |
| #26 | Gestión de Recursos de Marca | Paula | 
| #33 | Media Queries responsive | Equipo | 
| #34 | Fix overflow horizontal global.css | Ana Belén | 
| #35 | Fix footer__glow Footer.astro | Cintia |
| #36 | Fix carousel-track Sectionnine.astro | Jessica | 

---

## 🛡️ Líneas Rojas

- Prohibido push directo a `main`
- Prohibido texto hardcoded en componentes `.astro`
- `npm run build` obligatorio antes de cualquier push
- CSS puro — sin frameworks
- WCAG AA obligatorio

---

## 🔗 Enlaces

- 📁 **Repositorio:** https://github.com/AnaBHernandez/red3conecta-astro-landing
- 📖 **Wiki:** https://github.com/AnaBHernandez/red3conecta-landing/wiki
- 📋 **Board:** https://github.com/users/AnaBHernandez/projects/13
- 🚀 **Deploy:** https://red3conecta-landing.netlify.app

---

## 👥 Equipo

- 🧭 **Scrum Master:** [Ana Belén](https://github.com/AnaBHernandez)
- 📌 **Product Owner:** [Paula](https://github.com/paulova0121-alt)
- 💻 **Dev:** [Cintia](https://github.com/Zebdon)
- 💻 **Dev:** [Jessica](https://github.com/rodriguezjessika36-debug)

---

*Última actualización: 18/06/2026 · Ana Belén Hernández (Scrum Master)*