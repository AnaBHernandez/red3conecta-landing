# 📊 Bitácora de Proyecto: Red3Conecta
*Última actualización: 13/06/2026*

## 🎯 Estado General
**Sprint 1-2:** ✅ COMPLETADO  
**Sprint 3:** ⏳ EN CURSO (Refinamiento UI, i18n Bilingüe y Estandarización)

---

## ⚠️ Bloqueos / Impedimentos
- ✅ **Resuelto:** Navegación sincronizada y funcional (Navbar ↔ índices de secciones).
- ✅ **Implementado:** Sistema i18n bilingüe (ES/CA) con selector dinámico en Navbar.
- ⏳ **Pendiente:** Ajuste final de estilos del 404 y refactorización de "números mágicos" en CSS.

---

## ✅ Sprint 1 y 2 — COMPLETADO
- Desarrollo de 8 componentes visuales (Layout, Navbar, Footer, Hero, About, 4 Sections).
- Sincronización de anclajes (IDs) entre Navbar e index.astro completada.
- Sistema i18n base implementado (ca.json).

---

## ⏳ Sprint 3 — EN CURSO
| ID | Tarea | Responsable | Estado | Notas |
|---|---|---|---|---|
| #18 | Migración i18n completa (ES/CA) | Equipo | ⏳ EN CURSO | Sistema bilingüe funcional. |
| #31 | Mejoras de Estilos Dinámicos | Equipo | ✅ FINALIZADO | Variables CSS globales + transiciones 0.3s. |
| #26 | Gestión Recursos Marca | Paula | ⏳ SIGUIENTE | Consolidación de assets. |
| #27 | Git Merges + Deploy Netlify | Ana Belén | ⏳ SIGUIENTE | Programado tras QA final. |
| #32 | Auditoría QA/WCAG AA | Ana Belén | 🔍 EN REVISIÓN | Validación accesibilidad + contraste. |

---

## 🟢 Hitos Completados (Sprint 3)

### [HITO 8] Sistema i18n Bilingüe
- Selector de idiomas (ES/CA) en Navbar
- Sincronización de claves JSON (es.json ↔ ca.json)
- Carga dinámica de textos en componentes

### [HITO 9] Optimización de Estilos
- Migración a variables CSS globales (`:root`)
- Transiciones suaves (0.3s ease)
- Estados :hover, :focus, :visited, :active definidos

---

## 📌 Próximos Pasos
- [ ] Refactorización final: Eliminar "números mágicos" en CSS
- [ ] Implementación de Scroll Reveal (post-auditoría)
- [ ] Test final de accesibilidad con lector de pantalla (NVDA/VoiceOver)
- [ ] Deploy a producción en Netlify

---

## 🔧 Criterios DoD (Todos los componentes)
✅ Responsive (desktop + móvil ≤375px)  
✅ WCAG AA confirmado  
✅ 100% textos en ca.json/es.json  
✅ CSS Puro, sin frameworks  
✅ npm run build sin errores  
✅ i18n Bilingüe funcional  

---

*Nota: Sistema i18n bilingüe operativo. El proyecto soporta ES y CA dinámicamente.*