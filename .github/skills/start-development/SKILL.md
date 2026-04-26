---
name: start-development
description: Utilízala para iniciar un nuevo desarrollo a partir de un ticket de Jira.
---

Cuando se solicite iniciar un nuevo desarrollo:

1. Extrae el código y una breve descripción del resumen del ticket de Jira.
2. Propón nombres para la nueva rama:
    - Genera varias opciones con la descripción en formato train-case `{código}_{descripción}`
    - Ejemplo *Crear widget para mostrar la información del cliente en la página de caso*:
        - ABC-123_Crear-Widget-Cliente
        - ABC-123_Widget-Info-Cliente-Caso
        - ABC-123_Cliente-Widget-Caso
   - Solicita al usuario que elija una opción.
3. Cambia a la rama `master`.
4. Actualiza `master` con los últimos cambios del repositorio remoto.
5. Crea una nueva rama desde `master` con el nombre seleccionado y cámbiate a ella.
6. Genera el manifest `sf project generate manifest --name {código}_{descripción} --output-dir manifest/minors --source-dir .github`.
7. Informa al usuario de que todo está listo para comenzar el desarrollo y no hagas ni preguntes nada más.