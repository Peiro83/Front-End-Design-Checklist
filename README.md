![Front-End Design Checklist](/images/front-end-design-checklist-banner.jpg)
<h2 align="center">Front-End Design Checklist</h2>

<p align="center">
  <em> The Design Checklist para Desarrolladores Front-end es una lista exhaustiva de elementos que pueden ayudar al desarrollador a analizar y entender diseños para web para asegurar la calidad del desarrollo Front-end .</em>
</p>

[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](http://makeapullrequest.com) [![Join the chat at https://gitter.im/Front-End-Checklist/Front-End-Design-Checklist](https://badges.gitter.im/Front-End-Checklist/Front-End-Design-Checklist.svg)](https://gitter.im/Front-End-Checklist/Front-End-Design-Checklist) [![CC0](https://img.shields.io/badge/license-CC0-green.svg)](https://creativecommons.org/publicdomain/zero/1.0/)

## Tabla de contenidos
* **[1. Requerimentos de diseño](#1---Requerimentos-de-diseño)**
	* [1.1 Sistema de retículas](#11---sistema-de-retículas)
	* [1.2 Colores](#12---colores)
	* [1.3 Fuentes y textos](#13---fuentes-y-textos)
	* [1.4 Links and navigation](#14---links-and-navigation)
	* [1.5 Images / Icons](#15---images--icons)
	* [1.6 Forms and buttons](#16---forms-and-buttons)
	* [1.7 Responsive Web Design](#17---responsive-web-design)
	* [1.8 Style Guide and component approach](#18---style-guide-and-component-approach)
	* [1.9 Delivery files](#19---delivery-files)
* **[2. Analysis and pre-work phases](#2---analysis-and-pre-work-phases)**
	* [2.1 Paper analysis](#21---paper-analysis)
	* [2.2 Pre-development phase](#22---pre-development-phase)
* **[3. Validation](#3---validation)**
* **[4. Development phase](#4---development-phase)**
* **[5. Before production](#5---before-production)**

---

> The **Design Checklist para Desarrolladores Front-end** es una lista exhaustiva de elementos que los Diseñadores Web y Desarrolladores Fron-end necesitan tomar en consideración para facilitar su colaboración. Los siguientes elementos son una mezcla entre mejores prácticas y elementos basados en amplia experiencia analizando diseños para web.

En caso de buscar una lista de todos los emementos que debes tener/probar antes de lanzar un sitio/página HTML a producción, dale un vistazo a → [Front-End Checklist](https://github.com/eoasakura/Front-End-Checklist-ES).


## ¿Cómo usar The Desing Checklist?

Cuando llega el momento que se les presenta a desarrolladores nuevos diseños para web, antes de convertirlos a código, se deben considerar elementos que podrían pasar desapercibidos. The Front-end Design Checklist es una herramienta para desarrolladores Front-end y Diseñadores Web que tiene el objetivo de ayudarlos a trabajar sin problemas.

Puedes compartir esta lista con Diseñadores Web para asegurar ahorrar tiempo en las entregas o puedes utilizarla para revisar todos los elementos proporcionados por el equipo creativo y asegurar que todo está correcto antes de comenzar con la integración de código.


## ¿Por qué necesitas usar esto?

* Asegurar que todos los puntos son tomados en consideración por el equipo creativo.
* Tener un documento que los Diseñadores y Desarrolladores puedan consultar para asegurar una mejor comunicación y coherencia en la manera en que interactuan.
* Porque es fácil olvidar elementos importantes cuando eres presionado por tiempos de entrega cortos
* Evitar descubrir problemas cuando el equipo creativo ya está trabajando en otro proyecto.
* Para mostrar el trabajo complementario entre Diseñadores y Desarrolladores

---

## 1. - Requerimentos de diseño

Diseñar un sitio web o aplicación web requiere seguir algunas reglas y tomar en consideración que el proyecto no es solo un proyecto gráfico, sino también un proyecto web. La siguiente sección es crucial para cualquier proyecto web.

### 1.1 - Sistema de retículas

![Sistema de retícula](/images/grid-system.png)

* [ ] Una **retícula** es explícitamente proporcionada en el diseño y los detalles de ella están presentes en las especificaciones técnicas (ancho, medianiles, números de columnas...). El Diseñador Web puede mantener una retícula en una capa transparente y utilizarla en todos el proyecto.
	> ℹ️ [Guide Guide][6] es un plugin para Photoshop que puede ayudar a construir facilmente tu retícula.

	> ℹ️ En Sketch, puedes usar la herramienta integrada “[Make Grid][7]” para diseñar tu retícula.

* [ ] **Familiarizate con el sistema de retícula** que usarás en tu proyecto. La mayoría de las ocasiones, algunas opciones (como alineación, offsett, anidamiento...) son ignoradas por el desarrollador y tienden a remplazarlas innecesariamente por márgenes o relleno manual.
* [ ] Antes de trabajar en cada componente de tu sitio web, puedes **construir cada plantilla** usada en los diseños solo con las clases de la retícula. Construir la estructura antes que nada, te facilitará tu trabajo posterior.

```html
<div class="container">
  <div class="row">
    <div class="col-sm">
      <!-- Déjalo vacío al inicio -->
    </div>
    <div class="col-sm">
      <!-- Déjalo vacío al inicio -->
    </div>
    <div class="col-sm">
      <!-- Déjalo vacío al inicio -->
    </div>
  </div>
</div>
```

⚠️ *Si quieres asegurarte que la retícula y el ancho de los dispositivos sean respetados, podrías generar una plantilla PSD que le envies al Diseñador Web*

__Recursos adicionales:__ (recursos en inglés)

* 🛠 [Bootstrap Grid System][8] (v4) retícula de Bootstrap
* 🛠 [Flexbox Grid][9] Sistema de retícula aplicando Flexbox
* 📖 [Don't Overthink It Grids | CSS-Tricks][10]

**[⬆ volver a arriba](#tabla-de-contenidos)**

### 1.2 - Colores

![Colores](/images/colors.png)

* [ ] **A todos los colores usados en los diseños se les asigna un nombre** ($gris-claro, $gris-oscuro, $verde), este puede ser de acuerdo a su uso ( $fondo-de-página, $texto, $títulos...) Pueden ser exportados en un [archivo ACO][11] (si usas Photoshop o un símbolo de página para Sketch) y compartirlo con los desarrolladores.

![Muestras de color](/images/color-swatches.jpg)

* [ ] Los diferentes **colores de estado** de algunos elementos (como botones, enlaces, campos de texto) son definidos y trabajados en el contexto de un fondo claro y oscuro con texto claro y oscuro.

* [ ] Los colores más usados o los más importantes **son accesibles**(contraste entre colores adecuado) en el diseño para permitir una navegación fluida en el sitio web/aplicación web.

__Recursos adicionales:__ (recursos en inglés)
* 🛠 [WCAG - Contrast Checker](https://contrastchecker.com/) Herramienta para verificar contraste de colores
* 🛠 [Color Safe - accessible web color combinations](http://colorsafe.co/) Recomendaciones de colores accesibles
* 🛠 [Coolors.co - The super fast color schemes generator](https://coolors.co/)

**[⬆ volver a arriba](#tabla-de-contenidos)**

### 1.3 - Fuentes y textos

![Fuentes](/images/fonts.png)

Las fuentes son una parte esencial de cada diseño, no deben ser elegidas sin un buen juicio. Elegir la fuente incorrecta para un proyecto puede tener consecuencias de impacto financiero y legal.

Es recomendable solicitar a tu cliente comprar estas fuentes para evitar posibles problemas a futuro y tomar en consideración las condiciones de uso. Algunas fuentes para web están limitadas en terminos de vistas por página y no pueden ser almacenadas en tu hosting. ([Understanding Webfont Licensing Structures](https://aeolidia.com/understanding-webfont-licensing-structures/)).


* [ ] Las fuentes para escritorio (TTF o OTF) y las fuentes web, en **formato WOFF, WOFF2 y TTF** fueron proporcionadas (en un archivo Zip o se dio acceso al sitio web donde fueron compradas)
	> ℹ️ El formato TTF para escritorio no es el mismo que el TTF para web.

  __Recursos:__  (recursos en inglés)
	* 📖 [Using @font-face | CSS-Tricks](https://css-tricks.com/snippets/css/using-font-face/) Uso de la propiedad @font-face
* [ ] Una [fuente de respaldo](https://en.wikipedia.org/wiki/Fallback_font) fue especificada en el documento (idealmente en la Guía de estilos) para el Desarrollador Front-end.

  __Recursos:__ (recursos en inglés)
  * 📖 [CSS Basics: Fallback Font Stacks for More Robust Web Typography | CSS-Tricks](https://css-tricks.com/css-basics-fallback-font-stacks-robust-web-typography/)
  * [Create Your Own @font-face Kits » Font Squirrel](https://www.fontsquirrel.com/tools/webfont-generator)

* [ ] El **tamaño total** de las fuentes no debe exceder de 1 a 2 Mb (incluyendo todas las variantes: italica, negrita, etc.)

* [ ] Tanto como sea posible, **todos los textos son proporcionados en el lenguaje adecuado** en vez de textos de ejemplo (Lorem Ipsum y similares).

	> ℹ️ En el caso de sitios web multilenguaje, siempre preguntate a ti mismo cómo reaccionaría el diseño si los textos fueran más largos de lo que fueron definidos anteriormente. Recuerda que los Diseñadores Web acostumbran crear diseños perfectos y no siempre piensan sobre los posibles problemas o situaciones con demasiado texto. 

__Recursos adicionales:__ 
* 📖 [Optimización de fuentes web  |  Web  |  Google Developers](https://developers.google.com/web/fundamentals/performance/optimizing-content-efficiency/webfont-optimization) disponible en Español
* [`font-display` for the Masses | CSS-Tricks](https://css-tricks.com/font-display-masses/) contenido en inglés

**[⬆ volver a arriba](#tabla-de-contenidos)**

### 1.4 - Links and navigation

![Links and navigation](/images/links.png)

* [ ] All **links have a default, hover, focus, active and visited state** clearly defined (the Style Guide is the best document to specified these).
* [ ] Alternate views of all navigation states (hover, active/current page).

### 1.5 - Images / Icons

![Images](/images/images.png)

* [ ] A **favicon image** with at least 512px X 512px is provided in PNG format. The generation of all the others Favicons can be easily done with online tools.

  __Resources:__
  * [Favicon Generator for all platforms: iOS, Android, PC/Mac...](https://realfavicongenerator.net/)

* [ ] All icons are provided in **SVG format**, each in the same square dimension, in black and in a separated folder.

  __Resources:__
  * 🛠 [SVGOMG - SVGO's Missing GUI](https://jakearchibald.github.io/svgomg/)

* [ ] The **name of each icon** starts with `icon-` and is entirely in lowercase (without any space and using dashes to separate each word).

__Additional Resources:__
* 📖 [Essential Image Optimization](https://images.guide/)

**[⬆ back to top](#table-of-contents)**

### 1.6 Forms and buttons

![Forms](/images/form.png)

* [ ] All forms possess a title that can be used as a legend
* [ ] An example of the **different states of all input fields** were provided (at least focus and inactive/disabled state).
* [ ] **All error messages** were provided, the text (eventually in a separated document) the position and the color are clearly identifiable in the creatives and consistent. Some messages should be different according to the error.
  __Resources:__
  * 📖 [Forms Need Validation – UX Collective](https://uxdesign.cc/forms-need-validation-2ecbccbacea1)
* [ ] **Indicators of required/optional** fields are provided.
* [ ] The **primary and secondary buttons** are clearly identifiable and are used following common practices.
  __Resources:__
  * 📖 [Primary & Secondary Action Buttons – UX Planet](https://uxplanet.org/primary-secondary-action-buttons-c16df9b36150)
* [ ] An example of the **different states of a button** were provided (Normal, hover, focused, pressed and inactive state).
* [ ] Buttons with built-in **loading indicators** are provided and can be applied to any button.

__Additional Resources:__

* 📖 [Design Better Forms – UX Collective](https://uxdesign.cc/design-better-forms-96fadca0f49c)
* 📖 [Design Better Input Fields – UX Collective](https://uxdesign.cc/design-better-input-fields-3d02985a8e24)
* 📖 [Designing Perfect Text Field: Clarity, Accessibility and User Effort](https://uxplanet.org/designing-perfect-text-field-clarity-accessibility-and-user-effort-d03c1e26004b)
* 📖 [Button UX Design: Best Practices, Types and States – UX Planet](https://uxplanet.org/button-ux-design-best-practices-types-and-states-647cf4ae0fc6)
* 📖 [How To Design Better Buttons — Smashing Magazine](https://www.smashingmagazine.com/2016/11/a-quick-guide-for-designing-better-buttons/)
* 📖 [Buttons in Design Systems – EightShapes – Medium](https://medium.com/eightshapes-llc/buttons-in-design-systems-eac3acf7e23)

**[⬆ back to top](#table-of-contents)**

### 1.7 - Responsive Web Design

![Responsive](/images/responsive.png)

* [ ] The **mobile version** of the design is provided before or at the same time of the desktop version.

	> If the “**mobile first**” thinking was not followed by the creative team, some irregularities and inconsistencies may appear between the mobile and the desktop version. Check and flag these issues before starting the development of the project.
* [ ] The **tablet version** of the design in certain cases should be provide too.

⚠️ *The **pixel perfect** notion is today in a certain way deprecated. Today, it’s impossible to have a design that worked the same facing the multitude of the screen sizes.*

__Additional Resources:__

* 📖 [Official Google Webmaster Central Blog: Mobile-first Indexing](https://webmasters.googleblog.com/2016/11/mobile-first-indexing.html)

**[⬆ back to top](#table-of-contents)**

### 1.8 - Style Guide and component approach

![Styleguide](/images/styleguide.png)

* [ ] All components designed on each page were created with the **component based approach**  (Atomic Design). If not, issues can occur in terms of performance, maintainability of the project...

  __Resources:__
  * 📖 [Atomic design][16]
  * 📖 [6 Reasons for Component-Based UI Development](https://www.tandemseven.com/technology/6-reasons-component-based-ui-development/)

* [ ] A **Style Guide** needs to be provided listing all elements, components, styles, dimensions. Some boilerplates like [UX Power Tools](https://www.uxpower.tools/) can help saving time and keep consistency in the designs.

⚠️ *In the case where the Style Guide is missing, it's a good practice to build yourself a [living Style Guide](https://github.com/davidhund/styleguide-generators) to faciliate your work. Some CMS like Drupal, for example, have plugins that allow to develop a living Style Guide using [Pattern Lab](https://drupal-pattern-lab.github.io/).*

__Additional Resources:__

* 📖 [Style Guides – Design + Sketch – Medium](https://medium.com/sketch-app-sources/tagged/style-guides)
* 📖 [The CodePen Design Patterns and Style Guide](https://codepen.io/guide)
* 📖 [Lonely Planet Travel Guides and Travel Information](http://rizzo.lonelyplanet.com/styleguide/design-elements/colours)
* 📖 [Styleguide](https://www.yelp.com/styleguide)

#### In the case of an existing project:

Sometimes, the creative team needs to add new pages or modules in an existing project. They should have or create a list of all existing elements and try to use what is already there. Having a Style Guide already created can save hours and ensure consistency of the project.

**[⬆ back to top](#table-of-contents)**

### 1.9 - Delivery files

![Delivery files](/images/delivery-files.png)

* [ ] For all websites, the web designer needs to provide at least **2 PSD** (mobile, desktop and eventually tablet) or at least **1 Sketch file** which needs to be delivered with the dimension below (if you have Photoshop CC 2015 and above, I recommend using artboards).

	> ℹ️ Some web designers could eventually create multiple PSD corresponding to each components used and import them in a single PSD as “smart layer”. In that case, you’ll have multiple PSD linked to one or two files. In the case of Sketch, since the **libraries** exist since version 47, it is possible to link multiples files with symbols ……..

* [ ] The **creative files are cleaned** before delivering to developers (empty and uneccessary layer needs to be removed to avoid large files).

* [ ] The **404 error** (and eventually the page 500 error) page were designed.
* [ ] All **popins, popups and alert boxes** were designed and can be enable throw layers of compositions.

__Additional Resources:__

* 📖 [Photoshop Etiquette: A Guide to Discernible Web Design](http://photoshopetiquette.com/)

#### Specific rules for PSD file:

* [ ] **Layer compositions** are used to show each different pages, if multiple views are provided within the same PSD. It’s an easy way to avoid confusions and check that all elements are correctly organized.

**[⬆ back to top](#table-of-contents)**

## 2. - Analysis and pre-work phases

![Analysis and phases](/images/phases.png)

Before starting the analysis and the pre-work phases and after receiving the creative files, you need to check some important elements:

* __*Which version of Photoshop, Sketch is used?*__
  Some features are specific to some versions of Photoshop or Sketch. It is important to flag any issue regarding this as soon as possible.
* __*Is the width of each PSD or artboard correct?*__
  In case some space is added on each side of the design, check the exact width of the website.
* __*Are the creatives using too much “box-shadow”, “linear or radial gradient”…?*__
  Don’t forget the .... Effect which can have impacts on the browser painting performance.
* __*Is a sitemap / breadcrumb provided to understand the architecture of all pages and their dependencies?*__
* __*Does the website needs to have retina images?*__

**[⬆ back to top](#table-of-contents)**

### 2.1 - Paper analysis

![Paper Analysis](/images/analysis.png)

It is recommended **printing** some (or all) of the pages you have on an A3 format (or A4 if you don’t have this format). Because of the height of the page. you’ll probably need to print some designs on multiple pages.

I can’t imagine a better way to start than analysing creatives on a paper with a pencil (or different colourful pencils choosed to highlight different type of informations).

1. Define the **structure of the pages**, the headers, the sections, the articles, main, footer outlining these on at least one printed page.

2. Find all the **headings** that structured a page, ensure the `H1` is not on the logo and that the logical order is followed. Most of the time, the H1 for the homepage will be hidden with CSS but needs to keep its legitimate meaning. That analysis should be done with the help of a SEO specialist in case you have one in your team.

3. Try to find and regroup **similar components** giving them an individual name regarding their functionality and not just their context. For example, naming a tab system “

4. Most of the creative elements can be **done using CSS**. Today, it is not recommended to create any layout element using images. Any simple graphical element like buttons or borders should be done in CSS to avoid performance or scalability issues.

5. Find some **possible lack of coherence**, in case a Styleguide was not provided by the creative team, it’s your responsibility to ensure that every graphic element belong to a possible category (Buttons, Typography, Sliders…). It’ll help you to create your own CSS / Sass architecture or to identify which component you’ll need from an identified CSS Framework.

⚠️ *After the paper analysis phase, you can invite the creative team to use a tool like [InVision](https://www.invisionapp.com/), to facilitate the communication and exchange between the creative team and the developers. The possibility to comment directly on pages can be a time-saver and allow to keep a history of modifications and decisions.*

### 2.2 - Pre-development phase

* [ ] According to the specifications, **plugins needed were defined** in an early stage. Having a pre-list of possible plugins before starting the development can help the developer to stay focus and not spend too much time in doing research during the development phase. Obviously, some plugins may not perfectly fit and will be changed accordingly.

__Additional Resources:__

* 🛠 [Awesome JS][22]
* 🛠 [BestOfJS][23]


**[⬆ back to top](#table-of-contents)**

## 3. - Validation

The validation phase is when everything seems to be ready to be integrated. The client, in general, validate the creatives without waiting for any approval from the technical team. As exposed in the Design Checklist, it is essential that developers ensure the quality of the delivery before starting to code.

## 4. - Development phase

* [ ] All **medias can be cut and saved** before starting the development phase. That can help you to avoid back and forth between your creative software and your code editor.

* [ ] **The image folder has a clear architecture** where you  arranged the layout's images. It is important to stay consistent between projects in general. Defining a structure for that folder and a naming convention can be helpful.


  You can find an example of a possible structure with prefixes used to recognise each image appurtenance.

```bash
.
└── images
    ├── background
    ├── banners
    ├── icons
    └── layout
```

* [ ] **A naming convention is used** like adding prefixes to diferenciate types of images, all images used for background can be prefixed by `bg-`, icons by `icon-`, hero banners by `hero-` or `banner-` and so on.

## 5. - Before production

Before launching your website, be sure to review all your pages using the [Front-End Checklist](https://frontendchecklist.io)!

**[⬆ back to top](#table-of-contents)**

---

## Translations

The Front-End Design Checklist will be soon available in other languages. Don't hesitate if you want to help for forking this repository and start with a translation in your language!

## Support

If you have any question or suggestion, don't hesitate to use Gitter or Twitter:

* [Give an UP on Product Hunt](https://www.producthunt.com/posts/front-end-design-checklist)
* [Chat on Gitter](https://gitter.im/Front-End-Checklist][28]/Front-End-Design-Checklist?utm_source=share-link&utm_medium=link&utm_campaign=share-link)
* [Facebook](https://www.facebook.com/frontenddesignchecklist/)
* [Twitter](https://twitter.com/thedaviddias)

## Author

**[David Dias](https://github.com/thedaviddias)**

## Contributors

This project exists thanks to all the people who [contribute!](.github/CONTRIBUTING.md)

## License

[![CC0](https://i.creativecommons.org/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)

All icons are provided by [Icons8](https://icons8.com/)

**[⬆ back to top](#table-of-contents)**


[6]:	https://guideguide.me/
[7]:	https://www.sketchapp.com/docs/canvas/rulers-guides-grids/
[8]:	https://getbootstrap.com/docs/4.0/layout/grid/
[9]:	http://flexboxgrid.com/
[10]: https://css-tricks.com/dont-overthink-it-grids/
[11]:	https://www.lifewire.com/aco-file-2619477
[16]:	http://bradfrost.com/blog/post/atomic-web-design/
[22]:	https://js.libhunt.com/
[23]:	https://bestof.js.org/
[28]:	https://gitter.im/Front-End-Checklist/Front-End-Design-Checklist
