# GitHub Copilot para los amantes de .NET ❤️

Para poder ejecutar estas demos necesitas:

- Docker 🐋 instalado en tu máquina.
- La extensión [Dev Containers](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers) 🛳️ en Visual Studio Code.
- Clona este repo 👩‍💻
- O también puedes ejecutarlo en GitHub Codespaces 🐈‍⬛ [Echa un vistazo a este vídeo](https://www.youtube.com/watch?v=0qKG37C8sb8)


## Demos Copilot Chat

1. ¿Cómo puedo **crear una API en .NET Core con dotnet cli**? (hazle caso 🫡)
2. Intenta restaurar las dependencias, compilarlo, ejecutarlo, etc. a ver si lo hizo bien 🤓. En el **archivo steps.sh** tienes los comentarios que te ayudarán a preguntarle a GitHub Copilot
4. Usa la extensión de Postman para **probar la API**
3. Prueba lo mismo con el comando **/new**
4. **¿Puedes explicarme lo que hace esta clase?**
5. Ahora vamos a crear una API que gestione heroes. Para ello, lo primero que le voy a pedir es que me cree un modelo para estos: **Creáme un modelo para heroes**. Si reponde con una posible solución tienes 4 opciones:

<img src="images/GH%20Copilot%20Chat%20opciones%20cuando%20te%20genera%20código.png" width="50%">

La primera de ellas sirve para copiar el código en el portapapeles, la segunda lo inserta en el lugar donde esté el cursor en ese momento. Si haces clic sobre los tres puntos te permite generar un nuevo archivo con el contenido generado y, por último, tienes la opción de lanzar lo generado en el terminal.

Ahora con este modelo vamos a generar el controlador. Con el archivo abierto, pregúntale a GitHub Copilot Chat si puede crearte la API para este modelo. Podemos preguntar algo como **¿Puedes crearme una API para este modelo?** o **¿Puedes crearme un controlador para este modelo?**. (A la hora de escribir este markdown no me incluyó el using ni el namespace, pero fue fácil solucionarlo).

Si ahora ejecutas la aplicación deberías de tener una API que te permite hacer un CRUD sobre los heroes. Puedes probarlo con Postman.

También puedes preguntarle **¿Cómo puedo llamar a esta API desde Postman?** y te indicará los pasos de cómo hacerlo. En este entorno tienes instalada la extensión de Postman por si quieres probar.

<img src="images/GH%20Copilot%20Chat%20también%20te%20explica%20cómo%20usar%20Postman%20con%20este%20código.png" width="50%">

6. Puedes pedirle que te ayude a configurar el proyecto para depurarlo en Visual Studio Code: 

<img src="images/GH Copilot Chat Cómo puedo hacer que me genere la configuración de VS Code para depurar.png" width="50%">

7. **Oye, no quiero almacenar los heroes en memoria, ¿puedes ayudarme a crear un repositorio para almacenarlos en una base de datos?**

A lo que me puede contestar con algo como esto:

<img src="images/GH Copilot me ayuda a crear un repositorio y la configuración de EF - parte 1.png" width="50%">

<img src="images/GH Copilot me ayuda a crear un repositorio y la configuración de EF - parte 2.png" width="50%">

<img src="images/GH Copilot me ayuda a crear un repositorio y la configuración de EF - parte 3.png" width="50%">

En mi ejemplo, le pido además que se asegure de que DbContext cree la base de datos si no existe.

8. **¿Puedes darme la cadena de conexión para SQL Server en localhost?**

Puede ser que la cadena de conexión que te de inicialmente no te funcione. En este laboratorio el objetivo es aprovechar la base de datos que tenemos como parte de la configuración del Dev Container.

9.  **¿Puedes ayudarme a hacer tests unitarios?**

Puedes preguntarle directamente a GitHub Copilot chat o utilizar la opción **/tests**. Si conoces el framework de tests unitarios que quieres utilizar puedes indicárselo. En mi caso, le indico que quiero usar xUnit.

Además, puedes preguntarle **¿Dónde puedes guardar estos tests?** y posiblemente te recomiende crear un proyecto de tests unitarios. Si no le has dicho qué framework quieres utilizar puede que te genere un proyecto en un framework diferente al que te hizo la clase anterior 😬.

<img src="images/GH Copilot Chat con el comando test te auyda a crear tests.png" width="50%">

Por último, puedes preguntarle **¿Cómo puedo ejecutar estos tests?** y te indicará los pasos a seguir. 

<img src="images/GH%20Copilot%20cómo%20ejecuto%20los%20test%20unitarios.png" width="50%">

En incluso si le pides algunas extensiones que te ayuden a ejecutar los tests te puede recomendar algunas.

<img src="images/GH Copilot recomendación de extensiones para los tests.png" width="50%">

10. ¿Puedes generarme el Terraform para desplegar esta web en Azure?

### Traducción de código a otros lenguajes

Otra petición que puedes hacerle a GitHub Copilot es que traduzca el código a otros lenguajes. Por ejemplo, abre el archivo **HeroesController.cs** y pídele que te traduzca el código a Python, por ejemplo: **¿Puedes traducir este código a Python?**. 

<img src="images/GH Copilot - Traducción a otros lenguajes.png" width="50%">
