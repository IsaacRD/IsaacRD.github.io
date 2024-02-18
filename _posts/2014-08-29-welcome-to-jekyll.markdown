---
layout: post
title:  "Permisos de un archivo en Linux"
date:   2024-02-18 23:45:00
categories: mediator normal
tags: normal
image: /assets/article_images/2014-11-30-mediator_features/night-track.JPG
image2: /assets/article_images/2014-11-30-mediator_features/night-track-mobile.JPG
---
>En Linux, los permisos de archivos y directorios se gestionan mediante un sistema octal de tres dígitos, donde cada dígito representa un conjunto de permisos específico para el propietario, el grupo y otros. Cada conjunto de permisos se representa con un número entre 0 y 7. Aquí están los permisos posibles:

Read (r) - Lectura:

Representado por el bit 4.
Permite al usuario leer el contenido del archivo o ver el contenido del directorio.
Write (w) - Escritura:

Representado por el bit 2.
Permite al usuario modificar o eliminar el archivo, o agregar, eliminar o renombrar archivos en un directorio.
Execute (x) - Ejecución:

Representado por el bit 1.
Para archivos: permite al usuario ejecutar el archivo si es un programa o guion.
Para directorios: permite al usuario entrar (navegar) en el directorio.
Estos permisos se asignan a tres categorías de usuarios:

Propietario (owner): El usuario que creó el archivo o directorio.
Grupo (group): El grupo al que pertenece el archivo o directorio.
Otros (others): Todos los demás usuarios.
Ahora, los números en el sistema octal representan la combinación de permisos. Cada dígito representa la suma de los permisos correspondientes:

4: Lectura (r)
2: Escritura (w)
1: Ejecución (x)
Ejemplos de combinaciones de permisos:

0 (---): Sin permisos (ni lectura, ni escritura, ni ejecución).
1 (--x): Ejecución solamente.
2 (-w-): Escritura solamente.
3 (-wx): Escritura y ejecución.
4 (r--): Lectura solamente.
5 (r-x): Lectura y ejecución.
6 (rw-): Lectura y escritura.
7 (rwx): Lectura, escritura y ejecución.

>Por ejemplo, si ves chmod 755 archivo.txt, significa que el propietario tiene permisos de lectura, escritura y ejecución (7), mientras que el grupo y otros tienen permisos de solo lectura y ejecución (5).

#Ciberseguridad 
#Pentesting 
#SeguridadInformatica