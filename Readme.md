Configuración del Servidor Local y ngrok

Para cargar el proyecto que utiliza un modelo de Tensorflow.js, es necesario acceder a través de http/https. Puedes usar cualquier servidor para esto, y aquí te proporcionamos una forma de hacerlo:

1. **Configuración del Servidor Local**:

    Descarga Python en tu computadora si aún no lo tienes instalado.

    - Abre una línea de comandos o terminal.
    - Navega hasta la carpeta donde descargaste el repositorio.
    - Ejecuta el siguiente comando para iniciar un servidor local: 
      ```
      python -m http.server 8000
      ```
    - Abre tu navegador web y ve a http://localhost:8000 para acceder al proyecto.

2. **Utilización de ngrok**:

    Si deseas abrir el proyecto en tu dispositivo móvil y usar la cámara, necesitarás una conexión HTTPS. Puedes lograrlo usando ngrok:

    - Descarga ngrok en tu computadora y descomprímelo.
    - Abre una línea de comandos o terminal.
    - Navega hasta la carpeta donde descargaste ngrok.
    - Ejecuta el siguiente comando para crear un túnel HTTPS hacia tu servidor local:
      ```
      ngrok http 8000
      ```
    - Asegúrate de tener activos tanto el servidor local Python como el túnel ngrok.
    - En la línea de comandos, aparecerá un enlace HTTPS proporcionado por ngrok. Puedes acceder a este enlace desde tu dispositivo móvil, incluso si no estás en la misma red local.
    - Ten en cuenta que el túnel de ngrok expirará después de un tiempo (generalmente 2 horas), en ese caso, simplemente reinicia ngrok.
    - Abre un navegador en tu dispositivo móvil y visita el enlace HTTPS proporcionado por ngrok.
