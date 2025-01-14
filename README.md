
![TandemCodeWeb](docs/assets/images/tarjetalogo.svg)

# Script-Tease Group page. Awesome-profile-Cards.

## Introducción.
En este proyecto el cliente nos pidió realizar una aplicacion web para crear tarjetas de visita virtuales.
Las tarjetas se deben poder personalizar en cuanto a colores, imagen y enlaces.
La aplicación tiene dos páginas, una con el landing de la aplicación, que contiene el nombre y un pequeño resumen de su funcionalidad y una segunda página donde podemos acceder a la personalización y creación de la tarjeta.

## Tecnologías usadas.

En esta primera aproximación hemos realizado la estructura de la página (con HTML5) de las dos páginas, basándonos en una aproximación movil-first. Le hemos añadido estilos usando sass.

Y le hemos añadido las funcionalidades básicas en JavaScript.

## Funcionalidades añadidas.

Entre estas funcionalidades podemos resaltar:

  - Cambios en los input se reflejen automaticamente en la previsualización de la tarjeta.
  - Los iconos a las redes sociales solo aparecen si rellenamos el campo adecuado.
  - Estos iconos aparecen en el orden en que son escritos, si hemos rellenado los datos el orden resultante es el indicado por el cliente.
  - Solo será visible una fase de la personalización en cada momento, cuando desplegamos una de ellas las demás se colapsan automaticamente.

En la siguiente etapa del proyecto nos enfocaremos en desarrollar el resto de funcionalidades solicitadas por el cliente.


Para este proyecto hemos usado este starter kit de adalab.


## Adalab web starter kit

Ahoy! Esta es nuestro Starter Kit en node/gulp para este primer contacto con el desarrollo web
Incluye SCSS, un sistema de plantillas HTMl y un web server.

## Guía de inicio rápido
Necesitarás instalar [Node.js](https://nodejs.org/) y [Gulp](https://gulpjs.com) para trabajar con este Starter Kit, luego:
1. Descarga o clona el repositorio
2. Instala las dependencias locales con `$ npm install`
3. Arranca el kit con `$ gulp`

## Espera, ¿esto se hace siempre?
> ### Solo una vez al principio en cada ordenador que utilicemos:
- Instalamos node
- Instalamos el comando de gulp de forma global para poder usarlo desde cualquier carpeta usando `npm install --global gulp-cli`

> ### Cada vez que descarguemos o clonemos un repo:
- `npm install` para instalar los paquetes necesarios para convertir Sass a CSS, minizarlo, etc.

> ### Cada vez que estemos trabajando con nuestro código:
- Desde nuestra terminal, ejecutamos el comando `gulp` para que realice la tarea por defecto, que en el caso del `gulpfile.js` que tenemos en adalab-web-starter-kit estará pendiente de nuestros archivos Sass, html y JavaScript y los compilará, minificará y/o recargará el servidor cada vez que hagamos un cambio

## Tareas de gulp incluidas
### Inicio de un web server para desarrollo
```
$ gulp
```
Lanza un webserver con BrowserSync y varios watchers estarán pendientes de los archivos SCSS/JS/HTML, en la carpeta **public/**, para recargar el navegador cuando se necesite.

### Versión lista para subir a producción
```
$ gulp docs
```
En la carpeta **docs/** genera los CSS y JS minimizados y sin sourcemaps listos para subir al repo y activar GitHub Pages en `master/docs`.


## Estructura del proyecto
Nuestro **gulpfile.js** usa un JSON de configuración con las rutas de los archivos a generar/vigilar.

La estructura de carpetas tiene esta pinta:
```
/
`- _src
   |- assets
   |  |- icons
   |  |- images
   |  |- js
   |  `- scss
   |     `- core
   |
   `- templates
      `- partials

```

## HTML
Viene incluído el paquete [**gulp-html-partial**](https://www.npmjs.com/package/gulp-html-partial) que nos va a permitir tener un sistema de plantillas html

## Imágenes e iconos
Tenemos en **_src/** una carpeta para las imágenes del proyecto y una para los iconos como el favicon o los iconos de dispositivos móviles. Estos últimos se generan en la raíz de las carpetas **public/** y **docs/**

## CSS
Viene incluído el paquete [**gulp-combine-mq**](https://www.npmjs.com/package/gulp-combine-mq) que agrupa todas las mediaqueries al final del documento css.

## JS
Podemos usar parciales de JS: en el JSON de configuración, **config.json** especificamos los archivos JS que utilizamos y en el orden que deben procesarse.

## ¿Cómo actualizo si tengo una versión anterior?
En principio puedes descargar todos los archivos fuera de **_src/** y sustituir los de tu proyecto. Además deberías replicar la estructura de carpetas dentro de **_src/**.

## Falta algo?
Echas de menos que el kit haga algo en concreto? Pidelo sin problema a través de los Issues o si te animas a mejorarlo mándanos un PR :)
