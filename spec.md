### spec.md
1. Localizar los archivos `Sectioneight.astro` y `Sectionnine.astro`.
2. Identificar y eliminar las líneas `var(--color-border): ...` (sintaxis inválida).
3. Reemplazar por la propiedad CSS correcta (ej. `border: var(--border-base) solid var(--color-border);`).
4. Validar compilación con `npm run build`.