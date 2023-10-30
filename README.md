# Para los amantes de .NET ❤️

Para poder ejecutar estas demos necesitas:

- Docker 🐋 instalado en tu máquina.
- La extensión [Dev Containers](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers) 🛳️ en Visual Studio Code.
- Clona este repo 👩‍💻
- O también puedes ejecutarlo en GitHub Codespaces 🐈‍⬛ [Echa un vistazo a este vídeo](https://www.youtube.com/watch?v=0qKG37C8sb8)


## Demos Copilot Chat

1. ¿Cómo puedo crear una API en .NET Core con dotnet cli? (hazle caso 🫡)
2. Intenta restaurar las dependencias, compilarlo, ejecutarlo, etc. a ver si lo hizo bien 🤓. En el archivo steps.sh tienes los comentarios que te ayudarán a preguntarle a GitHub Copilot
4. Usa la extensión de Postman para probar la API
3. Prueba lo mismo con el comando */createworkspace*
4. ¿Puedes explicarme lo que hace esta clase?
5. Ahora vamos a crear una API que gestione heroes. Para ello, lo primero que le voy a pedir es que me cree un modelo para estos: *Creáme un modelo para heroes*. Si reponde con una posible solución tienes 4 opciones:

<img src="images/GH%20Copilot%20Chat%20opciones%20cuando%20te%20genera%20código.png" width="40%">

La primera de ellas sirve para copiar el código en el portapapeles, la segunda lo inserta en el lugar donde esté el cursor en ese momento. Si haces clic sobre los tres puntos te permite generar un nuevo archivo con el contenido generado y, por último, tienes la opción de lanzar lo generado en el terminal.

Ahora con este modelo vamos a generar el controlador. Con el archivo abierto, pregúntale a GitHub Copilot Chat si puede crearte la API para este modelo. Podemos preguntar algo como **¿Puedes crearme una API para este modelo?** o **¿Puedes crearme un controlador para este modelo?**. (A la hora de escribir este markdown no me incluyó el using ni el namespace, pero fue fácil solucionarlo).

Si ahora ejecutas la aplicación deberías de tener una API que te permite hacer un CRUD sobre los heroes. Puedes probarlo con Postman.

También puedes preguntarle **¿Cómo puedo llamar a esta API desde Postman?** y te indicará los pasos de cómo hacerlo. En este entorno tienes instalada la extensión de Postman por si quieres probar.

<img src="images/GH%20Copilot%20Chat%20también%20te%20explica%20cómo%20usar%20Postman%20con%20este%20código.png" width="40%">
