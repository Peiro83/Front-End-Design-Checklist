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
	* [1.4 Enlaces y navegación](#14---enlaces-y-navegación)
	* [1.5 Images / Icons](#15---images--icons)
	* [1.6 Formularios y botones](#16---formularios-y-botones)
	* [1.7 Diseño Web Responsivo](#17---diseño-web-responsivo)
	* [1.8 Guía de estilos y enfoque de componentes](#18---guia-de-estilos-y-enfoque-de-componentes)
	* [1.9 Delivery files](#19---delivery-files)
* **[2. Fases de análisis y previo al desarrollo](#2---fases-de-análisis-y-previo-al-desarrollo)**
	* [2.1 Análisis en papel](#21---análisis-en-papel)
	* [2.2 Fase antes del desarrollo](#22---fase-antes-del-desarrollo)
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

### 1.4 - Enlaces y navegación

![Enlaces y navegación](/images/links.png)

* [ ] Todos los **enlaces tienen los estados default, hover, focus, active y visited** claramente definidos (la Guía de Estilos es el mejor documento para especificar estos)
* [ ] Vistas alternadas de todos los estados de navegación (hover, active, página actual).

### 1.5 - Imágenes / Iconos

![Imágenes](/images/images.png)

* [ ] Una **imagen favicon** de almenos 512px X 512px es proporcionada en formato PNG. La generación de los demás Favicons pueden ser hechas fácilmente con herramientas en línea.

  __Recursos:__
  * [Favicon Generator for all platforms: iOS, Android, PC/Mac...](https://realfavicongenerator.net/)

* [ ] Todos los íconos son proporcionados en **formato SVG**, cada uno con las mismas dimensiones, en negro y por carpetas separadas.

  __Recursos:__
  * 🛠 [SVGOMG - SVGO's Missing GUI](https://jakearchibald.github.io/svgomg/)

* [ ] El **nombre de cada icono** comienca con `icono-` y solo en minúsculas (sin ningún espacio y usando `-` para separar cada palabra).

__Recursos adicionales:__
* 📖 [Essential Image Optimization](https://images.guide/)

**[⬆ volver a arriba](#tabla-de-contenidos)**

### 1.6 Formularios y botones

![Formularios](/images/form.png)

* [ ] Todos los furmularios poseen un título que puede ser usado como leyenda
* [ ] Un ejemplo de los **diferentes estados de todos los campos de entrada** fueron proporcionados (al menos los estados focus e inactivo/deshabilitado).
* [ ] Todos los **mensajes de error** fueron proporcionados , el texto (en un documento separado), la posición y colores son claramente identificados en los diseños y son consistentes. Algunos mensajes deben ser diferentes de acuerdo al error correspondiente.
  __Recursos:__
  * 📖 [Forms Need Validation – UX Collective](https://uxdesign.cc/forms-need-validation-2ecbccbacea1)
* [ ] **Indicadores para  campos requeridos/opcionales** son proporcionados.
* [ ] Los **botones primarios y secundarios** son claramente identificables y son usados siguiendo prácticas comunes.
  __Recursos:__
  * 📖 [Primary & Secondary Action Buttons – UX Planet](https://uxplanet.org/primary-secondary-action-buttons-c16df9b36150)
* [ ] Un ejemplo de los **diferentes estados de un botón** fueron proporcionados (estados default, hover, focused, pressed e inactive)
* [ ] Botones con **indicadores de carga** incorporados son proporcionados y pueden aplicarse a cualquier botón.

__Recursos adicionales:__

* 📖 [Design Better Forms – UX Collective](https://uxdesign.cc/design-better-forms-96fadca0f49c)
* 📖 [Design Better Input Fields – UX Collective](https://uxdesign.cc/design-better-input-fields-3d02985a8e24)
* 📖 [Designing Perfect Text Field: Clarity, Accessibility and User Effort](https://uxplanet.org/designing-perfect-text-field-clarity-accessibility-and-user-effort-d03c1e26004b)
* 📖 [Button UX Design: Best Practices, Types and States – UX Planet](https://uxplanet.org/button-ux-design-best-practices-types-and-states-647cf4ae0fc6)
* 📖 [How To Design Better Buttons — Smashing Magazine](https://www.smashingmagazine.com/2016/11/a-quick-guide-for-designing-better-buttons/)
* 📖 [Buttons in Design Systems – EightShapes – Medium](https://medium.com/eightshapes-llc/buttons-in-design-systems-eac3acf7e23)

**[⬆ volver a arriba](#tabla-de-contenidos)**

### 1.7 - Diseño Web Responsivo

![Responsive](/images/responsive.png)

* [ ] La **versión móvil** del diseño fue proporcionado antes o al mismo tiempo que la versión para escritorio.

	> Si el método **móvil primero** no fue aplicado por el equipo creativo, algunas irregularidades e inconsistencias pueden aparecer entre la versión móvil y la versión de escritorio. Verifica y marca estos problemas antes de iniciar el desarrollo del proyecto.
* [ ] En ciertos casos, la **versión para tabletas** del diseño es proporcionada.

⚠️ *El concepto **pixel perfecto** hoy en día está obsoleto. Es imposible tener un diseño que funcione de la misma forma frente a la multitud de tamaños de pantalla existentes.*

__Recursos adicionales:__

* 📖 [Official Google Webmaster Central Blog: Mobile-first Indexing](https://webmasters.googleblog.com/2016/11/mobile-first-indexing.html)

**[⬆ volver a arriba](#tabla-de-contenidos)**

### 1.8 - Guía de estilos y enfoque de componentes

![Styleguide](/images/styleguide.png)

* [ ] Todos los componentes en cada página fueron creados con el **enfoque basado en componentes** (Diseño Atómico). Si no es asi, pueden ocurrir problemas en terminos de rendimiendo, mantenimiento del proyecto, etc.

  __Rescursos:__
  * 📖 [Atomic design][16]
  * 📖 [6 Reasons for Component-Based UI Development](https://www.tandemseven.com/technology/6-reasons-component-based-ui-development/)

* [ ] Una **Guía de estilo** necesita ser proporcionada listando todos los elementos, componentes, estilos y dimensiones. Algunos boilerplates como [UX Power Tools](https://www.uxpower.tools/) pueden ayudar a ahorrar tiempo y mantener consistencia en los diseños.

⚠️ *En el caso de no contar con una Guía de estilo, es recomendable construir una [Guía de Estilos](https://github.com/davidhund/styleguide-generators) para facilitar tu trabajo. Algunos CMS como Drupal, tienen plugins que permiten desarrollar Guías de Estilo usando [Pattern Lab](https://drupal-pattern-lab.github.io/).*

__Recursos adicionales:__

* 📖 [Style Guides – Design + Sketch – Medium](https://medium.com/sketch-app-sources/tagged/style-guides)
* 📖 [The CodePen Design Patterns and Style Guide](https://codepen.io/guide)
* 📖 [Lonely Planet Travel Guides and Travel Information](http://rizzo.lonelyplanet.com/styleguide/design-elements/colours)
* 📖 [Styleguide](https://www.yelp.com/styleguide)

#### En el caso de un proyecto existente:

A veces, el equipo creativo necesita añadir páginas nuevas o módulos en un proyecto existente. Ellos deben tener o crear una lista de todos los elementos existentes e intentar usar lo que ya está ahí. Tener una Guia de Estilos ya creada puede salvar horas de trabajo y asegurar la consistencia del proyecto. 

**[⬆ Volver a arriba](#tabla-de-contenidos)**

### 1.9 - Entrega de archivos

![Entrega de archivos](/images/delivery-files.png)

* [ ]  Para todos los sitios web, el diseñador web necesita proporcionar al menos **2 PSD** (móvil, escritorio y eventualmente tableta) o al menos **1 archivo Sketch** que debe ser entregado con las medidas debajo (si usas Photoshop CC 2015 o superior, recomiendo usar artboards)

	> ℹ️ Algunos diseñadores web podrían crear multiples PSD correspondientes a cada componenete usado y los importan en un solo PSD como "capas inteligentes". En ese caso, tendrás multiples PSD enlazados a uno o más archivos. En el caso de Sketch, desde que las **librerias** existen desde la versión 47, es posible enlazar multiples archivos con símbolos.

* [ ] Los **archivos de diseño son limpiados** antes de entregar a los desarrolladores (se removieron capas innecesarias para evitar archivos grandes)

* [ ] La página de **error 404** (y eventualmente la página de error 500) fue diseñada.
* [ ] Todos los **popins, popups y cajas de alerta** fueron diseñados y pueden ser habilitados a treves de capas en la composición.

__Recursos adicionales:__

* 📖 [Photoshop Etiquette: A Guide to Discernible Web Design](http://photoshopetiquette.com/)

#### Reglas específicas para archivos PSD:

* [ ] **Composiciones en capas** son usadas para mostrar cada página si se proporcionan multiples vistas dentro del mismo PSD. Es una manera fácil de evitar confusiones y verificar que todos los elementos están organizados correctamente.

**[⬆ volver a arriba](#tabla-de-contenidos)**

## 2. - Fases de análisis y previo al desarrollo

![Analysis and phases](/images/phases.png)

Antes de iniciar las fases de  análisis y previo al trabajo y después de recibir los archivos de diseño, necesitas verificar algunos elementos importantes:

* __*¿Cuál versión de Photoshop, Sketch es usada?*__
  Algunas funciones son específicas de algunas versiones de Photoshop o Sketch. Es importante marcar cualquier problema que corresponda a esto tan pronto como sea posible.
* __*¿El ancho de cada PSD o artboard son correctos?*__
  En caso de que se añada espacios en cada lado del diseño, verifica el tamaño exacto del sitio web.
* __*¿Los diseños usan demasiado "box-shadow", "linear o radial gradient"?*__
  No olvides que ciertas propiedades pueden tener impacto en el rendimiento del navegador.
* __*¿Existe un mapa del sitio/breadcrumb para entender la arquitectura de todas las páginas y sus dependencias?*__
* __*¿El sitio web necesita tener imágenes retina?*__

**[⬆ volver a arriba](#tabla-de-contenidos)**

### 2.1 - Análisis en papel

![Análisis en papel](/images/analysis.png)

Se recomienda **imprimir** algunas (o todas) las páginas que tengas en formato A3 (o A4 si no posees ese formato). Debido al alto de la página, probablemente necesites imprimir algunos diseños en multiples páginas.

No puedo imaginar una mejor forma de iniciar que analisando los diseños en papel con un lapiz (o diferentes lapices de colores seleccionados para resaltar diferentes tipos de información).

1. Define la **estructura de las páginas**, encabezados, secciones, artículos, área principal, pie de página destacando estos al  menos en una página impresa.

2. Encuentra todos los **encabezados** en la estructura de página, asegurate que la etiqueta `H1`no se encuentre en el logo y que el orden lógico sea seguido. La mayoría de la veces, el H1 en la página de inicio será ocultado con CSS pero necesita mantener su significado legítimo. El análisis debe ser realizado con la ayuda de un especialista en SEO en caso de contar con uno en el equipo.

3. Intenta encontrar y reagrupar **componentes similares** asignandoles un nombre individual de acuerdo a su funcionalidad y no solo por su contexto.

4. La mayoría de los elementos de diseño pueden realizarse *usando CSS*. Hoy en día, es recomendado no usar ningun elemento de estructura usando imágenes. Cualquier elemento gráfico simple, como botones o bordes pueden ser echos en CSS para evitar problemas de rendimiento o escalabilidad.

5. Encuentra **posibles faltas de coherencia** en caso de no recibir una Guia de Estilo del equipo creativo, es tu responsabilidad asegurar que cada elemento gráfico pertenezca a una categoría (botones, tipografía, sliders,etc.). Te ayudará a crear tu propia arquitectura CSS/Sass o identificar cuáles componentes necesitarás de determinado Framework CSS.

⚠️ *Despues de la fase de análisis en papel, invita al equipo creativo a usar una herramienta como [InVision](https://www.invisionapp.com/) para facilitar la comunicación e intercambio entre el equipo creativo y los desarrolladores. La posibilidad de comentar en cada página puede ahorrar tiempo y permitir mantener un historial de modificaciones y decisiones.*

### 2.2 - Fase antes del desarrollo

* [ ] De acuerdo a las especificaciones, **los plugins necesarios fueron definidos** en una etapa temprana. Tener una lista previa de los plugins necesarios antes de comenzar el desarrollo puede ayudar al desarrollador a mantenerse enfocado y no ocupar mucho tiempo en investigar durante la fase de desarrollo. Obviamente, algunos plugins no serán adecuados y podrán cambiar.

__Recursos adicionales:__

* 🛠 [Awesome JS][22]
* 🛠 [BestOfJS][23]


**[⬆ volver a arriba](#tabla-de-contenidos)**

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
