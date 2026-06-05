# 📊 Red3Conecta - Landing Page (ConnectaDona)

Infraestructura digital compartida construida con el tercer sector, para el tercer sector. Un proyecto impulsado por Factoría F5 y Fundació Formació i Treball, con el soporte de UNADA.

## 🛠️ Especificaciones Técnicas
- **Framework:** Astro (Arquitectura limpia de sección única sin layouts redundantes).
- **Estilos:** CSS Nativo encapsulado mediante etiquetas `<style>` vinculadas a variables globales en `:root`. Prohibido el uso de utilidades externas (Tailwind/Bootstrap).
- **Estrategia de Idiomas (i18n):** Estrategia unilingüe exclusiva en **Catalán**. Todos los textos dinámicos se centralizan en `src/i18n/ca.json`.

## 🌿 Flujo de Trabajo en Git (Git Flow)
- `main`: Rama sagrada de producción (Protegida).
- `dev`: Rama común de integración para la unificación de los Sprints.
- `landing-page`: Rama compartida donde trabaja TODO el equipo (no ramas aisladas).