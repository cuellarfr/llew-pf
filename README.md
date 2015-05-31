Proyecto Final LLEW
===================

Este repositorio contiene el código fuente original empleado en mi proyecto final de la asignatura Lenguajes y Estándares Web del Grado Multimedia de la UOC.

Consideraciones técnicas
------------------------

Para la elaboración de esta práctica he utilizado las siguientes tecnologías:

- **GitHub.** El código fuente de este proyecto está alojado en un repositorio público en GitHub. <https://github.com/cuellarfr/llew-pf>.
- **Heroku**. La web creada en este proyecto ha sido subida a Heroku y puede ser visualizada en: <http://llew-pf.herokuapp.com/>
- **Serve ERB.** Serve es un framework open-source de prototipado rápido para la web. Hace fácil crear un prototipo de una aplicación web, o una web sencilla sin escribir ni una sola linea de código de back-end. He incluído información sobre cómo descargar y ejecutar Serve en el wiki de este repositorio: <https://github.com/cuellarfr/llew-pf/wiki/Acerca-de-Serve>
- **Haml.** Haml es un lenguaje de marcado ligero. Entre sus ventajas están que genera un código muy limpio y elegante. Visualmente es más fácil de entender puesto que se representa la estructura del DOM mediante sangrado, y además se evitan los típicos fallos creados al dejar etiquetas HTML abiertas. Más información en la web oficial de Haml: <http://haml.info/>
- **Sass.** Sass es un preprocesador de CSS. Utilizado de forma correcta, es muy útil puesto que expande las posibilidades de CSS mediante funcionalidades como variables, mixins, extensiones y reglas matemáticas. Además, permite crear hojas de estilo de forma modular, distribuídas en distintos archivos que son finalmente compilados en un archivo CSS estándar. Más información en <http://sass-lang.com/>
- **FitVids.** FitVids es un plugin de jQuery que permite incrustar vídeos con ancho ajustable a su contenedor. De esta forma podemos incluir vídeos que se adaptan al tamaño de la pantalla, imprescindible en webs responsive. Más información en: <https://github.com/davatron5000/FitVids.js>


Comentarios al código HTML y CSS
--------------------------------

He incluído comentarios al código HTML y CSS. Se pueden consultar fácilmente en el repositorio de GitHub:

- Archivos Sass (compilados después como CSS3): <https://github.com/cuellarfr/llew-pf/tree/master/sass>
- Archivos Haml (compilados después como HTML5): <https://github.com/cuellarfr/llew-pf/tree/master/views>


Arquitectura CSS
----------------

He seguido la metodología **Smacss** para organizar mis hojas de estilo. Smacss es una guía de estilo para escribir CSS de forma modular y escalable. Consiste en categorizar las reglas de CSS en reglas base (se refiere a los estilos para etiquetas HTML), reglas de maquetación (para definir estructura de páginas), reglas de módulos (se refiere a todo elemento visual repetible en una web) y reglas de estado (elementos alterados mediante Javascript). También se propone una nomenclatura estándar para reglas CSS, aunque en este caso he preferido seguir la nomenclatura BEM <https://en.bem.info/>. Más información sobre Smacss en: <https://smacss.com/>

<pre>
.
+-- base
|   +-- _elements.scss
|   +-- _normalize.scss
+-- layouts
|   +-- _global.scss
+-- modules
|   +-- _buttons.scss
|   +-- _lists.scss
|   +-- _nav.scss
|   +-- _panels.scss
+-- settings
|   +-- _mixins.scss
|   +-- _variables.scss
+-- _app.css
</pre>

