# spec.md
Objetivo: Validar la ejecución del pipeline tras configurar los secretos.
Acción: Hacer push a rama `landing-page` y monitorear logs en pestaña Actions.
DoD:
- Pipeline completa el job `deploy` con éxito (check verde).
- El log ya no muestra el error 404.