Modulo 0

2. Comandos básicos Linux
¿Qué es un terminal?
La terminal (también conocida como consola, terminal o símbolo del sistema) es una forma generalizada de llamar a la interfaz de usuario de línea de comandos: una pantalla (generalmente, de color de fondo negro sobre letras blancas) donde escribiendo comandos (secuencias de palabras especiales) ordenamos al sistema realizar acciones concretas.

La línea de comandos es una aplicación en la que puedes escribir y ejecutar comandos para realizar tareas como:

Navegar por las carpetas de tu computador.
Manipular archivos (crear, editar, copiar, mover y eliminar).
Conectarte a servidores remotos.
Crear scripts que te ayuden con tus tareas diarias.

Comandos
-¿En qué carpeta estoy? (pwd)
En la línea de comandos siempre vas a estar ubicado(a) sobre una ruta (carpeta) de tu sistema. Para conocer la ruta actual podemos utilizar el comando pwd (print work directory)
Nota: ¡No olvides el Enter al final de cada comando para ejecutarlo!
-Listar ficheros (ls)
Para ver los ficheros y carpetas del directorio actual, basta con utilizar el comando ls (LiSt files). Esto mostrará una lista en horizontal con todos los ficheros y carpetas encontradas.
-Cambiar de carpetas (cd)
Para movernos entre carpetas, utilizaremos el comando cd (change directory) seguido del nombre de la carpeta (movimiento relativo) o ruta completa (movimiento absoluto) a la que queremos acceder. Ten en cuenta que, al escribir el nombre de la carpeta o ruta, puedes pulsar TAB y el sistema te sugiere las opciones que encajen con lo que has escrito (o autocompleta si solo hay una opción), de modo que no tendrás que escribirlo por completo. Por ejemplo, si quieres ir a la carpeta raíz de tu sistema debes escribir: cd /

Resumen de comandos:
pwd Me permite conocer la ruta actual (Donde estoy ubicado).
ls ver los elementos de la carpeta donde estoy ubicado.
clear Limpiar la pantalla.
ls -la Ver detalle de la información con los permisos que tienen esos recursos.
mkdir crear un directorio.
rm – rf [nombre directorio]: Borrar de forma forzosa el recurso.
cd [carpeta]: dirigirme a una carpeta deseada.
cd .. devolverme a una ruta o carpeta anterior.
touch [NombreNuevoArchivo] : crear un archivo de cualquier tipo distinto a una carpeta.
nano [NombreNuevoArchivo] : Crear un archivo.

3. Instrucciones básicas de git
Un Sistema de Control de Versiones (SCV) es una aplicación que permite gestionar los cambios que se realizan sobre los elementos de un proyecto o repositorio, guardando así versiones del mismo en todas sus fases de desarrollo
¿Qué es Git?
Git es un sistema de control de versiones de código abierto ideado por Linus Torvalds (el padre del sistema operativo Linux) y actualmente es el sistema de control de versiones más extendido. A diferencia de otros SCV Git tiene una arquitectura distribuida lo que significa que en lugar de guardar todos los cambios de un proyecto en un único sitio, cada usuario contiene una copia del repositorio con el historial de cambios completo del proyecto Esto aumenta significativamente su rendimiento.
¿Qué es GitHub?
GitHub es una plataforma que permite a los usuarios socializar con personas de ideas afines. Puedes seguir a las personas y ver qué hacen o con quién se conectan

Primeros pasos:
Lo primero que debes hacer después de que has instalado git es configurar el nombre y correo que se va a utilizar para firmar cada commit que hagas. Utiliza los comandos

git config --global user.name "FirstName LastName"
git config --global user.email "email@example.com" validar la información de configuracion git config --global -e "email@example.com"

Por ejemplo, si tu nombre fuera "Simon Cano" utilizarías el siguiente comando: git config --global user.name "Simon Cano"
Y asumiendo que el correo es "simon@gmail.com" utilizarías el siguiente comando:
git config --global user.email "simon@example.com" Correo de la cuenta de git

Trabajando en un proyecto
El flujo de trabajo más simple con git es el siguiente:
Inicializa el repositorio (esto va a crear una carpeta oculta. git dentro del proyecto): git init
Trabaja en el código: crea, modifica y elimina archivos. Por ejemplo, vamos a construir una página web en donde necesitamos un archivo index.html, un archivo index.js y un archivo style.css
Prepara los cambios que vas a incluir en el siguiente commit. Para incluir todos los cambios utiliza: git add ." Para agregar todos los archivos
git add -A Para agregar todos los archivos, esta es otra de incluir los archivos
git add <nombreArchivo> Para agregar solo un archivo
Crea el commit: git commit -m 'El mensaje que describe los cambios'
Repite los pasos 2, 3 y 4 cada vez que realices un cambio en tu proyecto.
Vincular con un repositorio
En GitHub crear un repositorio con el nombre de tu proyecto
El repositorio debe ir vacio para este ejemplo (Sin Readme, sin licencias, entro otros)
Agregar la url del repositorio por medio del siguiente comando: git remote add origin <url repositorio>
Entregar los cambios git push origin <Raman main>
Resumen de los comandos más importantes
git config --global user.name <name> : define el nombre que se va a utilizar en los commits de forma global (para el usuario actual).
git config --global user.email <email> : define el correo electrónico que se va a utilizar en los commits de forma global (para el usuario actual).
git config --global -e : comando para verificar la información de la configuración
git init : este comando se encarga de iniciar el repositorio (esto va a crear una carpeta oculta .git en la carpeta donde ejecutes este comando).
git add . : prepara los archivos para el commit .
git commit -m <descripción de los cambios> : crea un commit a partir de los cambios que están en el index con el mensaje que se le pase a la opción -m .
git status : muestra la lista de archivos con cambios desde el último commit y los que van a ser incluídos en el siguiente commit.
git remote add origin <url repositorio> : Indicar la dirección del repositorio
git push origin <Raman main> : Entregar los cambios
git pull origin <Raman main> : Bajar los cambios

4. Instrucciones básicas MarkDown
## Título
### Subtítulo
Este es un ejemplo de texto que da entrada a una lista genérica de elementos:

- Elemento 1
- Elemento 2
- Elemento 3

Este es un ejemplo de texto que da entrada a una lista numerada:

1. Elemento 1
2. Elemento 2
3. Elemento 3

Al texto en Markdown puedes añadirle formato como **negrita** o *cursiva* de una manera muy sencilla.
Encabezados
H1
H2
H3
H4
H5
H6

Cursiva

MarkDown	Resultado
*cursiva*	cursiva
_cursiva_	cursiva
**negrita**	negrita
__negrita__	negrita

Videos
Las etiquetas de imagen que se vinculan a archivos con una extensión de video se convierten automáticamente en un reproductor de video. Las extensiones de vídeo válidas son .mp4, .m4v, .mov, .webm, y .ogv: Sample Video

Listas de tareas
Para crear una lista de tareas, introduce los elementos de la lista con un caracter de espacio regular, seguido de [ ]. Para marcar una tarea como completada, utiliza [x].

 Finish my changes
 Push my commits to GitHub
 Open a pull reques
Resaltar sintaxis de código Puedes agregar un identificador opcional de idioma para habilitar el resaltado de la sintaxis en tu bloque de código cercado.

Por ejemplo, para resaltar la sintaxis del código Ruby:
| ```lenguaje <codigo> ```| codigo |
Ejemplo;
|```ruby require 'redcarpet' markdown = Redcarpet.new("Hello World!") puts markdown.to_html puts markdown.to_html```|

require 'redcarpet'
markdown = Redcarpet.new("Hello World!")
puts markdown.to_html
puts markdown.to_html
# Valentina-Rojas
