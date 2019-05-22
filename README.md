# React - Preguntas Frecuentes

Esta guía pretende reunir contenido de calidad sobre los conceptos básicos de React en un solo sitio para tener una referencia rápida.

Recuerda que todos estamos aprendiendo. Lea, haz pruebas, ensúciate (está bien).

### Otros idiomas
[🇬🇧 English](https://github.com/timarney/react-faq)

[🇨🇳 简体中文](https://github.com/justjavac/react-faq)

# Comienzo

>Hay mucho que aprender, pero si se desglosa, hay algunos conceptos clave en los que enfocarse. JSX, elementos React, Componentes, Métodos de ciclo de vida, Propiedades y Estado. Los siguientes artículos te iniciarán en el camino hacia el aprendizaje de React.

**No sé nada de React, ¿que debería ver / leer antes de empezar?**
* [Pensando en React - Pete Hunt](https://facebook.github.io/react/docs/thinking-in-react.html)
* 🔥 [Enseñando React sin usar React](https://medium.com/@ericclemmons/teaching-react-without-using-react-a4b87cfd4e87#.q8cyvryw1) Eric Clemmons @ericclemmons
* 🔥 [13 cosas que necesitas saber sobre React](http://aimforsimplicity.com/post/13-things-you-need-to-know-about-react)  @kjendrzyca
* [Las 5 cosas que necesitas saber para entender React](https://medium.com/@sachagreif/the-5-things-you-need-to-know-to-understand-react-a1dbd5d114a3#.uii8of7um) Sacha Greif

**La documentación oficial de React es un gran recurso**
* [Documentación Oficial de React](https://facebook.github.io/react/docs/hello-world.html)

**Información adicional para empezar**
* [Pete Hunt: React: Rehaciendo las buenas prácticas (JSConf EU 2013)](https://www.youtube.com/watch?v=x7cQ3mrcKaY)
* [React en 7 Minutos](https://egghead.io/lessons/react-react-in-7-minutes) this is a slightly dated but still really good starter
* [Introducción completa a React - React, Webpack, Babel, Redux, React Router, SSR](https://btholt.github.io/complete-intro-to-react/) Brian Holt(@holtbt) for Frontend Masters worshop
* [Los momentos "Aha" con React](https://tylermcginnis.com/react-aha-moments) Tyler McGinnis @tylermcginnis33
* [Todas las cosas terribles que hice la primera vez que escribí una Aplicación Compleja con React](https://youtu.be/Fk--XUEorvc?t=20666) Raquel @raquelxmoss
* [Introducción a React](https://mva.microsoft.com/en-US/training-courses/introduction-to-react-16635?l=4wrKgdJrC_206218965) Eric W. Greene / Microsoft Virtual Academy

## Contenido

- [Historia](#historia)
- [Creando un Proyecto con React](#creando-un-proyecto-con-react)
- [¿Porque usar React?](#porque-usar-react)
- [JSX](#jsx)
- [El 'Virtual DOM'](#el-virtual-dom)
- [Elementos React](#elementos-react)
- [Componentes](#componentes)
- [Métodos del Ciclo de Vida](#métodos-del-ciclo-de-vida)
- [Tipos de Componentes](#tipos-de-componentes)
- [Buscando Componentes](#buscando-componentes)
- [Propiedades](#propiedades)
- [Tipos de Propiedades](#tipos-de-propiedades)
- [Estado](#estado)
- [Children API](#children-api)
- [Binding](#binding)
- [Eventos](#eventos)
- [Renderizado](#renderizado)
- [Claves](#claves)
- [Referencias](#referencias)
- [Contexto](#contexto)
- [Formularios](#formularios)
- [Controlled Components](#controlled-components)
- [React Ajax](#ajax-en-react)
- [Patrones](#patrones)
- [Gotchas](#gotchas)
- [PATENTES](#patentes)
- [Mixins](#mixins)
- [Internacionalización](#internacionalización)
- [Rendimiento](#rendimiento)
- [Animaciones](#animationes)
- [SVG y React](#svg-y-react)
- [Guias de estilo para React](#guias-de-estilo-para-react)
- [Redux and Mobx](#redux-y-mobx)
- [Añadir React a una Aplicacion existente](#añadir-react-a-una-aplicacion-existente)
- [CSS y React](#css-y-react)
- [Testing](#testing)
- [Contribuyendo a React JS](#contribuyendo-a-react-js)
- [Universal React](#universal-react)
- [Profundizando en React](#profundizando-en-react)
- [React Fiber](#react-fiber)
- [Cursos en Video](#cursos-en-video)
- [Accesibilidad (A11Y)](#Accesibilidad-a11y)
- [Charlas](#charlas)
- [Cursos](#cursos)
- [Libros](#libros)
- [Listas de Correo](#listas-de-correo)
- [Preguntas de entrevistas](#preguntas-de-entrevistas)
- [Herramientas](#herramientas)
- [Renderizado desde el servidor](#renderizado-desde-el-servidor)

# Historia
* [JSConfUS 2013 - Tom Occhino and Jordan Walke: JS Apps at Facebook](https://www.youtube.com/watch?v=GW0rj4sNH2w&index=10&list=PL37ZVnwpeshF7AHpbZt33aW0brYJyNftx) The one where React became #OSS
* [Our First 50,000 Stars](https://facebook.github.io/react/blog/2016/09/28/our-first-50000-stars.html) Vjeux @vjeux

# Creando un Proyecto con React

**¿Cómo creo un nuevo Proyecto con React?**

> Depende de lo que estás buscando. Con/sin configuración, server-rendering etc... aquí hay algunos a considerar. Obviamente, también puedes configurar React desde cero.

* [create-react-app](https://github.com/facebookincubator/create-react-app) No configuration or complicated folder structures, just the files you need to build your app.
* [nwb](https://github.com/insin/nwb) Crea aplicaciones React sin configuración (hasta que lo necesites)
* [next.js](https://github.com/zeit/next.js) A minimalistic framework for universal server-rendered React applications
* [react-server](https://github.com/redfin/react-server) Batteries-included Server-rendered React applications. Note: also see [React 30 -> 002 - Streaming React](https://www.youtube.com/watch?v=XW_c60NCkI4)
* [react-boilerplate](https://github.com/mxstbr/react-boilerplate) A highly scalable, offline-first foundation with the best DX and a focus on performance and best practices
* [create-react-pwa](https://github.com/jeffposnick/create-react-pwa create-react-app) + Progressive Web App goodness
* [gatsby](https://github.com/gatsbyjs/gatsby) Transform plain text into dynamic blogs and websites using React.js

Ver también estos proyectos [projects](https://github.com/facebookincubator/create-react-app#alternatives)

**¿Dónde puedo encontrar videos de como usar 'React Create App'?**

[React Create App + Express](https://www.youtube.com/watch?v=gbVhmaW04bc&feature=youtu.be) @sprjrx @ladyleet


**¿Dónde puedo probar React Online?**

* [extends React.Component style](http://codepen.io/Arney/pen/OXYqWb)
* [React.createClass style](http://codepen.io/Arney/pen/QERoaQ)
* [React JSBin](http://react.jsbin.com/?html,css,js,output)
* [WebpackBin](http://www.webpackbin.com/EkscblgMM)

# ¿Porque usar React?

>
* Componentes Componibles
* Fácil uso en proyectos existentes
* Declarativo
* Funcional / Inmutable


**Es rápido?**
* [¿Es React.js rápido? Más rápido que {framework}? … ¿o más preguntas relevantes que hacer?](https://medium.com/react-weekly/is-react-js-fast-faster-than-framework-or-are-there-more-relevant-questions-to-be-asking-bcf40211f89b#.ll2aubhbi) Jeff Barczewski @jeffbski

**¿Entonces que hace tan bueno a React?**

* [7 puntos fuertes sobre React que todo desarrollador debería saber](https://vacuumlabs.com/blog/7-strengths-of-react-every-programmer-should-know-about) Samuel Hapák @samuha
* [Design Principles](https://facebook.github.io/react/contributing/design-principles.html)

# JSX
**¿Qué es JSX?**

>JSX es un preprocesador que añade sintaxis XML a JavaScript. Puedes perfectamente usar React sin JSX, pero JSX hace React mucho más elegante. - http://buildwithreact.com

* [Tutorial: JSX](http://buildwithreact.com/tutorial/jsx)
* [JSX en Profundidad](https://facebook.github.io/react/docs/jsx-in-depth.html)
* [JSX en React: El otro lado de la moneda](https://medium.com/@housecor/react-s-jsx-the-other-side-of-the-coin-2ace7ab62b98#.i5rmd9h07) Cory House @housecor
* [¿Qué significa JSX?](https://twitter.com/tomocchino/status/769931611303321601) Tom Occhino @tomocchino

**¿Qué hace React realmente por mí?**

[Este es el tipo de cosas que JSX evita que tengas que administrar](https://gist.github.com/insin/8e72bed793772d82ca8d) Jonny Buchanan ‏@jbscript

# El 'Virtual DOM'

>El DOM virtual proporciona una implementación ligera del DOM y del sistema de eventos. En lugar de tratar con el navegador, manipula una versión en memoria del DOM.

**¿Qué es el Virtual DOM?**
* 💯  [El funcionamiento interno del Virtual DOM](https://medium.com/@rajaraodv/the-inner-workings-of-virtual-dom-666ee7ad47cf#.q3jxayda5) @rajaraodv
* [React's diff algorithm](http://calendar.perfplanet.com/2013/diff/) Christopher Chedeau @vjeux
* [La única cosa que nadie explica correctamente sobre React - ¿Por qué el Virtual DOM?](https://hashnode.com/post/the-one-thing-that-no-one-properly-explains-about-react-why-virtual-dom-cisczhfj41bmssp53mvfwmgrq) Sai Kishore Komanduri @saiki
* [Pete Hunt: Los secretos del Virtual DOM de React (FutureJS 2014)](https://www.youtube.com/watch?v=-DX3vJiqxm4)

**¿Todo sobre el Virtual DOM es por la velocidad?**

*No*

Ver :

https://twitter.com/dan_abramov/status/790326092582252544
https://twitter.com/acdlite/status/779693791607336960

> I wonder if we can reclaim the VDOM term to mean "Value DOM", as in Value Type, instead of "Virtual DOM"...? More accurate. **@sebmarkbage**
<hr>
> It doesn't improve perf over hand written DOM code but it's hard to write on scale. React scales well. **@dan_abramov**
<hr>
> React ultimately has to call browser APIs at some point, it can't possibly be faster than writing the same exact calls by hand **@dan_abramov**
<hr>
>React will not do anything that you cannot. By definition everything it does can be reproduced (and some people have with other libraries/frameworks that follow similar conventions). The point is not that React does something that you can't, but rather that by introducing React to your application you are relieved of having to worry about manually handling your DOM, manually determining how to update it efficiently, minimizing traversals, etc. - [Sean Grogg](https://www.quora.com/Is-ReactJS-faster-than-direct-DOM-manipulation-with-JavaScript-or-jQuery)

**Key Takeaway:**

> React keeps your product reasonably fast without you having to think about it all the time, or to jump through the hoops **@dan_abramov**

# Elementos React
> Los elementos son los bloques de construcción más pequeños en las aplicaciones React.
> Los Elementos son los componentes que están "hechos de ..."
— [Documentación de React](https://facebook.github.io/react/docs/rendering-elements.html)

* [Qué hace un 'Elemento' un 'Elemento' vs un componente?](https://twitter.com/timarney/status/790540834466701312) Tim Arney @timarney
* [Entendiendo la diferencia entre un Elemento React y un Componente React](https://quickleft.com/blog/understanding-the-difference-between-react-elements-and-components) Alex Johnson
* [Elementos React vs Componentes React](https://tylermcginnis.com/react-elements-vs-react-components) Tyler McGinnis

# Componentes
> Los Componentes te permiten dividir la interfaz en piezas independientes y reutilizables, y pensar en cada pieza de forma aislada. Conceptualmente, los componentes son como funciones de JavaScript. - [Documentación de React](https://facebook.github.io/react/docs/components-and-props.html)

**¿Cuáles son las mejores prácticas al trabajar con componentes?**

> * Keep it (F)ocused. (Mantenlo enFocado)
* Keep it (I)ndependent. (Mantenlo Independiente)
* Keep it (R)eusable. (Mantenlo Reutilizable)
* Keep it (S)mall. (Mantenlo Pequeño)
* Keep it (T)estable. (Mantenlo Testeable)
* en definitiva, `FIRST`.

> — Addy Osmani https://addyosmani.com/first

Ver :  https://twitter.com/mxstbr/status/790084862954864640 Max Stoiber @mxstbr

# Métodos del Ciclo de Vida

>Los componentes tienen varios "métodos de ciclo de vida" que te permiten anular / ejecutar código en momentos concretos.

**¿Qué son los métodos del ciclo de vida?**

* [Diagrama de los Ciclos de vida de los Componentes React](http://codepen.io/eduardoboucas/full/jqWbdb) Eduardo Bouças @eduardoboucas
* [Ir más allá con los métodos del ciclo de vida de React](https://medium.com/@notrab/going-further-with-react-lifecycle-methods-2ffdc5bdf52c#.bu0ufrosb) Jamie Barton
* [Especificaciones de los Componentes y los Ciclos de Vida](https://facebook.github.io/react/docs/component-specs.html)
* [My #reactjs component lifecycle cheatsheet for quick reference](https://twitter.com/pbesh/status/738008776805060608) Peter Beshai @pbesh
* [Los Ciclos de Vida de los Componentes React](https://medium.com/react-ecosystem/react-components-lifecycle-ce09239010df#.w7v5cw6tk) Osmel Mora @osmel_mora

# Tipos de Componentes
> Hay dos tipos principales de componentes: funcionales y de clase

```
// Componente Funcional
function Welcome(props) {
  return <h1>Hello, {props.name}</h1>;
}

// Componente de Clase

class Welcome extends React.Component {
  render() {
    return <h1>Hello, {this.props.name}</h1>;
  }
}
```

Los componentes se pueden utilizar (compuestos) de muchas maneras, ver los siguientes enlaces para patrones e ideas para la creación de componentes.

**¿Cómo decido qué tipo de Componente utilizar?**

>Se reduce a pocos factores... uno de los principales es decidir lo que un componente debe hacer.
Ver: [Some Thoughts on Function Components in React](https://medium.com/javascript-inside/some-thoughts-on-function-components-in-react-cb2938686bc7#.2oazdyli1) from A. Sharif @sharifsbeat for some help deciding.

También:

* [React.Component vs React.createClass](https://reactjsnews.com/composing-components) Naman Goel & Zach Silveira
* [React.createClass vs extends React.Component](https://toddmotto.com/react-create-class-versus-component) Todd Motto
* [4 tipos de Componentes React diferentes](https://www.peterbe.com/plog/4-different-kinds-of-react-component-styles) Peter Bengtsson @peterbe
* [Funciones como Componentes Hijo (Child Components) y Componentes de alto nivel (Higher Order Components)](http://rea.tech/functions-as-child-components-and-higher-order-components) Ken Ding

**Funciones sin Estado** [```<Código />```](http://reactpatterns.com/#Stateless%20function)

* [Componentes React Funcionales sin Estado: Nueve puntos que pudo haber pasado por alto](https://medium.com/@housecor/react-stateless-functional-components-nine-wins-you-might-have-overlooked-997b0d933dbc#.iydj782xq) Cory House @housecor
* [Adoptando Funciones en React](https://medium.com/javascript-inside/embracing-functions-in-react-d7d558d8bd30#.igvxagy0e) A. Sharif @sharifsbeat

**Presentational and Container Components**  [```<Código />```](http://reactpatterns.com/#Container%20component)

* [Componentes de Presentación y Componentes Contedor](https://medium.com/@dan_abramov/smart-and-dumb-components-7ca2f9a7c7d0#.xo2al5187) Dan Abramov @dan_abramov

**Higher-Order Components** [```<Código />```](http://reactpatterns.com/#Higher-order%20component)

* [ReactCasts #1 - Higher Order Components](https://www.youtube.com/watch?v=LTunyI2Oyzw) Cassio Zen @cassiozen
* [React Higher Order Components in depth](https://medium.com/@franleplant/react-higher-order-components-in-depth-cf9032ee6c3e#.mpb29ree6) @franleplant
* [Higher Order Components: A React Application Design Pattern](https://www.sitepoint.com/react-higher-order-components) Jack Franklin @Jack_Franklin
* [Mixins Are Dead. Long Live Composition](https://medium.com/@dan_abramov/mixins-are-dead-long-live-higher-order-components-94a0d2f9e750#.prpfdo79n) Dan Abramov @dan_abramov
* [Higher Order Components: Theory and Practice](http://engineering.blogfoster.com/higher-order-components-theory-and-practice)
* [Real World Examples of Higher-Order Components](http://rea.tech/reactjs-real-world-examples-of-higher-order-components/) Mehdi Mollaverdi @mehdimollaverdi
* [Start Reacting: HOC](https://www.youtube.com/watch?v=ymJOm5jY1tQ) OliverFencott @OliverFencott

**Función como Componente hijo** [```<Código />```](http://reactpatterns.com/#Function%20as%20children)

* [Función como Componente hijo](https://medium.com/merrickchristensen/function-as-child-components-5f3920a9ace9#.10fbiyqc5) Merrick Christensen @iammerrick
* [I've mentioned this before, but I'm a big fan of child functions in React](https://twitter.com/brian_d_vaughn/status/779362701596164097) Brian Vaughn @brian_d_vaughn
* [He mencionado esto antes, pero soy un gran fan de las funciones hijas en React](https://twitter.com/brian_d_vaughn/status/779362701596164097) Brian Vaughn @brian_d_vaughn

**¿Qué tipos de Componentes hay?**

* [React Component Jargon as of August 2016](https://blog.anthonycomito.com/react-component-jargon-as-of-august-2016-28451d8ceb1d#.a417p5u26) Anthony Comito @a_comito

# Buscando Componentes

**¿Dónde hay buenos sitios para encontrar componentes?**

* [Catálogo de Componentes React](https://github.com/brillout/awesome-react-components)
* [React Rocks](https://react.rocks)

#Propiedades

**¿Qué son las Propiedades?**

>props (abreviatura de propiedades) son la configuración de un Componente, sus opciones si es posible. Son recibidos desde arriba y son inmutables en lo que respecta al Componente que los recibe. - react-guide

Ver : [props vs state](https://github.com/uberVU/react-guide/blob/master/props-vs-state.md)

**¿Cómo puedo pasar Propiedades?**

* [Transfiriendo Propiedades](https://facebook.github.io/react/docs/transferring-props.html)

**¿Cómo paso valores Booleanos?**

* [¿`<Foo bar={true} />` y `<Foo bar>` en JSX es lo mismo?](https://twitter.com/Jack_Franklin/status/768735664485568512) Jack Franklin @Jack_Franklin

**¿Debo usar import, props o context en React?**

* [Diferencias entre require() y pasar un objeto por propiedades o contexto](http://stackoverflow.com/questions/39111775/differences-between-require-and-passing-an-object-via-prop-or-context/39111942) Dan Abramov @dan_abramov

# Tipos de Propiedades

>Los Tipos de propiedades (PropTypes) son esencialmente un diccionario en el que se definen qué propiedades necesita tu componente y de que tipo(s) deben ser. - Niels Gerritsen

**¿Qué son los Tipos de Propiedades?**
* [¿Qué son los Tipos de Propiedades?](https://themeteorchef.com/snippets/what-are-proptypes) Ryan Glover @themeteorchef

**¿Por qué son importantes los Tipos de Propiedades en React?**
* [Porque son importantes los Prototipos en React](http://wecodetheweb.com/2015/06/02/why-react-proptypes-are-important)  Niels Gerritsen @NielsG89

**¿Cómo puedo validar los Tipos de Propiedades?**
* [Mejor validación de Tipos de Propiedades en React](https://medium.com/@MoeSattler/better-prop-validation-in-react-cc83590d311f#.wdhbsrlgj) Moe Sattler @travelperk

# Estado

> En un sentido, "estado" significa la representación visual actual de la aplicación en la pantalla... En el sentido React, el "estado" es un objeto que representa las partes de la aplicación que pueden cambiar. Cada componente puede mantener su propio estado, que vive en un objeto llamado `this.state`. - Dave Ceddia

**¿Qué es el Estado en React?**

* [Guia visual del Estado en React](https://daveceddia.com/visual-guide-to-state-in-react) Dave Ceddia @dceddia

**¿Cómo manejo el estado?**

* [Los 5 Tipos de Estado en una aplicación React](http://jamesknelson.com/5-types-react-application-state) James K Nelson @james_k_nelson
* [State of React #1: A Stateless React App?](http://jamesknelson.com/state-react-1-stateless-react-app) James K Nelson @james_k_nelson
* [A Case for setState](https://medium.com/@zackargyle/a-case-for-setstate-1f1c47cd3f73#.w89epdtmo) Zack Argyle
* [¿Dónde conservo los datos de un Componente React?: state, store, static, and this](https://medium.freecodecamp.com/where-do-i-belong-a-guide-to-saving-react-component-data-in-state-store-static-and-this-c49b335e2a00#.8k7tc37cs) Sam Corcos
* [Como manejar el Estado en React. The missing FAQ](https://medium.com/react-ecosystem/how-to-handle-state-in-react-6f2d3cd73a0c#.dwz84fx9s) Osmel Mora @osmel_mora
* [Should I keep something in React component state? I made a small cheatsheet.](https://twitter.com/dan_abramov/status/749710501916139520) Dan Abramov @dan_abramov
* [Best Practices for Component State in React.js](http://brewhouse.io/blog/2015/03/24/best-practices-for-component-state-in-reactjs.html) Gabe Scholz @gabescholz
* [Exploring React’s State Propagation](https://www.sitepoint.com/exploring-reacts-state-propagation) Eric Greene @ericwgreene

**¿Cómo puedo desacoplar el estado y la interfaz de usuario?**

* [Cómo puedo desacoplar el estado y la interfaz de usuario](https://medium.com/@mweststrate/how-to-decouple-state-and-ui-a-k-a-you-dont-need-componentwillmount-cc90b787aa37#.7l8ji1wer) Michel Weststrate @mweststrate

**Vengo de jQuery... ¿cómo puedo adaptarme mentalmente para trabajar con React / Estado?**
* [Thinking Statefully](https://daveceddia.com/thinking-statefully) Dave Ceddia @dceddia

**I heard you can pass a function to setState when should do that?**
**Escuché que se puede pasar una función a setState ¿cuándo debería hacer eso?**
* [Usando una funció en `setState` en vez de un objeto](https://medium.com/@shopsifter/using-a-function-in-setstate-instead-of-an-object-1f5cfd6e55d1#.h3fokbh9a) Sophia Shoemaker

# Children API

* [ReactCasts #3 - React's Children API](https://www.youtube.com/watch?v=DJ53-G8EbxE) Cassio Zen @cassiozen

# Binding
>El método bind de JavaScript tiene varios usos. Normalmente, se utiliza para preservar el contexto de ejecución de una función que se ejecuta en otro contexto.

**¿Qué debe usar para conectar métodos en Clases React?**
* [To bind or not to bind?](https://twitter.com/dan_abramov/status/790612782471319553) Dan Abramov @dan_abramov
* [fat Arrow vS Autobind VS bind](https://www.reddit.com/r/reactjs/comments/54xnao/fat_arrow_vs_autobind_vs_bindbindbindbindbind/d85wj0l) Dan Abramov @dan_abramov

**¿Qué es eso del "Binding"?**

* [No uses bind cuando pases propiedades](https://daveceddia.com/avoid-bind-when-passing-props) Dave Ceddia
* [5 maneras de manejar el Binding](https://medium.com/@housecor/react-binding-patterns-5-approaches-for-handling-this-92c651b5af56#.4z71l0kmb) Cory House @housecor
* [¿Cómo lidiar con la referencia a `this` dentro de una promesa?](https://www.toptal.com/react/tips-and-practices) Toptal Developers

# Eventos

**¿Cómo funciona el sistema de eventos en React?**

* [Los eventos de React en profundidad](https://www.youtube.com/watch?v=dRo_egw7tBc) Kent C. Dodds, Ben Alpert, & Dan Abramov

# Renderizado

**¿Qué debe ir en la función de render?**

* [La respuesta es devolver algo (return) lo antes posible](https://medium.com/@SimonRadionov/return-as-soon-as-you-know-the-answer-dec6369b9b67#.82kxymyki) @SimonRadionov

# Claves
>React utiliza las Claves ([keys](https://facebook.github.io/react/docs/reconciliation.html#keys)) para ayudar con la reconciliación (es decir, cómo calcula la diferencia del DOM para cada procesamiento).

```
<ul>
  <li key="2015">Duke</li>
  <li key="2016">Villanova</li>
</ul>
```

**¿Por qué no puedo poner la key en las propiedades (o definir el valor predeterminado en otro lugar)?**

* [¿Por qué no puedo poner la clave en las Propiedades por defecto](https://www.reddit.com/r/reactjs/comments/4mjdcf/why_cant_i_put_key_in_default_props_or_define_the/d3xwa6m)

**¿Qué debo utilizar para una key?**

* [Index as a key is an anti-pattern](https://medium.com/@robinpokorny/index-as-a-key-is-an-anti-pattern-e0349aece318#.y4ru46ikc) Robin Pokorný @robinpokorny

**¿Cuáles son algunos ejemplos en los que debería cambiar manualmente una key?**

* [The key is using key](https://twitter.com/timarney/status/730785238654287873) Tim Arney @timarney

# Referencias

>El atributo `ref` permite guardar una referencia a un elemento React específico o a un componente devuelto por la función `render()`. Esto puede ser valioso cuando se necesita una referencia, desde dentro de un componente, a algún elemento o componente contenido en la función `render()`. - reactenlightenment.com

**¿Qué son las Referencias (refs) y porqué las Referencias de tipo String son malas?**

* [Refs to Components](https://facebook.github.io/react/docs/more-about-refs.html)
* [Why do you use findDOMNode()?](https://twitter.com/dan_abramov/status/752936646602031104) Dan Abramov @dan_abramov
* [String refs are bad in quite a few ways](https://news.ycombinator.com/edit?id=12093234) Dan Abramov @dan_abramov

# Contexto

⚠️ El contexto es una **característica avanzada y experimental**. Es probable que la API cambie en futuras versiones. Los rumores de su existencia son verdaderos pero ten cuidado!

* [ReactCasts #4 - Context (Part 1)](https://www.youtube.com/watch?v=lxq938kqIss&t=1s) Cassio Zen @cassiozen
* [ReactCasts #5 - Context (Part 2)](https://www.youtube.com/watch?v=mwYHDXS6uSc&feature=youtu.be) Cassio Zen @cassiozen
* [How to handle React context in a reliable way](https://medium.com/react-ecosystem/how-to-handle-react-context-a7592dfdcbc#.rtwgxxy0d) Osmel Mora @osmel_mora
* [How to safely use React context](https://medium.com/@mweststrate/how-to-safely-use-react-context-b7e343eff076#.m6v9tsgub) Michel Weststrate @mweststrate
* [Context all the things with React](https://www.youtube.com/watch?v=k9AhBMwj1w4) Stephen Rivas Jr. (@sprjrx)

# Formularios

**¿Cómo puedo crear formularios con React?**

* [Learn Raw React: Ridiculously Simple Forms](http://jamesknelson.com/learn-raw-react-ridiculously-simple-forms) James K Nelson @james_k_nelson

**¿Cómo puedo validar la entrada de formularios?**
* [Elegant Form Validation Using React](https://spin.atomicobject.com/2016/10/05/form-validation-react) Jordan Schaenzle
* [Building validated forms with great UX in React](https://youtu.be/1Urj4TZ5BLI?t=2437) Marcela Hrdá
* [react-validation](https://github.com/vacuumlabs/react-validation)


# Controlled Components

**What is a controlled component?**

Via Loren Stewart @lorenstewart111 [React.js Forms: Controlled Components](http://lorenstewart.me/2016/10/31/react-js-forms-controlled-components)

>A controlled component has two aspects:

1. Controlled components have functions to govern the data going into them on every onChange event, rather than grabbing the data only once, e.g. when a user clicks a submit button. This 'governed' data is then saved to state (in this case, the parent/container component's state).

2. Data displayed by a controlled component is received through props passed down from it's parent/container component.

> This is a one-way loop – from (1) child component input (2) to parent component state and (3) back down to the child component via props – is what is meant by unidirectional data flow in React.js application architecture.

# Ajax en React

**¿Cuál es la mejor práctica para obtener datos de servidor en los componentes React?**
>Depende! Ver: [React AJAX Best Practices](http://andrewhfarmer.com/react-ajax-best-practices) Andrew H Farmer @ahfarmer

* [Carga y uso de datos externos con React](http://mediatemple.net/blog/tips/loading-and-using-external-data-in-react) Chris Coyier @chriscoyier

# Patrones

* [Patrones en React](http://reactpatterns.com) @chantastic
* [React.js in patterns](http://krasimirtsonev.com/blog/article/react-js-in-design-patterns) Krasimir Tsonev
* [Patterns For Style Composition In React](http://jxnblk.com/writing/posts/patterns-for-style-composition-in-react) Brent Jackson @jxnblk
* [Haz tus Componentes de React bonitos](https://medium.com/walmartlabs/make-your-react-components-pretty-a1ae4ec0f56e#.ctwfvx379) Mark Brouch @markbrouch

# Gotchas

**¿Qué son los Gotchas en React?**

* [React Gotchas](https://daveceddia.com/react-gotchas) Dave Ceddia @dceddia 
* [How to Render Components Outside the Main ReactJS App](https://blog.komand.com/how-to-render-components-outside-the-main-react-app)
* [Watch Out for Undefined State](https://daveceddia.com/watch-out-for-undefined-state) Dave Ceddia @dceddia 

# PATENTES

**¿Qué es todo eso que escucho sobre la cláusula de PATENTES de Facebook?**

* [Some links to point people to when they misinterpret PATENTS clause or spread false claims](https://gist.github.com/gaearon/df0c4025e67399af72786d7ac7c819cc) Dan Abramov @dan_abramov
* [React’s license: necessary and open?](http://lu.is/blog/2016/10/31/reacts-license-necessary-and-open) Luis Villa @luis_in_140

# Mixins

**¿Por qué los Mixins se consideran perjudiciales?**

* [Mixins Considered Harmful](https://facebook.github.io/react/blog/2016/07/13/mixins-considered-harmful.html) Dan Abramov @dan_abramov

# Internacionalización

**¿Cómo debo manejar la internacionalización?**

* [Internacionalización en React](https://medium.freecodecamp.com/internationalization-in-react-7264738274a0#.bcfxgycwv) Preethi Kasireddy

**¿Qué repositorios existen para la internacionalización?**
* [react-intl](https://github.com/yahoo/react-intl)
* [react-localize](https://github.com/sprjr/react-localize) @sprjrx

# Librerías de terceros

**¿Cómo utilizo Librerías de terceros?**

* [Integración con Librerías de terceros](https://www.youtube.com/watch?v=GWVjMHDKSfU&feature=youtu.be&a) Rally Coding

# Rendimiento

**¿Cómo puedo hacer que mi aplicación sea más rápida?**

* [Component Rendering Performance in React](https://medium.com/modus-create-front-end-development/component-rendering-performance-in-react-df859b474adc#.gvyat7vkb) Grgur Grisogono
* [Don‘t use PureComponent everywhere. Measure](https://twitter.com/dan_abramov/status/759383530120110080) Dan Abramov @dan_abramov
* [React.js pure render performance anti-pattern](https://medium.com/@esamatti/react-js-pure-render-performance-anti-pattern-fb88c101332f#.hewsz120q)
* [Should I use shouldComponentUpdate?](http://jamesknelson.com/should-i-use-shouldcomponentupdate) James K Nelson @james_k_nelson
* [Reconciliation](https://facebook.github.io/react/docs/reconciliation.html)
* [Quick slides on #reactjs performance](http://presentations.survivejs.com/react-performance/#/?_k=ivqhoe) Juho Vepsäläinen @bebraw

# Animaciones

**¿Cómo animo cosas en React?**

* 🔥 💯 [Animando en React](https://youtu.be/Fk--XUEorvc?t=2344 Sarah Drasner) @sarah_edo
* [Animaciones de la interfaz de usuario con React - El camino correcto](https://medium.com/@joethedave/achieving-ui-animations-with-react-the-right-way-562fa8a91935#.g8qmlz5d6) Joe Davis
* [Animaciones con ReactTransitionGroup](https://medium.com/@cheapsteak/animations-with-reacttransitiongroup-4972ad7da286#.qmrksnixv) Chang Wang @CheapSteak

**¿Hay alguna API declarativa para animaciones?**

* [React Motion](https://github.com/chenglou/react-motion)
* [Una pequeña introducción a React Motion](https://medium.com/@nashvail/a-gentle-introduction-to-react-motion-dc50dd9f2459#.aio7blbsi)

**¿Cómo puedo animar las transiciones de página?**

* [React Page Transition Animations](https://medium.com/front-end-hacking/react-page-transition-animations-9d18c90a9831#.lc9943ajq) Huan Ji

**¿Cuáles son algunos de los mejores repositorios sobre animación en React?**
* [react-animations](https://github.com/FormidableLabs/react-animations)
* [react-anime](https://github.com/stelatech/react-anime)
* [react-motion](https://github.com/chenglou/react-motion)
* [velocity-react](https://github.com/twitter-fabric/velocity-react)
* [state-transitions](https://github.com/jacobp100/state-transitions)
* [react-tween](https://github.com/clari/react-tween)

# SVG y React

**¿Cómo trabajo con SVG en React?**

* [Icons as React Components](https://medium.com/@david.gilbertson/icons-as-react-components-de3e33cb8792#.lmbz3v9ic)
* [Creating an SVG Icon System with React](https://css-tricks.com/creating-svg-icon-system-react) @sarah_edo

# Guías de estilo para React

**¿Dónde puedo encontrar buenas guías de estilo para React?**

* [Eventbrite React & JSX Coding Style Guide](https://github.com/eventbrite/javascript/tree/master/react)
* [Airbnb React/JSX Style Guide](https://github.com/airbnb/javascript/tree/master/react)


# Redux y Mobx

**¿Qué es (Redux/Mobx)?**

* [Confundido! ¿Redux o MobX?](https://www.reddit.com/r/reactjs/comments/4npzq5/confused_redux_or_mobx)

**¿Necesito usar (Redux/Mobx)?**

* [You don’t need Redux if your data never changes. The whole point of it is managing changes.](https://twitter.com/dan_abramov/status/737036433215610880) Dan Abramov @dan_abramov
* [You Might Not Need Redux](https://medium.com/@dan_abramov/you-might-not-need-redux-be46360cf367#.kgnqdp8p6) Dan Abramov @dan_abramov
* [Redux or MobX: An attempt to dissolve the Confusion](http://www.robinwieruch.de/redux-mobx-confusion/) Robin Wieruch @rwieruch

**¿Cómo escalar aplicaciones React-Redux?**

* [About folder structure, styling, data fetching, etc.](https://www.smashingmagazine.com/2016/09/how-to-scale-react-applications/) Max Stoiber @mxstbr
* [Acerca de la estructura de carpetas, estilo, extracción de datos, etc.](https://www.smashingmagazine.com/2016/09/how-to-scale-react-applications/) Max Stoiber @mxstbr

# Añadir React a una Aplicación existente

**¿Cómo empiezo a integrar React en una aplicación existente?**

* [How to Sprinkle ReactJS into an Existing Web Application](https://scotch.io/tutorials/how-to-sprinkle-reactjs-into-an-existing-web-application) Andrew Del Prete @andrewdelprete
* [Don't Rewrite, React!](https://www.youtube.com/watch?v=BF58ZJ1ZQxY) Ryan Florence
* [Migrar con seguridad a React](https://www.youtube.com/watch?v=sXDZBxbRRag&list=PLNBNS7NRGKMG3uLrm5fgY02hJ87Wzb4IU&index=1) Jamis Charles

# CSS y React
* Ver esto: 🔥 💯 [Styling React.JS applications](https://www.youtube.com/watch?v=19gqsBc_Cx0) Max Stoiber @mxstbr

**¿Qué pasa con los estilos en React?**

Puedes utilizar CSS simple o cualquier preprocesador (Sass, Less etc ...) con React. React genera marcado HTML estándar, así técnicamente puedes seguir haciendo lo que has estado haciendo hasta ahora.

> El uso de CSS para diseñar nuestro contenido de React es muy sencillo. Debido a que React termina generando las etiquetas HTML habituales, todos los trucos CSS que has aprendido a lo largo de los años para dar estilo al HTML siguen aplicándose. -  kirupa

* [What to use for React styling? ](http://andrewhfarmer.com/how-to-style-react) Andrew H Farmer
* [Styling React](http://survivejs.com/react/advanced-techniques/styling-react) survivejs.com
* [Styling in React](https://www.kirupa.com/react/styling_in_react.htm) kirupa
* [Styling React Components in JavaScript](https://www.youtube.com/watch?v=0aBv8dsZs84) Michael Chan


**¿Puedo Utilizar Bootstrap con React?**
* [React-Bootstrap](https://react-bootstrap.github.io) - Componentes Bootstrap 3 components hechos con React
* [bootstrap-loader](https://github.com/shakacode/bootstrap-loader) - Carga los estilos y scripts de Bootstrap con Webpack

### Dando estilos a nivel de Componente

>  Existen varios enfoques para React que nos permiten dar estilos a nivel de componente. - survivejs.com

**¿Qué repositorios debo revisar para dar estilo a nivel de componentes?**

* [styled-components](https://github.com/styled-components/styled-components) + [Styling React Applications](https://youtu.be/1Urj4TZ5BLI) @mxstbr 
* [glamor](https://github.com/threepointone/glamor) @threepointone
* [aphrodite](https://github.com/Khan/aphrodite)- Khan Academy

Nota: ver también - [Styled components o Glamor?](https://www.reddit.com/r/reactjs/comments/5eq8ew/styled_components_or_glamor)


**Cual es la diferencia entre "estilos en línea" y “CSS-in-JS”?**
* [Writing your styles in JS ≠ writing inline styles](http://mxstbr.blog/2016/11/inline-styles-vs-css-in-js) Max Stoiber @mxstbr

**Solo necesito dar unos estilos en línea simples... ¿Cuál es la manera más sencilla de utilizar para dar estilos en línea en React?**

* [React Docs, estilos en línea](https://facebook.github.io/react/docs/dom-elements.html#style)
* [classnames](https://github.com/JedWatson/classnames) - A simple javascript utility for conditionally joining classNames together. @JedWatson

**¿Qué recursos están disponibles para ver los pros y los contras de los estilos en línea y CSS en JS?**
* [PANEL ON 'INLINE STYLES'](http://shoptalkshow.com/episodes/180-panel-on-inline-styles) @ShopTalkShow
* [CSS en JS puede que no sea la solución a todos sus problemas](https://blog.grommet.io/post/2016/08/10/css-in-js-may-not-be-the-solution-to-all-your-problems) Alan Souza
* [CSS in JS + CSS Modules](http://www.dadsindev.com/12)@dadsindev
* [CSS in JS tech chat](https://www.youtube.com/watch?v=BXOF_8jDdf8) Kent C. Dodds & Sarah Drasner

**¿Qué hay sobre CSS Modules para dar estilos?**
* [css-modules](https://github.com/css-modules/css-modules) @markdalgleish
* [CSS Modules con ejemplos](http://andrewhfarmer.com/css-modules-by-example) Andrew H Farmer

**Hay demasiadas opciones sobre CSS en JS ¿Como puedo compararlas?** 
* [React: CSS en JS, comparativa de técnicas](https://github.com/MicheleBertoli/css-in-js) Michele Bertoli @MicheleBertoli
* [Comparativa de Librerías "CSS en JS" en React](https://github.com/FormidableLabs/radium/tree/master/docs/comparison - radium)

**¿Cómo puedo diseñar un componente que sea muy reutilizable y personalizable?**
* [Reusable React Component with Overridable Inline CSS Styles](http://staxmanade.com/2016/06/reusable-react-component-with-overridable-inline-css-styles/)

# Testing

* [Testeando Aplicaciones React](https://www.youtube.com/watch?v=eWN8F_WOBAQ) Jack Franklin
* [La gente parece reírse de esto, pero creo que es realmente bastante razonable](https://twitter.com/dan_abramov/status/762257231471579136) Dan Abramov @dan_abramov

# Contribuyendo a React JS

**¿Dónde puedo aprender sobre cómo contribuir a React JS?**

* [Contribuyendo a React JS](https://www.youtube.com/watch?v=wUpPsEcGsg8) Kent C. Dodds

# Universal React

* [React en el Servidor para principiantes](https://scotch.io/tutorials/react-on-the-server-for-beginners-build-a-universal-react-and-node-app) Luciano Mammino @loige

# Profundizando en React
* [Notas de implementación - Cómo funciona realmente React](https://facebook.github.io/react/contributing/implementation-notes.html) Dan Abramov @dan_abramov
* [Construyendo una Aplicación React desde 0](https://www.youtube.com/watch?v=_MAD4Oly9yg) Paul O'Shannessy @zpao
* [React Architecture – OSCON](http://blog.vjeux.com/2014/javascript/react-architecture-oscon.html) Christopher Chedeau @vjeux
* [ReactJS: Bajo el capó](https://www.youtube.com/watch?v=xsKYAa1ZXpQ) Boris Dinkevich @BorisDinkevich
* [REACT INTERNALS](https://zackargyle.github.io/react-internals-slides/#/?_k=7f19z9) Zack Argyle @ZackArgyle

# React Fiber

**¿Qué, por qué y cómo?**
* [Why, What, and How of React Fiber with Dan Abramov and Andrew Clark](https://youtu.be/crM1iRVGpGQ?list=PLV5CVI1eNcJi8sor_aQ2AzOeQ3On3suOr)

**¿Qué es React Fiber?**

* Experimental - [React Fiber Architecture](https://github.com/acdlite/react-fiber-architecture) Andrew Clark @acdlite
* Experimental - [What's Next for React](https://www.youtube.com/watch?v=aV1271hd9ew) Andrew Clark @acdlite

**¿Está listo React Fiber?**
* http://isfiberreadyyet.com

**¿Cómo puedo contribuir a Fiber?**
* [Fiber Principles: Contributing To Fiber](https://github.com/facebook/react/issues/7942)

# Cursos en Video

**¿Hay buenos recursos de video/cursos para aprender React?**

* https://egghead.io/courses/react-fundamentals GRATIS (+ otros de pago)
* https://reactforbeginners.com
* https://app.pluralsight.com/courses/react-redux-react-router-es6
* https://www.pluralsight.com/courses/react-flux-building-applications
* https://frontendmasters.com/courses/react-intro (they have a bunch)
* http://courses.reactjsprogram.com/courses/reactjsprogrambundle
* https://LearnRedux.com
* https://egghead.io/courses/manage-complex-state-in-react-apps-with-mobx
* https://www.udemy.com/react-redux
* https://www.awesomereact.com

Ver también [Videos de Conferencias](https://www.awesomereact.com/conferences)

# Accesibilidad (A11Y)

**¿Qué pasa con la accesibilidad?**

* [Cómo diseñar para la accesibilidad](http://www.bbc.co.uk/gel/guidelines/how-to-design-for-accessibility) *Note:* not specific to React but a solid primer on the topic

<hr>

**¿Cómo manejo la accesibilidad en React?**
* [Excerpt from React.js Conf 2015 - Hype!](https://www.youtube.com/watch?v=z5e7kWSHWTg#t=631) Ryan Florence
* [Bringing the Web Back to the Blind by Ryan Florence ](https://www.youtube.com/watch?v=YuzS-g6Qvq8) *Nota:* no es específico de React, sino un principio sólido sobre el tema.

# Charlas
* [React to the Future - Slide Deck](http://elijahmanor.com/talks/react-to-the-future/dist) Elijah Manor @elijahmanor
* [React Things - PDF Slides](https://react.rocks/blog/images/React_Intro_sept_2016.pdf) Jeff Winkler @winkler1

# Cursos

**¿Dónde puedo tener cursos sobre React?**
<hr>

*Micheal Jackson* @mjackson & *Ryan Florence* @ryanflorence

* https://reactjs-training.com

<hr>
*Brian Holt* @holtbt

* https://btholt.github.io/es6-react-pres
* https://btholt.github.io/complete-intro-to-react
* https://github.com/btholt/react-redux-workshop

# Libros

**¿Dónde puedo encontrar buenos libros sobre React?**

* [React Enlightenment ](http://www.reactenlightenment.com) Cody Lindley @codylindley
* [Build your first real world React.js application](http://academy.plot.ly/#react) Max Stoiber @mxstbr
* [SurviveJS React](http://survivejs.com/react/introduction)
* [Fullstack React](https://www.fullstackreact.com)

# Listas de Correo

**¿Dónde puedo encontrar listas de correo sobre React?**

* [React.js Newsletter](http://reactjsnewsletter.com)
* [React Status](http://react.statuscode.com)
* [Fullstack React](http://newsletter.fullstackreact.com)
* [This Week In React](https://thisweekinreact.com)
* [React Digest](http://reactdigest.net)

# Preguntas de entrevistas

* [12 preguntas esenciales en una entrevista de React.js](https://www.toptal.com/react/interview-questions)
* [React Interview Questions](https://github.com/eltonjuan/react-interview-questions/blob/master/ReactInterviewQuestions.md)
* [quiz.md](https://gist.github.com/gaearon/8fa9fdd2c4197ee0b52894877bf587a4) Dan Abramov @dan_abramov
* [5 Essential React.js Interview Questions](https://www.codementor.io/reactjs/tutorial/5-essential-reactjs-interview-questions)
* [The Vital Guide to React.js Interviewing](https://chandanpandey.com/2016/10/27/the-vital-guide-to-react-js-interviewing)
* [React Interview Questions](https://tylermcginnis.com/react-interview-questions) Tyler McGinnis @tylermcginnis33

# Herramientas

**¿Qué herramientas para desarrolladores hay disponibles para React?**

* [StoryBook](https://getstorybook.io/)  (A visual way to develop your UI components. Show them in different states and develop them interactively).  `Ver` [Ejemplo StoryBook](http://airbnb.io/react-dates/) +  [React Storybooks meets Create React App](https://voice.kadira.io/react-storybooks-meets-create-react-app-ac8a3f32cc79#.fcah86vcb)
* [React Developer Tools](https://facebook.github.io/react/blog/2015/09/02/new-react-developer-tools.html)
* [why-did-you-update](https://github.com/garbles/why-did-you-update) - Puts your console on blast when React is making unnecessary updates.
* [Herramientas de rendimiento](https://facebook.github.io/react/docs/perf.html)

# Renderizado desde el servidor

**¿Necesito renderizado desde el servidor (Server-Side Rendering)?**
* [Should I use React Server-Side Rendering?](http://andrewhfarmer.com/server-side-render/)
