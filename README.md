<img src='https://devjoseph.herokuapp.com/static/img/python-django.a07e0585.05de5d61e1a1.png'>

# Instalación de Django

Para empezar a desarrollar en Django, necesitaremos hacer algunas herramientas, así que procederemos a instalar lo siguiente:

1. Un editor de código
2. Instalar Python
3. Tener pip como manejador de paquetes (Suele venir al instalar Python)
4. Instalar extensión para Python

## 1. Instalar el editor de código
Este nos ayuda a tener un entorno de proyecto ordenado por cada archivo que tendremos. Suele utilizarse para diferentes lenguajes.

* <a href='https://www.youtube.com/watch?v=Hs49jA6FizM'>Video de instalación de Visual Studio Code en Windows</a>
* <a href='https://www.youtube.com/watch?v=eG27tmTfFFc'>Video de instalación de Visual Studio Code en Mac</a>

Una vez que tengas el editor de texto, podrás personalizarlo como tu quieras, esto es para comodidad a la hora de que estes desarrollando.

En la tienda de extensiones podrás encontrar:
* Temas para tu Visual que van desde claros y oscuros
* Iconos de visualización de archivos
* Extensiones de autocompletado de cada lenguaje
* Herramientas para servidores locales
* Mucho más

La personalización es a tu gusto y diferente a cada persona pero te recomiendo estos videos para ir iniciando, y con el tiempo, tú tendrás tus extensiones favoritas.

Recuerda, no necesitas instalar todo, solo lo que a ti te guste

* <a href='https://www.youtube.com/watch?v=RwL1IgzmM8Y&t=463s'>Personalización de Visual Studio Code (VSCode) para este 2021 - Configuración y Extensiones</a>
* <a href='https://www.youtube.com/watch?v=uLQkQG7fpS8'>Ponle EFECTO GLASS a tu EDITOR 😎 de CODIGO CON las sig. EXTENSIONES 🔨🔧 en Windows y Mac</a>

Algunos trucos
* <a href='https://www.youtube.com/watch?v=ZYSUN99taBo'>🏆Los 5 mejores TRUCOS [poco conocidos] para VSCODE usado por PROFESIONALES (2021)</a>

Y uno que si te recomiendo es el guardado automático, varia en cada programador y puedes desactivarlo cuando tu gustes.
<a href='https://www.youtube.com/watch?v=Dhkth0KW4hU'>Activar autoguardado Visual Studio</a>

## 2. Instalar Python
La instalación de python cambia dependiendo el sistema operativo.

### Instalar Python en Windows

<a href='https://www.youtube.com/watch?v=nXgxe3JM7Rc'>Video de instalación de Python en Windows</a>

### Instalar Python en Mac
Cuando utilizas un Sistema operativo basado en Unix, suele venir instalado una versión de python, solo que es una versión vieja (2.6) así que solo tendrás que actualizar a una versión más actual.

<a href='https://www.youtube.com/watch?v=_V21h27_rj8'>Video de instalación de Python en Mac</a>

### ¿Cómo saber que versión tengo?
Para visualizar que versión tenemos vamos a utilizar la consola/terminal 

#### En Windows

Para abrir la consola de windows, podemos buscar la palabra `cmd`en el buscador de windows y nos abrira una consola. 

En la consola colocaremos:
```Bash
py --version
```

#### En Mac
Le vamos a dar buscar y colocaremos `terminal` y abriremos la aplicación.

En la terminal colocaremos:
```Bash
python --version
```




## 3. Pip 
Para ver que ya tenemos pip, procederemos a ir a la consola/terminal como vimos en un paso anterior.

### Windows
```Bas
pip --version
```
### Mac
```Bas
pip3 --version
```
## 4. Instalar extensión para Python
En la parte de extensiones de Visual Code, vamos a buscar la correspondiente a `Python`. Estas extensiones suelen aparecer cuando incorporas un archivo de algún lenguaje y es recomendable instalarlas cuando nos preguntan. 

<img src='https://i.blogs.es/0e7a72/python-extension-marketplace/450_1000.png'>

---

## Introducción a Django

Ahora que ya contamos con nuestro editor de código, lo que haremos es crear la carpeta donde empezaremos a trabajar. 

### Moverse a la carpeta documentos

Vamos a tener una carpeta donde trabajaremos, así que crearemos una. 

La forma en que voy a crearla es desde la consola, ya que vamos a estar trabajando con un servidor y ese esta corriendo en la consola.

#### Paso 1: Abrir la consola o terminal y moverte a la carpeta documentos

Cuando abrimos nuestra terminal, nos abre siempre el  usuario que estamos en nuestra computadora.

##### Windows: 
```Bash
C:\usarios\yourUser>
```

y si colocas `dir` podrás observar la carpeta documentos, descargas, videos entre otras.

Para moverte a `Documentos` solo deberás teclear:

```Bash
C:\usarios\yourUser> cd Docu
```

y sin terminar la palabra, presiona la tecla `tabulador` para que se autocomplete y das enter.

Ahora debes estar en una ruta como:

```Bash
C:\usarios\yourUser\Documentos>
```

##### Mac:
Cuando abres la terminal, ese no te especifica tu posición en las carpetas ya que sale algo parecido a esto:
```Bash
yourUser@nameComputer ~ %
```

Pero al igual que Windows, estas posicionado en tu usuario, así que nos moveremos igual a la carpeta Documentos

```Bash
yourUser@nameComputer ~ % cd Docu
```

y sin terminar la palabra, presiona la tecla `tabulador` para que se autocomplete y das enter.

Ahora debes estar en una ruta como:

```Bash
yourUser@nameComputer Documents % 
```

### Paso 2: Crear una carpeta llamada proyecto

Para crear una carpeta, utilizaremos el comando `mkdir` y a lado el nombre del proyecto.

Ejemplo Windows:

```Bash
C:\usarios\yourUser\Documentos> mkdir tutorial
```

Ejemplo Mac:
```Bash
yourUser@nameComputer Documents % mkdir tutorial
```

Ahora que ya creamos la carpeta, accedemos a ella con `cd tutorial`

### Paso 3: Crear entorno virtual y descargar Django

Para esto vas a seguir el siguiente tutorial donde solo vas a hacer los pasos 2 y 3.

<a href='https://github.com/DanielCarmonaPhantom/Tutorial-Entornos-Virtuales-Python'>Tutorial Entornos Virtuales Python</a>

### Paso 4: Instalar Django

Vamos a instalar el framework de DJango 

En Windows, ejecuta:
```Bash
pip install django
```
En Unix o MacOS, ejecuta:
```Bash
pip3 install django
```

Ahora que tenemos django instalado, podremos utilizar el comando en la consola/terminal: `django-admi startproject`.

Este nos ayuda a crear el proyecto django y debemos especificar el nombre.

Este nombre del proyecto es general como Netflix, Instagram, Facebook. Es el nombre principal de tu proyecto

```Bash
django-admin startproject nombreProyecto
```

### Paso 5: Levantar servidor de Django

En Windows, ejecuta:
```Bash
py manage.py runserver
```
En Unix o MacOS, ejecuta:
```Bash
python3 manage.py runserver
```

Te dara un link de una url, copialo y pegalo en tu navegador y observaras el Hello World de Django.