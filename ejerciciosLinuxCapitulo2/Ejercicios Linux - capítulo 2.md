# Ejercicios Linux - capítulo 2

[TOC]



## Comandos utilizados:

- cd
- ls
- mkdir
- pwd

## Estructura de carpetas de Linux

A continuación se muestra una tabla con las direcciones mas importantes de un sistema Linux: 

![image-20250924100404546](./Ejercicios Linux - capítulo 2.assets/image-20250924100404546.png)

## Ejercicios

##### 1 - ¿En qué directorio se encuentran los ficheros de configuración del sistema?

​	Se encuentran en el directorio etc. `cliente@clienteUbuntu:/etc`

##### 2 - Para entrar en un sistema Linux hace falta a) nombre de usuario, contraseña y dirección IP, b) nombre de usuario y contraseña o c) únicamente una contraseña..

​	b) nombre de usuario y contraseña

##### 3 - Muestra el contenido del directorio actual

```bash
$ ls
```

![image-20250924100243283](./Ejercicios Linux - capítulo 2.assets/image-20250924100243283.png)

##### 4 - Muestra el contenido del directorio que está justo a un nivel superior. 

```bash
$ ls ..
```

![image-20250924102217437](./Ejercicios Linux - capítulo 2.assets/image-20250924102217437.png)

##### 5 - ¿En qué día de la semana naciste?, utiliza la instrucción `cal` para averiguarlo

```bash
$ cal 12 1995
```

​	Con esto obtengo el mes de mi nacimiento y observo que el día 16 es 		sábado.

![image-20250924103040683](./Ejercicios Linux - capítulo 2.assets/image-20250924103040683.png)

##### 6 - Muestra los archivos del directorio /bin

```bash
$ cd bin
```

​	Depende de en que lugar nos encontremos, habrá que hacer `cd ..` hasta 	llegar a la raíz (también hay otras formas) y luego ejecutar el `cd bin`.

![image-20250924103401036](./Ejercicios Linux - capítulo 2.assets/image-20250924103401036.png)

##### 7 - Suponiendo que te encuentras en tu directorio personal (`/home/nombre`), muestra un listado del contenido de `/usr/bin` 

##### 	a) con una sola línea de comando,

```bash
$ cd /bin
```

![image-20250924104016338](./Ejercicios Linux - capítulo 2.assets/image-20250924104016338.png)

##### 	b) moviéndote paso a paso por los directorios y 

```bash
$ cd ..
$ cd ..
$ cd bin
```

![image-20250924104121267](./Ejercicios Linux - capítulo 2.assets/image-20250924104121267.png)

##### 	c) con dos líneas de comandos.

```bash
$ cd /
$ cd bin
```

![image-20250924104214114](./Ejercicios Linux - capítulo 2.assets/image-20250924104214114.png)

##### 8 - Muestra todos los archivos que hay en `/etc` y todos los que hay dentro de cada subdirectorio, de forma recursiva (con un solo comando).

```bash
$ ls -R /etc
```

![image-20250924105839951](./Ejercicios Linux - capítulo 2.assets/image-20250924105839951.png)

##### 9 - Muestra todos los archivos del directorio `/usr/X11R6/bin` ordenados por tamaño (de mayor a menor). Sólo debe aparecer el nombre de cada fichero, sin ninguna otra información adicional.

```bash
$ ls -S /usr/X11R6/bin
```

![image-20250926105527092](./Ejercicios Linux - capítulo 2.assets/image-20250926105527092.png)

![image-20250926105559138](./Ejercicios Linux - capítulo 2.assets/image-20250926105559138.png)

##### 10 - Muestra todos los archivos del directorio `/etc` ordenados por tamaño (de mayor a menor) junto con el resto de características, es decir, permisos, tamaño, fechas de la última modificación, etc. El tamaño de cada fichero debe aparecer en un formato “legible”, o sea, expresado en Kb, Mb, etc.

```bash
$ ls -Slh /etc
```

![image-20250926111120929](./Ejercicios Linux - capítulo 2.assets/image-20250926111120929.png)

##### 11 - Muestra todos los archivos del directorio `/bin` ordenados por tamaño (de menor a mayor). Sólo debe aparecer el tamaño y el nombre de cada fichero, sin ninguna otra información adicional. El tamaño de cada fichero debe aparecer en un formato “legible”, o sea, expresado en Kb, Mb, etc.

```bash
$ ls -Sshr /bin
```

![image-20250926111503513](./Ejercicios Linux - capítulo 2.assets/image-20250926111503513.png)

##### 12 - Muestra el contenido del directorio raíz utilizando como argumento de `ls` una ruta absoluta.

```bash
$ ls /
```

![image-20250926111654924](./Ejercicios Linux - capítulo 2.assets/image-20250926111654924.png)

##### 13 - Muestra el contenido del directorio raíz utilizando como argumento de `ls` una ruta relativa. Suponemos que el directorio actual es `/home/elena/documentos`.

```bash
$ cd..
$ cd..
$ cd ..
$ ls
```

O

```bash
$ ls ../../..
```

![image-20250926120540425](./Ejercicios Linux - capítulo 2.assets/image-20250926120540425.png)

##### 14 - Crea el directorio `gastos` dentro del directorio personal.

```bash
$ mkdir gastos
```

![image-20250926120859401](./Ejercicios Linux - capítulo 2.assets/image-20250926120859401.png)

##### 15 - ¿Qué sucede si se intenta crear un directorio dentro de `/etc?`

​		Nos dice que no tenemos permisos.

![image-20250926121630131](./Ejercicios Linux - capítulo 2.assets/image-20250926121630131.png)

##### 16 - Muestra el contenido del fichero `/etc/fstab`

```bash
$ cat /etc/fstab
```

![image-20250926121938997](./Ejercicios Linux - capítulo 2.assets/image-20250926121938997.png)

##### 17 - Muestra las 10 primeras líneas del fichero `/etc/bash.bashrc`

```bash
$ head /etc/bash.bashrc
```

![image-20250926122716523](./Ejercicios Linux - capítulo 2.assets/image-20250926122716523.png)

##### 18 - Crea la siguiente estructura de directorios dentro del directorio de trabajo personal:

![image-20250926103938774](./Ejercicios Linux - capítulo 2.assets/image-20250926103938774.png)

```bash
$ mkdir multimedia
$ cd multimedia
$ mkdir musica
$ mkdir imagenes
$ mkdir video
$ mkdir presentaciones
$ cd imagenes
$ mkdir personales
$ mkdir otras
```

![image-20250926123040673](./Ejercicios Linux - capítulo 2.assets/image-20250926123040673.png)

##### 19 - Crea un fichero vacío dentro del directorio `musica`, con nombre `estilos_favoritos.txt`

```bash
$ touch estilos_favoritos.txt
```

![image-20250926123710722](./Ejercicios Linux - capítulo 2.assets/image-20250926123710722.png)

##### 20 - Utiliza tu editor preferido para abrir el fichero `estilos_favoritos.txt` e introduce los estilos de música que más te gusten. Guarda los cambios y sal.

```bash
$ vi estilos_favoritos.txt
rock
pop
rock-pop
jass
blues	
:q (para guargar)
:w (para salir)
```

![image-20250926124923548](./Ejercicios Linux - capítulo 2.assets/image-20250926124923548.png)

##### 21 - Muestra todo el contenido de `estilos_favoritos.txt`



##### 22 - Muestra las 3 primeras líneas de `estilos_favoritos.txt`



##### 23 - Muestra la última línea de `estilos_favoritos.txt`



##### 24 - Muestra todo el contenido del `fichero estilos_favoritos.txt` excepto la primera línea. Se supone que no sabemos de antemano el número de líneas del fichero.
