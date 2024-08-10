# Hello Node

Teniendo en cuenta los recursos anteriores de la semana, usted debe crear un archivo dockerfile que construya una imagen que cumpla con los siguientes requerimientos.

- La imagen debe extender de la versión 16 de node.
- La imagen debe exponer el puerto 3020, el cual es el puerto que usa la aplicación.
- La imagen debe copiar el archivo package.json y el archivo app.js dentro de ella. Solo esos dos archivos.
- La imagen debe instalar (en fase de build) todos los paquetes necesarios por medio del comando npm install.
- La imagen debe ejecutar el comando node app.js en fase de runtime. Esta ejecución debe ser tipo exec y no tipo shell. Para mayor información revise la documentación de docker.
- Agregue una etiqueta de metadata (LABEL) con el nombre "author" y su correo uniandes como valor. Esto será verificado por el calificador.

Suba su archivo Dockerfile como entregable de la actividad en coursera para cumplir con la entrega.

Para conseguir que usted complete satisfactoriamente con la configuración del dockerfile le recomendamos realizar los siguientes pasos:

### Primero) Cree el archivo dockerfile

- Descargue este repositorio en su máquina local.
- Cree el archivo Dockerfile al mismo nivel que el archivo app.js.
- Configure el archivo para que cumpla con los requerimientos especificados anteriormente.

### Segundo) Cree la imagen localmente

- Abra un terminal y ubíquese en la ruta del proyecto (al mismo nivel de los archivos app.js y Dockerfile).
- Use el comando de construcción de imágenes de docker haciendo uso del tag "hello-node". Recuerde que por estar ubicado en el mismo sitio del dockerfile la ruta para el archivo es únicamente un punto ( . ).
- Valide que se haya creado la imagen correctamente por medio del comando que lista las imágenes de docker.

### Tercero) Ejecute el contenedor

- Ejecute el comando que ejecuta la imagen "hello-node" en su máquina. Recuerde que debe hacer un mapeo de puertos para que pueda acceder al servicio en su máquina física.
- Valide por medio de su navegador el funcionamiento de la aplicación, accediendo a la ruta "http://localhost:**puerto**/hello". Verá un mensaje de felicitaciones.

Si cumple con los tres pasos, suba únicamente el archivo de Dockerfile a la actividad en coursera.

> Nota: solo en el caso que el dockerfile supere el validador, se calificará como lograda la actividad.

Éxitos!!
