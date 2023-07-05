Walter

Pude solucionar el problema de compilacion de SASS a CSS. Lo que ellos quieren es que hagas el codigo de estilizado en SASS, y eso lo compiles a CSS.
(Ya que no se puede linkear una hoja de estilizado de SASS a un HTML)

* Elimine archivos que estaban vacios como son y eran inecesarios"_variables.scss, _bs.scss, _navbar.scss".

*Si te fijas en los archivos SASS vas a poder ver que todos sus nombres cambiaron por su igual en ingles. (Creo que se te va a ser mas facil escribir los archivos en ingles.)

*Tambien vas a encontrar en la carpeta de COMPONENTES un nuevo archivo llamado "_body,scss", alli se encuentra el codigo que estaba en el CSS al momento de descargar
la carpeta del proyecto. Podes ver que si eliminas la carpeta o simplemente borras el "@import "./componentes/body";" del archivo "_style.scss" van a desaparecer
varios estilos de la pagina (Estilos que anteriormente habias agregado al HTML).

*Instale las dependencias "node-sass", "nodemon" y eso lo hice cuando viniste trayendo la computadora. (Lo podes visualizar en el archivo "package.json").

*En el mismo archivo "package.json" vas a encontrar 2 nuevos scripts/comandos, cada vez que quieras compilar sass a css tenes que ejecutar el siguiente comando
en la terminal de tu Visual Studio "npm run watch-css". (Este comando va a convertir todo lo que este en la carpeta "_style.scss" a codigo CSS y lo va a pegar en 
la carpeta style.css).

ADVERTENCIA: Cuando ejecutes el comando tene cuidado porque como te digo va a compilar todo a css, es decir va a reemplazar todo lo que se encuentre en la carpeta "style.css",
cualquier cambio en los estilos que quieras hacer hacelo en sass para que no pierdas todo lo que estabas haciendo.

*Arregle los problemas de tipado del archivo footers, estaban mal escritos los atributos dentro de "color: nth(""""""""""""")"




+Quedaria agregarle una animacion a traves de sass y el trabajo de SEO+
+Se te va a hacer mas facil empezar con el trabajo de SEO, agregale algunas keywords y un favicon+
+Para la animacion no te puedo ayudar mucho ya que no sabria como realizar animacion en sass con map y nexting+
+Te recomiendo hacerlo normalmente como si lo hicieras en css pero en sass, ahi si te podria ayudar+

+SALUDOS+

PD: *Agregue las animaciones, vas a ver la carpeta de scss llamada "_animation.scss" en la carpeta de componentes. Son dos animaciones una simple barra de carga amarilla que vas 
a ver arriba de cada pagina y un hover que se va a activar cada vez que mantengas el cursor sobre el titulo de la pagina.
Revisando el HTML vas a encontrar en la primera parte del navbar un div con la clase "AnimacionDeCarga" es la clase que use para darle la animacion al div. Y ademas vas a encontrar dentro de las 
clases del titulo la clase "AnimacionDeTitulo". Podes revisar todas las animaciones en el archivo que te mencione antes ("_animation.scss").