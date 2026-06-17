# spec.md — Especificaciones Técnicas y Bitácora de Cambios

## 1. Correcciones de Sintaxis CSS (Sprint 2)
* **Problema:** Definiciones de variables CSS ilegales dentro de componentes (`Sectioneight.astro`, `Sectionnine.astro`).
* **Acción:** Eliminadas declaraciones `var(--variable): valor` y reemplazadas por el uso de variables en propiedades estándar.
* **Sintaxis:** Se ha estandarizado a:
    `border: 1px solid var(--color-border);`
    `border-radius: var(--radius-md);`

## 2. Refactorización de Navegación (Sprint 3)
* **Problema:** Redundancia en el selector de idioma (`.navbar__lang`) y conflictos de posicionamiento (alineación izquierda/derecha) en desktop y mobile.
* **Estrategia:** 1.  Extracción de `.navbar__lang` fuera del contenedor `.navbar__menu`.
    2.  Agrupación lógica mediante `div.navbar__right-group` para el selector de idioma y el botón hamburguesa.
    3.  Uso de `display: flex` con `margin-left: auto` para garantizar la alineación a la derecha en todos los viewports.
* **Acción:** * Reorganización del HTML en `Navbar.astro`.
    * Implementación de `order` en CSS para asegurar que el botón hamburguesa siempre esté tras el selector de idiomas.
    * Aumento de `max-width` en `navbar__container` a `1280px` para mejor distribución del espacio.

## 3. Validación y QA
* **Build:** `npm run build` verificado exitosamente.
* **Responsive:** Comprobado que el layout se mantiene en línea y no se superponen los elementos tras el ajuste de márgenes.
* **Git Flow:** Cambios validados en `landing-page`, fusionados en `styles-changes`.

---
*Documentación técnica mantenida por: Ana Belén (Scrum Master)*
*Fecha: 17/06/2026*