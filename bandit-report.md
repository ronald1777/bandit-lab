**Level 0**
Objetivo:Encontrar la contraseña del siguiente nivel en el archivo readme.

\*\*Comandos utilizados:\*\*

```bash

ls

cat readme

```



Se listaron los archivos del directorio actual

con `ls` y se leyó el contenido del archivo

readme con `cat`.


Contraseña:

ZjLjTmM6FvvyRnrb2rfNWOZOTa6ip5If



**Level 1**
Objetivo: Leer el archivo llamado "-" que está en el directorio home.

Comandos utilizados:
```bash
cat ./-
```
El archivo se llama "-" que es un carácter especial.
Para leerlo, se usa `./- ` para indicar la ruta relativa.

Contraseña: 263JGJPfgU6LtdEvgfWU1XP5yac29mFx


**Level 2**
Objetivo: Leer un archivo que tiene espacios en su nombre.
Comandos utilizados:
```bash
ls
cat./ "--spaces in this filename--"
```
Para leer archivos con espacios en el nombre,
se usan comillas o se escapan los espacios con `\`.
Contraseña:MNk8KNH3Usiio41PRUEoDFPqfxLPlSmx


**Level 3**
Objetivo: Encontrar un archivo oculto dentro del directorio inhere.
Comandos utilizados:
```bash
   ls
   cd inhere
   ls -la
   cat ...Hiding-From-You
```
Se navegó al directorio `inhere` y se usó `ls -la` para mostrar archivos ocultos.
El archivo se llamaba `...Hiding-From-You` (con tres puntos al inicio).
Contraseña: 2WmrDFRmJIq3IPxneAaMGhap0pFhF3NJ

**Level 4**
Objetivo: Encontrar el único archivo legible por humanos entre varios archivos en el directorio inhere.
   Comandos utilizados:
```bash
   ls
   cd inhere
   ls
   file ./-file*
   cat ./-file07
```
   Se usó el comando `file` con wildcard `*` para identificar el tipo de cada archivo, después de intentar leerlos uno a uno.
   Al finall archivo `-file07` era el único con formato "ASCII text"
   (texto legible por humanos). Se usó `./` antes del nombre porque empieza con guión.
   Contraseña:4oQYVPkxZOOEOO5pTW81FB8j8lxXGUQw

   **Level 5**
   Objetivo: Encontrar un archivo con características específicas: 
   -tamaño 1033 bytes
   -no ejecutable
   -legible por humanos.

   Comandos utilizados:
```bash
ls
cd inhere
find . -type f -size 1033c ! -executable
cat ./maybehere07/.file2
```
Se usó el comando `find` con filtros: `-type f` (archivo regular),
`-size 1033c` (1033 bytes), `! -executable` (no ejecutable).
Contraseña: HWasnPhtq9AVKe0dmk45nxy20cvUa6EG







