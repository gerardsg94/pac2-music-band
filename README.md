# UOC Boilerplate

UOC Boilerplate is a starter template for the HTML and CSS Tools courses from the [Master's Program in Multimedia Applications](https://estudis.uoc.edu/ca/masters-universitaris/aplicacions-multimedia/presentacio) and the [Master's Program in Web App and Website Development](https://estudis.uoc.edu/ca/masters-universitaris/desenvolupament-llocs-aplicacions-web/presentacio) at the [Universitat Oberta de Catalunya](https://www.uoc.edu). It aims to provide a basic, modern frontend web development starter pack based on Parcel and including a Sass compiler, an ES6 transpiler, minifiers, an image transformer, and development tools.

This is the 3.x version of UOC Boilerplate, available since the UOC 2020-2 semester.

## Requirements

[Node.js](http://nodejs.org/) >= 14.15.x

## Getting started

Clone this repository with `git clone`, or download a .zip file using the top right green button.

Using the Terminal, navigate to the project folder and run `npm install`.

## Features

- Uses [Parcel v2](https://parceljs.org) module bundler.
- NPM scripts for fast development and production build (see Commands below).

### Stylesheets

- [Sass/SCSS](https://sass-lang.com) to CSS compilation.
- Minification and optimization of CSS files on production builds with [`cssnano`](https://github.com/cssnano/cssnano) (`@parcel/optimizer-cssnano`).
- [PostCSS](https://postcss.org/) features:
  - Transpile modern CSS with [`postcss-preset-env`](https://preset-env.cssdb.org/features).
  - Automatically add CSS prefix to unsupported properties with [`autoprefixer`](https://autoprefixer.github.io/).

### HTML

- Minification and optimization of CSS files on production builds [`htmlnano`](https://github.com/posthtml/htmlnano) (`@parcel/optimizer-htmlnano`).
- [PostHTML](https://github.com/posthtml/posthtml) features:
  - Include partial HTML files with [`posthtml-include`](https://github.com/posthtml/posthtml-include).

### Scripts

- Allow for modern JavaScript (ES201x/ES8/ES7/ES6…) which is automatically transpiled to ES5 and minifed in production builds, with [Babel](https://babeljs.io/).

### Images

- Image transformation with [`@parcel/transformer-image`](https://parceljs.org/recipes/image/) (based on [`sharp`](https://sharp.pixelplumbing.com/)).

### Development

- Development server launch and live reloading on file changes.
- Friendly error reporting.

## How to use this boilerplate

Content lives inside the `src/` folder. If you do not want to change the configuration or are unsure about what you are doing, do not edit files outside the `src/` folder.

Always run the following commands during the development stage and for production builds. Please note that it is expected that all projects built with this boilerplate are compiled using `npm run build` before they are published.

### Commands

| Command         | Description                                                                                                                                                                                                                                                                                                                                                         |
| --------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `npm run dev`   | Runs a local web server for development and opens the browser to display it. Automatically compiles styles and scripts whenever a file in `src/` is changed, and live reloads the browser. This is what _must be run_ on the development stage.                                                                                                                     |
| `npm run build` | Compiles and minifies and optimizes the files in the assets folder. The generated compiled and optimized files are located in the `dist/` folder. This is what _must be run_ before publishing the project. This is also the build command to be run by external deployment services such as Netlify. The publishable files are then located in the `dist/` folder. |
| `npm run clean` | Deletes the current `/dist` folder and cache folders.                                                                                                                                                                                                                                                                                                               |
| `npm run test`  | Displays a success message if everything is working as expected.                                                                                                                                                                                                                                                                                                    |

## Need help? / Want to help out?

Feel free to create a [new issue](https://github.com/uoc-advanced-html-css/uoc-boilerplate/issues/new/) or drop me a line at jorditarrida@uoc.edu.

Are you using this Boilerplate for your projects or for educational purposes? I would love to hear about it!

---------------------------------------------------------

ENUNCIAT

El lloc web ha de tenir quatre pàgines (pàgina de portada i tres pàgines interiors), seguint els wireframes proporcionats. La temàtica del lloc web ha de ser informació sobre el festival de música que organitzes. Tota la informació que no es proporciona amb l’enunciat, així com la línia gràfica, la pots decidir tu segons els gustos o et convingui. Cal seguir aquestes directrius sobre cada pàgina:
La pàgina de portada: ha d’estar maquetada amb CSS Grid i has de realitzar algun disseny interessant, semblant al què podria ser un poster promocional de la banda. Com a punt de partida, pots llegir l’article “How I design with CSS Grid” de Chen Hui Jing, on explica com fer una pàgina de portada en format poster. També et pots inspirar en alguns dels vídeos de la Jen Simmons al seu canal Layout Land. La maquetació que realitzis ha de ser compatible amb navegadors que no suportin CSS Grid, usant @supports i oferint una versió alternativa, com s’explica a la guia del mòdul 3.2. Cal que assoleixis els objectius proposats, però no cal que siguis massa creatiu o que perdis moltíssim temps en aquest apartat.
Una de les pàgines interiors ha d'incloure una retícula amb informació sobre els membres del grup de música, maquetada amb flex. Per a aquesta retícula, no pots utilitzar les classes de Bootstrap .row o .col-*.
Una de les pàgines interiors ha de seguir un format d’article i incloure un mínim de 4 paràgrafs de text i 2 fotografies. Pot ser una pàgina que contingui informació genèrica del grup de música, una pàgina de l’estil notícia o nota de premsa, o qualsevol altra opció que compleixi els requisits descrits. A banda de la maquetació de la pàgina caldrà que apliquis estils a alguns elements HTML que habitualment podrien formar part d’una pàgina d’aquest tipus, com ara <blockquote> o llistes (com es pot veure al wireframe).
La tercera pàgina interior és de contingut completament lliure. La pots usar per a ensenyar qualsevol cosa que sàpigues fer o que hagis après. Algunes idees són: una pàgina de contacte amb un formulari funcional (pot ser interessant provar Netlify Forms), una galeria de fotos interactiva, un joc, vídeos…
El lloc web ha de ser responsive i s’ha de poder visualitzar correctament des de qualsevol dispositiu modern (telèfon, tauleta, ordinador…). A la reunió només vas tenir temps de fer els wireframes de la versió d’escriptori, així que caldrà veure com adaptes a dispositius més petits l’estructura acordada.
Cal partir de UOC Boilerplate per al teu desenvolupament. Assegura't d'estar-ne usant la darrera versió (en el moment d'escriure aquest enunciat, la darrera versió és la 3.5.0). Cal respectar l’estructura i nomenclatura de carpetes i fitxers (a no ser que la metodologia o guia d’estil escollida indiqui el contrari!). Tens tota la informació sobre la instal·lació i ús a la guia del mòdul 1.
Cal que facis una tria d’una o més de les metodologies i guies d’estil estudiades al mòdul 2 i l’apliquis al teu desenvolupament.
Cal usar Bootstrap 5, carregat a UOC Boilerplate i personalitzat amb Sass com s’indica als materials, i usar un mínim de 4 components diferents. Cal personalitzar algun paràmetre dels components utilitzats a través de variables Sass, tal com s’explica a la secció Customize de la documentació de Bootstrap.
A banda, cal incorporar i usar alguna altra dependència externa, com ara FontAwesome o qualsevol altra que consideris interessant. Pot ser una bona idea per a la pàgina de contingut lliure. Pots explicar al fòrum quina és, per què l’has escollida, i si tens cap dubte o incidència amb el seu ús.
A més d’aquesta dependència, cal que hi instal·lis Stylelint i en personalitzis la configuració perquè apliqui els criteris d’estils escollits, amb plugins i normes. Cal que un cop executis l’ordre per a validar-ho no hi aparegui cap error.
Cal utilitzar necessàriament les següents característiques de Sass: variables, imbricació (nesting), funcions, parcials i importació.
Un cop finalitzat el desenvolupament, cal que publiquis el codi a GitHub i facis un deployment a Netlify, com s’explica a la guia del mòdul 1.

Enllaços d'interes:
https://www.youtube.com/watch?v=DSsrLrvvPPU
https://github.com/xgqfrms/css-poster-all-in-one

