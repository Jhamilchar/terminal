Resumen Sobre la shell o terminal de linux 

Caminando en la terminal:

Para poder caminar con la terminal iremos explorando como con un (ls) que vendria a ser para listar una carpeta dentro o un (ls -l) siendo lo mismo pero la diferencia que es un tipo de listado mas largo con detalles añadidos comotamaño de bits pero una mejor un comando legible para los humanos vendria a ser un 
(ls -lh), y para poder movernos entre carpetas usamos (cd) que es un "change directory" muy usado en la terminal.

Un pequeño truco para no escribir todo el comando que ya usaste simplemtente lo haces con una flecha para arriba o abajo 

Cuando estes perdido en la terminal o no sabes donde ubicarte es tam simple como escribir (pwd) lo cual te mostrara la ruta del directorio, o usar los puntos despues de un "cd" siendo que un punto (cd .) te ubicara en la misma carpeta (cd ..) pero con 2 puntos te enviara a una directorio anterior y con estos comandos podras moverte facilmente desde la terminal

Manipulando archivos:

Siendo "ls" un comando util y muy usado este tiene interesantes variaciones como, (ls -ls) Lo cual ordena por tamaño de directorios o carpetas, (ls -lr) ordena de reversa

y viendo un arbol general con (tree) pero al hacerlo podria ser muy dificil de entenderlo y para esto existe la posibilidad de tener niveles como (tree -L 2) de esta forma solo te mostrara hasta que nivel mostrarte y lo que necesitas.

La forma ideal para crear un directorio es el comando (mkdir) o un (touch) para crear archivos desde la terminal y para poder renombrar podemos usar (mv [nombre_antiguo] [nombre_nuevo]) o para borrar algun archivo o directorio.

para borrar un directorio se usa (rm -r [nombre]) o para borrar un archivo usamos (rm [nombre]) PERO EL MEJOR COMANDO PARA HACER ESTO ES AGREGARLE UNA "i" 
(rm -ri [nombre]) de esta manera preguntara antes de borrarlo por si ocurre un error y perder los datos de todo tu trabajo.

Que es un comando?

//Es un programa ejecutable
//Comando de utilidad de la shell
//Una funcion de shell
//un alias

Dicho esto exploraremos contenido de nuestros archivos
Con el comando (help cd) presionando con doble tab mostara caracteristicas generales de los comandos 
Y con el comando (type [nombre del comando]) Muestra que tipo de comando es 

Muchos comandos son dificiles de acordarse pero pudemos usar un "alias" en la shell de la siguiente forma (l="ls -lh") aunque este alias es momentanea 

Wildcards

Nos permite encontrar patrones o realizar busquedas mas avanzadas con el comando (ls) agregando caracteres especiales dentro de la shell 

(ls *.[extension]) lista los elementos que terminen con la misma extension como "doc.html, text.html"
(ls [nombre]*) lista los elementos con el nombre que compartan al principio y los caracteres posteriormente "datos1, datos123"
(ls [nombre]?) lista los elementos con el nombre que compartan al principio y solo un caracter "datos1" {PUNTO IMPORTANTE ES QUE EL SIGNO DE INTERRAGION SUELE MEDIR LOS CARACTERES QUE BUSCAS}
(ls -d [[:upper:]]*) Lista los elementos de mayusculas
(ls -d [[:lower:]]*) Lista los elementos de minusculas
(ls [iniciales de las letras que queremos que busque]*)


Redirecciona cómo funciona la shell

Todo empieza desde el teclado (STDN) que vendria a ser el teclado y al usar un comando antes que te envie el resultado que se necesita esto tiene 2 opciones (STOUT) que muestra los resultados o (STDERR) que muestra si hubo un error posteriormente lo imprime el la pantalla "DENTRO DE TODO ESTO EL STOUT TIENE EL CODIGO 1, Y EL STDERR TIENE EL CODIGO 2 (FILE DESCRIPTION)" 

Para redirigir un archivo esta es la manera "ls [carpeta] > [misarchivos.txt]" posteriormente verlo con "less [archivo]"  
Pero para visualizar el error necesitamos escribir lo siguiente (ls [cualquier cosa] 2> error.txt) de esta manera visualziando con el comando (head error.txt), imprimira el error






