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

## Forks y colaboración

### 1. ¿Qué es un fork en GitHub?

Un fork es una copia de un repositorio que se crea en GitHub dentro de otra cuenta. Permite trabajar sobre un proyecto existente sin modificar directamente el repositorio original.

### 2. ¿En qué se diferencia un fork de una rama?

Una rama es una línea de trabajo dentro del mismo repositorio. En cambio, un fork es otro repositorio independiente en GitHub, que puede tener sus propias ramas y cambios.

### 3. ¿En qué cuenta se almacena un fork?

Normalmente, el fork se almacena en la cuenta de GitHub de la persona que lo crea. Así puede desarrollar sus cambios sin necesidad de tener permisos de escritura en el repositorio original.

### 4. ¿Cuándo resulta útil trabajar mediante un fork?

Es útil cuando queremos colaborar en un proyecto de otra persona, probar nuevas funciones o corregir errores sin modificar directamente su repositorio. También permite trabajar cuando no tenemos permisos para escribir en el original.

### 5. ¿Qué relación existe entre el repositorio original y el fork?

El fork parte del contenido del repositorio original, pero ambos pueden evolucionar de forma independiente. Los cambios realizados en uno no se incorporan automáticamente al otro.

### 6. ¿Qué es el repositorio upstream?

Upstream es el nombre que se suele dar al repositorio original del que procede un fork. Se utiliza como referencia para consultar sus cambios y, cuando sea necesario, incorporarlos al fork.

### 7. ¿Qué diferencia existe entre origin y upstream?

`origin` suele identificar el repositorio remoto asociado a nuestro repositorio local, normalmente nuestro propio fork. `upstream` suele identificar el repositorio original del proyecto. Son nombres convencionales que se pueden configurar de otra manera.

### 8. ¿Cómo se propone que un cambio del fork llegue al repositorio original?

Cuando los cambios están preparados y publicados en el fork, se puede abrir una solicitud de incorporación de cambios (*pull request*). En ella se explica qué se ha modificado para que los responsables del proyecto puedan revisarlo.

### 9. ¿Quién decide si se acepta la propuesta?

La decisión corresponde a los responsables o mantenedores del repositorio original, según sus normas de colaboración. Pueden aceptar los cambios, pedir modificaciones o rechazar la propuesta.

### 10. ¿Puede seguir evolucionando el repositorio original mientras existe el fork?

Sí. El repositorio original y el fork pueden recibir cambios por separado. Si el original avanza, podemos actualizar nuestro fork incorporando esos cambios y resolver posibles conflictos si las modificaciones afectan a las mismas partes del código.