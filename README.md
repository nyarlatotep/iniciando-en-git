# Init on git


**some basic helps and references to begginers on git, locally and synch it to remotes.**

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
                                                                                                                                                             
                                                                                                                                                             
>  Something like a guide for Begginers. All of us need guidence at the start, Mom was there when learn to walk 😂🤩😛                                       
>  I will add another version in english soon, just that i have time for.                                                                                     
                                                                                                                                                                                                                                                                                                                                             
--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Para todos aquellos que comienzan a utilizar y conocer **"Git"** como sistema de control de versiones para proyectos/colaborativos, lo mas recomendable, solo como consejo y dato básico para quienes no lo sepan o tengan una base y conocimiento acerca de; es familiarizarse con el uso de la consola de comandos, sea cual sea la que les agrade utilizar ya sea **"bash"** en Linux y sus distros, **"Powershell"** o **"CMD"** en Windows, los comandos para utilizar la **"CLI"** > (Command Line Interface) de Git son prácticamente los mismo en todas, a excepción de ciertas variables específicas de cada  consola.

Haciendo referencia a lo anterior, por supuesto hay que saber que dicha CLI, hay que instalarla como aplicación o paquete dependiendo el sistema operativo así como el medio por el que lo desees instalar; Estos pueden ser:

* Linux y distros (Debian y ZYpp hay muchas otras y sus respectivos package manager)
   * En el caso de Linux la única manera de instalarlo es por medio de la interface de comandos haciendo uso de administrador de paquetes __apt__ o __apt-get__ en el caso de sitemas Debian y __zypper__ en el caso de sistemas de bibliotecas ZYpp como es el caso de OpenSUSE
      
      ```bash
      sudo apt-get update && sudo apt-get upgrade  \
      sudo apt-get install git 
      ```
      ```bash
      sudo zypper update
      sudo zypper upgrade
      sudo zypper install git
      ```
--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

* Windows 
   * En el caso de Windows es posible instalar la CLI de varias maneras, pero por mencionar las mas rápidas, son:
   1. Descargar el paquete de instalación, archivo .zip o .tar (De inicio es mejor el bin o exe) 
       Lo pueden encontrar en el [sitio oficial de git-scm](https://git-scm.com/). Aqui tmb pueden encontrar todas las formas de instalarlo en 
       las distros de linux.
    2. El repositorio de [git en GitHub](https://github.com/git/git).
    3. Algún administrador de paquetes como Node.js (npm) o Chocolatey si es que tuvieran instalado alguno:

npm:

    npm install git@latest -g
         
choco:      

    choco install git --required-version <version-a-instalar>
      
----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

En fin cualquiera que sea el método es lo mas recomendable iniciar por conocer los comandos básicos para administrar repositorios locales y sincronizarlos con los "remotes" los cuales conocen bien y son los que se alojan aquí en el hub de  **GitHub**; para lo cual es importante saber como es el funcionamiento inicial para que no resulte en problemas como los que muchos tuvimos al principio y que ustedes manifiestan experimentar. 
Antes de ocupar un __"IDE"__ o entorno de desarrollo (Puedo recomendarles [Atom](https://github.com/atom/atom) un editor de código opensource, ligero y potente desarrollado por GitHub, o tmb [VisualStudio Code](https://code.visualstudio.com/Download) de Microsoft, editor de código potente y ligero, tiene muchos plug-in's (extensiones) que les serán de mucha ayuda), es recomendable lo antes mencionado y saber que inicialmente:

**
1. Debes crear el repositorio en GitHub
2. Si tienes un repo local, asegurate de crear el archivo de ignorados .gitignore, para evitar que subas carpetas o archivos que no son útiles o no deban estar en la red.
3. Si quieres subir un proyecto o parte de el al hub, pero no has iniciado un repositorio local __(git init)__ presta atención en que directorio o carpeta estas ubicado en tu consola, si aun no lo sabes bien, tendrás que clonar tu repo en la web dentro tu directorio local __(git clone <https url> <ssh url>)__ a lo que yo pienso y opino que es la mejor manera como iniciado, de sincronizar tus repositorios y no te estes confundiendo con las ramas y como agregar o eliminar remotos etc, Primero lo primero, claro. 
4. Continuando en el punto anterior, Observa en que directorio te ubicas antes de ejecutar git clone, cuando clonas el repositorio este **CREA UNA NUEVA CARPETA** conteniendo todo lo que haya en tu repositorio en la web, así como una carpeta oculta .git donde se encuentra la configuración global, los REFS, HEADS, diffs, entre otros. Si haces el clone dentro de la carpeta que contiene tu proyecto local, esta quedará fuera de tu repositorio clonado, conteniendo esté a su vez y habrá una bola de problemas y confusiones si quieres sacar la carpeta clonada o meter los archivos a esta. 
5. Es mejor clonar el repositorio en un __"source"__ como P/E  **"C:\\Users\<tu-usuario>\source\repos\<todos-tus-repos>"**  de esta manera queda fuera de tu proyecto e independiente , dejando la libertad y posibilidad de que puedas arrastrar o copiar tus archivos de proyecto que quieras subir a tu repo en GitHub y evitandote dolores de cabeza y complicar lo que no lo es.
**
  
--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Para terminar y espero les sea de ayuda lo anterior, claro que hay mucho mas, pero creo que lo anterior es algo que no muchos sabemos cuando iniciamos y que es lo mas básico para ir comprendiendo el funcionamiento, los comandos y pasos posteriores y mas avanzados de administrar git, les recomiendo mucho que visiten el siguiente link, el cual los llevará a los Labs de GitHub, que son tutoriales y pequeños cursos, muy bien explicados e interactivos, para iniciadores y unos mas avanzados. Con estos comprenderás mas a fondo que es, lo que puedes hacer y como administrar tus repositorios y contribuir en proyectos grupales o de código abierto.

https://lab.github.com/

Suerte y recuerda que echando a perder se aprende :P así como también la práctica hace al maestro y mas "tonto" el que no pregunta que el que quiere disipar las dudas y adquirir conocimientos. 😛
