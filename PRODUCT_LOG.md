# 📊 PRODUCT_LOG.md - Red3Conecta Landing

Bitácora histórica del desarrollo de la landing page de Red3Conecta. Registra el contexto, problemas resueltos y criterios de calidad de cada hito validado por el equipo.

---

## 🟢 [HITO 1]: Establecimiento de la Gobernanza y Ecosistema de Orquestación (Sprint 1)
- [cite_start]**Problema:** Necesidad de migrar del enfoque de servidor Express antiguo a una arquitectura estática moderna con Astro[cite: 502], aislar dependencias correctamente, fijar estándares visuales y coordinar un entorno de trabajo híbrido con modelos de IA en local para optimizar el consumo de tokens.
- [cite_start]**MVP:** - Definición del flujo Git Flow simplificado en la rama de integración `dev`[cite: 561, 570].
  - [cite_start]Creación de la política de nombres de ramas de tareas bajo el formato `feature/*`[cite: 570, 572].
  - Establecimiento del modelo híbrido de desarrollo y orquestación del proyecto (Ana Belén + Gemini + Claude + Ollama).
- **QA-IA:** Verificación del aislamiento de `node_modules` mediante el archivo oculto `.gitignore` en la raíz del espacio de trabajo.

---

## 🟢 [HITO 2]: Arquitectura de Estilos y Chasis Base (Sprint 1)
- **Problema:** Saneamiento de las hojas de estilo base de la diseñadora y maquetación del chasis raíz de la landing de sección única para evitar colapsos visuales y asegurar la navegación nativa por anclas sin usar layouts redundantes.
- **MVP:**
  - Depuración de sintaxis en `src/styles/global.css`, saneando las llaves de cierre del bloque `:root`.
  - Implementación de resets universales (`*`), comportamiento de desplazamiento suave (`scroll-behavior: smooth`) y offset de anclas (`scroll-margin-top: 80px`) para evitar el solapamiento con el menú fijo corporativo.
  - Creación del archivo unilingüe de internacionalización `src/i18n/ca.json` con los literales oficiales para `nav` y `footer` extraídos del documento de contenidos aprobado por Jesús Rivera.
  - Maquetación del chasis raíz semántico en `src/pages/index.astro` con atributo `lang="ca"` obligado para cumplir con la accesibilidad WCAG AA.
- **QA-IA:** Sintaxis de cascada CSS validada y pruebas de tipado de datos estáticos completadas con éxito en el frontmatter de Astro sin errores de compilación (`npm run dev`).

---

## 🟢 [HITO 3]: Saneamiento de Historial y Alineación de Entorno (Sprint 1)
- **Problema:** Commit erróneo inicial redactado en catalán que rompía la convención de idioma establecida para las bitácoras internas de gobernanza y control del repositorio.
- **MVP:** - Ejecución de un desecho seguro del commit en la terminal de Ubuntu mediante un reset suave (`git reset --soft HEAD~1`).
  - Preservación íntegra de los archivos físicos de documentación creados en el espacio de trabajo local.
  - Reempaquetado y confirmación del commit con el mensaje de control redactado estrictamente en español.
- **QA-IA:** Verificación del árbol de Git limpia. Los archivos `PRODUCT_LOG.md` y `WIKI_GOVERNANZA.md` han pasado con éxito al histórico de la rama `dev`.