![logo-u]

##![Undefined] PROYECTO MODULO 2 EQUIPO 5 ADALAB
**My proffesional card: proyecto incubadora JavaScript (JS)**

**My proffesional card 📺 es un proyecto sencillo en equipo de de desarrollo de una aplicación web que nos permite crear una tarjeta de visita profesional personalizada. Te permite introducir tus datos profesionales y de contacto, tu foto y guardarlo en local storage.**

Comenzando 🚀 Para utilizarla solo necesitas cargar el enlace y....tendrás tu tarjeta profesional un clic de distancia.

Construido con 🛠️ JavaScript (JS), HTML5 y CSS3. Además, nos hemos servido del preprocesador SASS y de Gulp

Se aceptan expresiones de gratitud tales como una cerveza 🍺 o un café ☕
---

**Nombre del equipo - Undefined:**

Demo Para ver el resultado del desarrollo de la página web puedes visitar el siguiente enlace: http://beta.adalab.es/project-promo-m-module-2-team-5/


## Guía de inicio rápido

> **NOTA:** Instalar previamente [Node JS](https://nodejs.org/) para trabajar con este repo:

### Pasos a seguir para arrancar el proyecto desde tu ordenador:

1. No clonar este repo (porque no podrás añadir commits), descargarlo.
1. Crear un repo nuevo y añadir los archivos descargados.
1. **Abre una terminal** en la carpeta raíz de tu repositorio.
1. **Instala las dependencias** locales ejecutando en la terminal el comando:

```bash
npm install
```

Una vez hemos instalado las dependencias, vamos a arrancar el proyecto. **El proyecto hay que arrancarlo cada vez que lo abras** Para ello ejecuta el comando:

```bash
npm start
```

Este comando:

- **Abre una ventana de Chrome y muestra la página web**, al igual que hace el plugin de VS Code Live Server (Go live).
- También **observa** todos los ficheros que hay dentro de la carpeta `src/`, para que cada vez que modifiques un fichero **refresca tu página en Chrome**.
- También **procesa los ficheros** HTML, SASS / CSS y JS y los **genera y guarda en la carpeta `public/`**. Por ejemplo:
  - Convierte los ficheros SASS en CSS.
  - Combina los diferentes ficheros de HTML y los agrupa en uno o varios ficheros HTML.

Después de ejecutar `npm start` ya puedes empezar a editar todos los ficheros que están dentro de la carpeta `src/` y programar cómodamente.

### Pasos para publicar el proyecto en GitHub Pages:

Para generar la página para producción ejecuta el comando:

```bash
npm run docs
```

Y a continuación:

1. Sube a tu repo la carpeta `docs/` que se te acaba de generar.

```bash
git add -A
git commit -m "commit message"
git push
```

1. Entra en la pestaña `settings` de tu repo.
1. Y en el apartado de GitHub Pages activa la opción **master branch /docs folder**.

Además, los comandos:

```bash
npm run push-docs
```

o

```bash
npm run deploy
```

son un atajo que nos genera la versión de producción y hace push de la carpeta `docs/` del tirón.

## Flujo de archivos con Gulp

Estas tareas de Gulp producen el siguiente flujo de archivos:

![Gulp flow](./gulp-flow.png)

## `gulpfile.js` y `config.json`

Nuestro **gulpfile.js** usa el fichero `config.json` de configuración con las rutas de los archivos a generar / observar.

De esta manera separarmos las acciones que están en `gulpfile.js` de la configuración de las acciones que están en `config.json`.

## Estructura de carpetas

La estructura de carpetas tiene esta pinta:

```
src
 ├
 ├─ images
 |
 ├─ js // los ficheros de esta carpeta se concatenan en el fichero main.js y este se guarda en public/main.js
 |
 ├─ scss
 |  ├─ core
 |  ├─ layout
 |  └─ pages
 |  └─ styles
 |
 └─ html
    └─ index
    └─ design-card
    └─ partials
```

## Funcionamiento de la web

Búsqueda Se escribe en el input vacío creado para la búsqueda y al hacer click con el ratón sobre Search, la aplicación se conectará al API abierto de TVMaze para búsqueda de series. Obtenemos como respuesta un listado de elementos filtrados según lo que hayamos escrito en el input.

Favoritos Una vez aparecen los resultados de búsqueda, podremos indicar cuáles son nuestras series favoritas. Para hacer una serie favorita hacemos click sobre ella. Esta serie seleccionada cambiará su color de fondo y, además, se añadirá al listado de la izquierda donde veremos todas nuestras series marcadas como favoritas.

Almacenamiento local Hay que almacenar el listado de favoritos en el localStorage, de esta forma, al recargar la página, el listado de favoritos se mantiene como estaba.

### Gracias por visitar nuestro proyecto, será genial recibir feedback para mejorarlo!
