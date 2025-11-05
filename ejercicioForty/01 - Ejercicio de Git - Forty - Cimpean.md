# 01 - Ejercicio de Git - Forty - local y remoto

> Módulo: Despliegue de Aplicaciones 
>
> Web Profesora: Inés Menéndez
>
> Alumno: Cimpean Gabriel

[TOC]

## Trabajo en local

#### 1. Inicializa un nuevo repositorio Git en una carpeta llamada "`forty`" y agrega los archivos proporcionados en el aula virtual. 

![image-20251105095845644](C:\Users\2dawd05\AppData\Roaming\Typora\typora-user-images\image-20251105095845644.png)

#### 2. Renombra la rama master a `main`. 

![image-20251105100002182](C:\Users\2dawd05\AppData\Roaming\Typora\typora-user-images\image-20251105100002182.png)

#### 3. Haz que los ficheros `README.txt` , `LICENSE.txt` y `passwords.txt` sean ignorados por el control de versiones.

![image-20251105100115030](C:\Users\2dawd05\AppData\Roaming\Typora\typora-user-images\image-20251105100115030.png)

#### 4. Crea el archivo `passwords.txt` . Comprueba que el control de versiones lo ignora.

 ![image-20251105102016097](C:\Users\2dawd05\AppData\Roaming\Typora\typora-user-images\image-20251105102016097.png)

#### 5. Crea una rama llamada "`feature-content`" . Muévete a esa rama. Cambia, en la línea 3477, el `font-size` por `1.5em` en el archivo `main.css` . Confirma cambios y haz commit. Muestra los logs de la forma más gráfica posible. 

![image-20251105102708672](C:\Users\2dawd05\AppData\Roaming\Typora\typora-user-images\image-20251105102708672.png)

![image-20251105102613413](C:\Users\2dawd05\AppData\Roaming\Typora\typora-user-images\image-20251105102613413.png)

![image-20251105102859271](C:\Users\2dawd05\AppData\Roaming\Typora\typora-user-images\image-20251105102859271.png)

#### 6. Elimina el archivo "`passwords.txt`" en la carpeta `forty` . Verifica el estado del repositorio. ¿Hay cambios pendientes? 

![image-20251105103041412](./01 - Ejercicio de Git - Forty - Cimpean.assets/image-20251105103041412.png)

#### 7. Crea un nuevo archivo llamado " `about.html` ", partiendo del archivo `generic.html` y agrégalo al repositorio, haz un nuevo commit. 

![image-20251105103302095](./01 - Ejercicio de Git - Forty - Cimpean.assets/image-20251105103302095.png)

#### 8. Cambia a la rama `main` . Examina los logs del repositorio de forma gráfica. 

![image-20251105103604174](./01 - Ejercicio de Git - Forty - Cimpean.assets/image-20251105103604174.png)

#### 9. Modifica algo en el archivo `generic.html` , comprueba que hay cambios, y realiza otro commit . Examina los logs del repositorio de forma gráfica. 

![image-20251105103751979](./01 - Ejercicio de Git - Forty - Cimpean.assets/image-20251105103751979.png)

#### 10. Modifica algo en el fichero `elements.html` . Confirma los cambios, pero no hagas commit. 

![image-20251105103852022](./01 - Ejercicio de Git - Forty - Cimpean.assets/image-20251105103852022.png)

#### 11. Mira las diferencias de `elements.html` . Los cambios no nos gustan, deshaz los cambios de `elements.html` . Comprueba que no hay cambios pendientes. 

![image-20251105104003318](./01 - Ejercicio de Git - Forty - Cimpean.assets/image-20251105104003318.png)

#### 12. Muestra las diferencias entre dos ramas.

 ![image-20251105104135347](./01 - Ejercicio de Git - Forty - Cimpean.assets/image-20251105104135347.png)

#### 13. Fusiona la rama "`feature-content`" con la rama principal (main). Muestra los logs del repositorio de una forma gráfica y completa. 

![image-20251105104411813](./01 - Ejercicio de Git - Forty - Cimpean.assets/image-20251105104411813.png)

#### 14. Crea una nueva rama llamada " `hotfix` " y en ella, corrige un error crítico en el archivo " `index.html` ". (Por ejemplo, añade el enlace a la nueva página about.html) 

![image-20251105104613665](./01 - Ejercicio de Git - Forty - Cimpean.assets/image-20251105104613665.png)

#### 15. Fusiona la rama "`hotfix`" con la rama principal y verifica el historial de commits de forma que se vean todas las ramas gráficamente. ¿Borrarías la rama `hotfix` ? ¿En qué caso? ¿Cómo? 

![image-20251105104713841](./01 - Ejercicio de Git - Forty - Cimpean.assets/image-20251105104713841.png)

Lo borraría en caso de que no se utilice mas mediante `git branch -d hotfix`.

#### 16. Muestra el historial de cambios limitado a los últimos 3 commits. 

![image-20251105105112219](./01 - Ejercicio de Git - Forty - Cimpean.assets/image-20251105105112219.png)

#### 17. Etiqueta el commit actual como "v1.0" y muestra las etiquetas existentes.

![image-20251105105213437](./01 - Ejercicio de Git - Forty - Cimpean.assets/image-20251105105213437.png)



## Trabajo en remoto

#### 1. Sube al remoto los ficheros de tu repositorio local.

![image-20251105110724052](./01 - Ejercicio de Git - Forty - Cimpean.assets/image-20251105110724052.png)

#### 2. En local, crea una rama 'feature-head'. Cambia el título en la sección head de index.html , borra los comentarios del head , o previos, también. Confirma y sube los cambios al remoto. 

![image-20251105111601942](./01 - Ejercicio de Git - Forty - Cimpean.assets/image-20251105111601942.png)

#### 3. En remoto, crea una rama 'feature-articulo'. Duplica la página generic , nómbrala como articulo.html , y añade como contenido un artículo sobre Git. Confirma los cambios y realiza un commit. Muestra los commits del repositorio tal como se ven en GitHub. 

![image-20251105112528217](./01 - Ejercicio de Git - Forty - Cimpean.assets/image-20251105112528217.png)

![image-20251105112716853](./01 - Ejercicio de Git - Forty - Cimpean.assets/image-20251105112716853.png)

#### 4. En el repositorio local examina los cambios. Actualiza el repositorio con el remoto. Fusiona en 'main' las dos ramas 'feature'. Crea la etiqueta 'v2.0'. Muestra los logs, commits, etiquetas y ramas actuales, en local y en remoto.

#### ![image-20251105112943722](./01 - Ejercicio de Git - Forty - Cimpean.assets/image-20251105112943722.png) 

![image-20251105112957712](./01 - Ejercicio de Git - Forty - Cimpean.assets/image-20251105112957712.png)

![image-20251105113011132](./01 - Ejercicio de Git - Forty - Cimpean.assets/image-20251105113011132.png)

![image-20251105113024712](./01 - Ejercicio de Git - Forty - Cimpean.assets/image-20251105113024712.png)

![image-20251105113144477](./01 - Ejercicio de Git - Forty - Cimpean.assets/image-20251105113144477.png)

![image-20251105113219683](./01 - Ejercicio de Git - Forty - Cimpean.assets/image-20251105113219683.png)

![image-20251105113329667](./01 - Ejercicio de Git - Forty - Cimpean.assets/image-20251105113329667.png)

#### 5. En tu copia local, crea una rama nueva . En la rama nueva, cambia los enlaces de la página index.html para que apunten correctamente a la nueva página articulo.html . Confirma los cambios. 

![image-20251105113558997](./01 - Ejercicio de Git - Forty - Cimpean.assets/image-20251105113558997.png)

![image-20251105113709314](./01 - Ejercicio de Git - Forty - Cimpean.assets/image-20251105113709314.png)

#### 6. Muestra los logs de forma que se vean las ramas en tu copia local. 

![image-20251105113856459](./01 - Ejercicio de Git - Forty - Cimpean.assets/image-20251105113856459.png)

#### 7. Te gusta el resultado de los cambios. Incorpora los cambios de la rama nueva a la principal. 

![image-20251105114017228](./01 - Ejercicio de Git - Forty - Cimpean.assets/image-20251105114017228.png)

#### 8. Sube los cambios al remoto borrando la rama nueva , si es necesario. Comprueba primero con un comando en local, las ramas que hay en el repositorio remoto. 

![image-20251105114136145](./01 - Ejercicio de Git - Forty - Cimpean.assets/image-20251105114136145.png)

![image-20251105114151089](./01 - Ejercicio de Git - Forty - Cimpean.assets/image-20251105114151089.png)

![image-20251105114213880](./01 - Ejercicio de Git - Forty - Cimpean.assets/image-20251105114213880.png)

![image-20251105114228793](./01 - Ejercicio de Git - Forty - Cimpean.assets/image-20251105114228793.png)

#### 9. Muestra en local los cambios en el archivo index.html entre la versión actual y la anterior. 

![image-20251105114319361](./01 - Ejercicio de Git - Forty - Cimpean.assets/image-20251105114319361.png)

#### 10. En el repositorio en GitHub, navega hasta el archivo index.html y selecciona la opción "History".

![image-20251105114433608](./01 - Ejercicio de Git - Forty - Cimpean.assets/image-20251105114433608.png)