# PRODUCT_LOG.md
*Última actualización: 08/06/2026 | Scrum Master: Ana Belén*

## 🏁 ESTADO: SPRINT 1 (Cierre)
| Componente | Estado | Responsable | Notas |
| :--- | :--- | :--- | :--- |
| **#12 Layout** | ✅ HECHO | Ana Belén | CSS Nativo |
| **#13 Navbar** | ✅ HECHO | Ana Belén | i18n + WCAG AA |
| **#14 Footer** | ✅ HECHO | Cintia | CSS saneado |
| **#17 Assets** | 🔴 BLOQUEO | Paula | Pendiente migración a /public |
| **#18 Auditoría**| ⏳ ESPERA | Ana Belén | Plan Pruebas WCAG AA |

## 🚀 SPRINT 2 (En curso)
| Componente | Estado | Responsable | Notas |
| :--- | :--- | :--- | :--- |
| **#19 Hero** | ✅ HECHO | Ana Belén | Estructura semántica + i18n |
| **#20 About** | 📋 PENDIENTE | Cintia | (Antiguo Sectionfive) |
| **#21 Challenges**| 📋 PENDIENTE | Paula | (Antiguo Sectionsix) |
| **#22 Ally** | 📋 PENDIENTE | Paula | - |
| **#23 Platform** | 📋 PENDIENTE | Ana Belén | (Antiguo Sectionfour) |
| **#29 Impact** | 📋 PENDIENTE | Paula | - |

## 🚧 LOG DE INCIDENCIAS
* **Bloqueo Crítico (#17):** Errores 404 en la carga de iconos. El desarrollo depende de Paula.
* **Gestión de Gobernanza:** Se ha eliminado `Card.astro` del inventario activo para optimizar el bundle.
* **Sincronización:** Se ha mantenido la nomenclatura `Sectionfour/five/six` en el sistema de archivos para evitar roturas de compilación, pero se han mapeado correctamente en este Log contra las tareas del Backlog.
* **Calidad (Línea Roja #5):** Se detecta texto *hardcoded* en componentes de terceros. Se ha establecido el plan de refactorización centralizada en `ca.json` para el día 09/06/2026.