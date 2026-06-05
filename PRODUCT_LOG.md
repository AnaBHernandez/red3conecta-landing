# 📊 PRODUCT_LOG.md - Red3Conecta Landing

Bitácora histórica del desarrollo de la landing page de Red3Conecta. Registra el contexto, problemas resueltos y criterios de calidad de cada hito validado por el equipo.

---

## 🟢 [HITO 1]: Establecimiento de la Gobernanza y Ecosistema de Orquestación (Sprint 1)
- **Problema:** Necesidad de migrar del enfoque de servidor Express antiguo a una arquitectura estática moderna con Astro, aislar dependencias correctamente, fijar estándares visuales y coordinar un entorno de trabajo híbrido con modelos de IA en local para optimizar el consumo de tokens.
- **MVP:** - Definición del flujo Git Flow simplificado en la rama de integración `dev`.
  - Creación de la política de nombres de ramas de tareas bajo el formato `feature/*`.
  - Establecimiento del modelo híbrido de desarrollo y orquestación del proyecto (Ana Belén + Gemini + Claude + Ollama).
- **QA-IA:** Verificación del aislamiento de `node_modules` mediante el archivo oculto `.gitignore` en la raíz del espacio de trabajo.

---

## 🟢 [HITO 2]: Arquitectura de Estilos y Chasis Base (Sprint 1 - COMPLETADO)
- **Problema:** Saneamiento de las hojas de estilo base de la diseñadora y maquetación del chasis raíz de la landing de sección única para evitar colapsos visuales y asegurar la navegación nativa por anclas sin usar layouts redundantes. Bloqueo inicial por error de TypeScript (`Cannot find module '../i18n/ca.json'`).
- **MVP:**
  - Creación física del directorio `src/i18n/` y archivo `src/i18n/ca.json` con las claves oficiales en catalán del documento de contenidos de Jesús Rivera.
  - Depuración de sintaxis en `src/styles/global.css`, saneando las llaves de cierre del bloque `:root`.
  - Implementación de resets universales (`*`), comportamiento de desplazamiento suave (`scroll-behavior: smooth`) y offset de anclas (`scroll-margin-top: 80px`) para evitar el solapamiento con el menú fijo corporativo.
  - Maquetación del chasis raíz semántico en `src/pages/index.astro` con atributo `lang="ca"` obligado para cumplir con la accesibilidad WCAG AA.
- **QA-IA:** Sintaxis de cascada CSS y módulo JSON validados. El entorno en la rama `dev` compila al 100% sin errores de tipado o archivos faltantes mediante `npm run build`. El árbol de directorios locales cumple de forma estricta las líneas rojas de Paula.

---

## 🟢 [HITO 3]: Saneamiento de Historial y Alineación de Entorno (Sprint 1)
- **Problema:** Commit erróneo inicial redactado en catalán que rompía la convención de idioma establecida para las bitácoras internas de gobernanza y control del repositorio.
- **MVP:** - Ejecución de un desecho seguro del commit en la terminal de Ubuntu mediante un reset suave (`git reset --soft HEAD~1`).
  - Preservación íntegra de los archivos físicos de documentación creados en el espacio de trabajo local.
  - Reempaquetado y confirmación del commit con el mensaje de control redactado estrictamente en español.
- **QA-IA:** Verificación del árbol de Git limpia. Los archivos `PRODUCT_LOG.md` y `WIKI_GOVERNANZA.md` han pasado con éxito al histórico de la rama `dev`.

---

## 🟢 [HITO 4]: Alineación de Design Tokens y Desbloqueo de Cascada CSS (Sprint 1 - COMPLETADO)
- **Problema:** Colapso visual en el servidor de desarrollo local (`http://localhost:4321`). El componente `Navbar.astro` ignoraba los estilos globales debido a una desalineación de nombres de variables CSS y a un error de sintaxis en la primera línea de `global.css`, donde la falta de un salto de línea limpio unía el bloque de comentarios corporativos de Paula con la apertura del `:root`.
- **MVP:**
  - Refactorización atómica de los estilos encapsulados de la Navbar para consumir estrictamente los tokens oficiales de Paula (`--color-white`, `--color-black`, `--color-light-brown`, etc.).
  - Corrección sintáctica del archivo `src/styles/global.css`, aplicando un espaciado limpio para habilitar el parseo correcto de las propiedades `:root`.
  - Vinculación explícita e importación del archivo de estilos globales en el *frontmatter* de `src/pages/index.astro`.
- **QA-IA:** Compilación local exitosa. Verificación visual en navegador de la correcta aplicación del esquema de color cálido, tipografías estructuradas y pseudo-clases (`:hover`) corporativas sobre el componente.

---

## 🟢 [HITO 5]: Apertura del Ciclo de QA e Inclusión del Equipo (Sprint 1 - COMPLETADO)
- **Problema:** Necesidad de unificar el componente dinámico `<Navbar />` dentro del chasis estructural definitivo y aislar los envíos en el servidor remoto de GitHub, evitando alteraciones accidentales de la rama común de desarrollo (`dev`) antes de pasar la auditoría interna.
- **MVP:**
  - Sustitución del menú HTML plano manual por la inyección limpia del componente modular `<Navbar />` en `index.astro`.
  - Saneamiento y limpieza de la rama local `dev` mediante el comando `git restore` para asegurar la neutralidad del repositorio.
  - Sincronización masiva de los cambios en la rama de trabajo aislada `feature/navbar` y apertura formal de la **Pull Request (PR)** dirigida hacia la rama `dev`.
- **QA-IA:** Flujo Git Flow cerrado con éxito por parte de la Scrum Master. El código queda en estado "En Revisión" en la Wiki, transfiriendo el relevo a Jessica (QA) para la verificación física del comportamiento responsivo e i18n en su máquina local antes de autorizar el *merge*.

## 🟢 [HITO 6]: Consolidación de la Navbar y Depuración de Design Tokens (Sprint 1 - COMPLETADO)
- **Problema:** Los enlaces de la barra se volvían de color azul y subrayados por defecto tras ser pulsados debido a la falta de control de estados nativos del navegador. Además, el texto del footer se solapaba por detrás de la Navbar al hacer scroll debido a que la propiedad `position: sticky` flotaba sobre un contenedor transparente sin un fondo opaco definido.
- **MVP:**
  - Optimización radical de `src/styles/global.css`, eliminando el 100% de los comentarios informativos para aligerar la carga de la cascada CSS y agilizar el parseo.
  - Implementación de las pseudo-clases `:visited` y `:active` fijadas en color negro (`var(--color-black)`) con la regla estricta `!important` en `Navbar.astro` para anular permanentemente los estilos por defecto del navegador.
  - Corrección de la clase `.navbar` inyectando un fondo opaco `#ffffff` sólido y una sombra de separación base (`box-shadow`) de respiro visual.
- **QA-IA:** Verificación en `localhost:4321` exitosa tras incorporar la importación de `global.css` en la raíz. La barra se comporta como un bloque sólido, opaco e independiente, y los enlaces mantienen el flujo cromático corporativo antes y después de interactuar con ellos. Cambios fusionados y subidos limpiamente a la rama remota `dev`.

## 🟢 [HITO 7]: Migración a Rama Compartida Landing-Page (Sprint 1 - COMPLETADO)
- **Problema:** Necesidad de cambiar estrategia Git Flow: eliminar ramas `feature/*` individuales y adoptar rama compartida `landing-page` para trabajo coordinado del equipo.
- **MVP:**
  - Creación de rama `landing-page` desde `dev`
  - Nuevo flujo: compañeras pushean a `landing-page`, Ana Belén verifica y mergea a `dev`
  - Actualización de wikis GitHub con nueva política de ramas
- **QA-IA:** Rama creada, flujo documentado en wikis, equipo alineado.

---

## 📋 SPRINT 1 - ESTADO ACTUAL
✅ **#12 Layout + Base CSS** - Completado  
✅ **#13 Navbar** - Completado  
⏳ **#14 Footer** - Cintia (en Landing-page)  
⏳ **#18 Plan de Pruebas WCAG AA** - Ana Belén (siguiente)