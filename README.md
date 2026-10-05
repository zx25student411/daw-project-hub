# DAW Project Hub

Pequeña página web para practicar un flujo profesional de trabajo con Git y GitHub.

## Conflicto resuelto

El conflicto se produjo porque las ramas `main` y `feature/nuevo-eslogan` modificaron la misma línea del archivo `index.html`.

El archivo afectado fue `index.html`, concretamente el texto de presentación situado dentro de la cabecera.

Para resolverlo se decidió combinar las dos ideas en una única frase:

"Un espacio para aprender a desarrollar, publicar y mantener aplicaciones web, conociendo las fases de su desarrollo y despliegue."

La resolución se comprobó eliminando los marcadores de conflicto, ejecutando `git diff` y comprobando posteriormente con `git status` que no quedaban conflictos y que el repositorio estaba limpio.

## Instrucciones

### Abrir la página

Para abrir la página web, abre el archivo `index.html` en un navegador web o utiliza la opción "Go Live" de Visual Studio Code.

### Publicar la rama

Para publicar esta rama en GitHub, utiliza:

```bash
git push -u origin docs/instrucciones

## Fetch y Pull

`git fetch` descarga la información y los cambios del repositorio remoto, pero no los integra automáticamente en la rama local.

`git pull` descarga los cambios del repositorio remoto y los integra en la rama local.

Fetch permite revisar los cambios antes de integrarlos porque actualiza las referencias remotas sin modificar directamente nuestra rama de trabajo.

Pull combina la descarga de cambios con su integración posterior en la rama local.
