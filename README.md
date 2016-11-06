# React - Preguntas Frecuentes

Esta guía pretende reunir contenido de calidad sobre los conceptos básicos de React en una solo sitio para una rápida referencia.

Recuerda que todos estamos aprendiendo. Lea, haz pruebas, ensucie (está bien).

## Contenido

- [Comienzo](#start)
- [Historia](#history)
- [Creando un Proyecto con React](#creating-a-react-project)
- [¿Porque usar React?](#why-use-react)
- [JSX](#jsx)
- [El 'Virtual DOM'](#the-virtual-dom)
- [Elementos React](#react-elements)
- [Componentes](#components)
- [Métodos del Ciclo de Vida](#lifecycle-methods)º
- [Tipos de Componentes](#component-types)
- [Buscando Componentes](#finding-components)
- [Propiedades](#props)
- [Prototipos](#proptypes)
- [Estado](#state)
- [Binding](#binding)
- [Eventos](#events)
- [Renderizado](#rendering)
- [Keys](#keys)
- [Refs](#refs)
- [Contexto](#context)
- [Formularios](#forms)
- [Controlled Components](#controlled-components)
- [React Ajax](#react-ajax)
- [Patrones](#patterns)
- [Gotchas](#gotchas)
- [PATENTES](#patents)
- [Mixins](#mixins)
- [Internacionalización](#internationalization)
- [Rendimiento](#performance)
- [Animacioness](#animations)
- [SVG & React](#svg--react)
- [Guias de estilo para React](#react-style-guides)
- [Redux and Mobx](#redux-and-mobx)
- [Añadir React a una Aplicacion existente](#adding-react-to-an-existing-app)
- [CSS y React](#css-and-react)
- [Testing](#testing)
- [Vídeos de Conferencias](#conference-videos)
- [Contribuyendo a React JS](#contributing-to-react-js)
- [Universal React](#universal-react)
- [Deep Dive](#deep-dive)
- [React Fiber](#react-fiber)
- [Cursos en Video](#video-courses)
- [A11Y](#a11y)
- [Charlas](#talks)
- [Entrenamiento](#training)
- [Libros](#books)
- [Listas de Correo](#newsletters)
- [Preguntas de entrevistas](#interview-questions)


#Comienzo

**No sé nada de React, ¿que debería ver / leer antes de empezar?**
* [Documentación Oficial de React](https://facebook.github.io/react/docs/hello-world.html)
* [Pensando en React - Pete Hunt](https://facebook.github.io/react/docs/thinking-in-react.html)
* [Pete Hunt: React: Rethinking best practices (JSConf EU 2013)](https://www.youtube.com/watch?v=x7cQ3mrcKaY)
* 🔥 [Todas las cosas terribles que hice la primera vez que escribí una Aplicación Compleja con React ](https://youtu.be/Fk--XUEorvc?t=20666) Raquel @raquelxmoss
* [Enseñando React sin usar React](https://medium.com/@ericclemmons/teaching-react-without-using-react-a4b87cfd4e87#.q8cyvryw1) Eric Clemmons @ericclemmons
* [React en 7 Minutos](https://egghead.io/lessons/react-react-in-7-minutes) es un poco antiguo, pero es un buen comienzo
* [Introducción to React](https://mva.microsoft.com/en-US/training-courses/introduction-to-react-16635?l=4wrKgdJrC_206218965) Eric W. Greene / Microsoft Virtual Academy
* [Libros](#books)

#Historia
* [JSConfUS 2013 - Tom Occhino and Jordan Walke: JS Apps at Facebook](https://www.youtube.com/watch?v=GW0rj4sNH2w&index=10&list=PL37ZVnwpeshF7AHpbZt33aW0brYJyNftx) The one where React became #OSS
* [Our First 50,000 Stars](https://facebook.github.io/react/blog/2016/09/28/our-first-50000-stars.html) Vjeux @vjeux

#Creando un Proyecto con React

**¿Como creo un nuevo Proyecto con React?**

* 💯 [create-react-app](https://github.com/facebookincubator/create-react-app)
* [nwb](https://github.com/insin/nwb) si necesitas más control sobre la configuración

**¿Donde puedo encontrar videos de como usar 'React Create App'?**

[React Create App + Express](https://www.youtube.com/watch?v=gbVhmaW04bc&feature=youtu.be) @sprjrx @ladyleet


**Can I play around with React Online?**
**¿Donde puedo probar React Online?**

* [extends React.Component style](http://codepen.io/Arney/pen/OXYqWb)
* [React.createClass style](http://codepen.io/Arney/pen/QERoaQ)
* [React JSBin](http://react.jsbin.com/?html,css,js,output)

#¿Porque usar React?

>
* Componentes Componibles
* Fácil uso en proyectos existentes
* Declarativo
* Funcional / Immutable friendly


**Es rápido?**
* [¿Es React.js rápido? Más rápido que {framework}? … ¿o más preguntas relevantes que hacer?](https://medium.com/react-weekly/is-react-js-fast-faster-than-framework-or-are-there-more-relevant-questions-to-be-asking-bcf40211f89b#.ll2aubhbi) Jeff Barczewski @jeffbski

**¿Entonces que hace tan bueno a React?**

* [7 puntos fuertes sobre React que todo desarrollador debería saber](https://vacuumlabs.com/blog/7-strengths-of-react-every-programmer-should-know-about) Samuel Hapák @samuha
* [Design Principles](https://facebook.github.io/react/contributing/design-principles.html)

#JSX
**¿Qué es JSX?**

>JSX es un preprocesador que añade sintaxis XML a JavaScript. Puedes perfectamente usar React sin JSX, pero JSX hace React mucho más elegante. - http://buildwithreact.com

* [Tutorial: JSX](http://buildwithreact.com/tutorial/jsx)
* [JSX en Profundidad](https://facebook.github.io/react/docs/jsx-in-depth.html)
* [JSX en React: El otro lado de la moneda](https://medium.com/@housecor/react-s-jsx-the-other-side-of-the-coin-2ace7ab62b98#.i5rmd9h07) Cory House @housecor
* [¿Qué significa JSX?](https://twitter.com/tomocchino/status/769931611303321601) Tom Occhino @tomocchino

**¿Qué hace React realmente por mí?**

[Este es el tipo de cosas que JSX evita que tengas que administrar](https://gist.github.com/insin/8e72bed793772d82ca8d) Jonny Buchanan ‏@jbscript

#El 'Virtual DOM'

>El DOM virtual proporciona una implementación ligera del DOM y del sistema de eventos. En lugar de tratar con el navegador, manipula una versión en memoria del DOM.

**¿Qué es el Virtual DOM?**
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

#Elementos React
> Los elementos son los bloques de construcción más pequeños en las aplicaciones de React.
> Los Elementos son los componentes que están "hechos de ..."
— [Documentación de React](https://facebook.github.io/react/docs/rendering-elements.html)

* [Qué hace un 'Elemento' un 'Elemento' vs un componente?](https://twitter.com/timarney/status/790540834466701312) Tim Arney @timarney
* [Entendiendo la diferencia entre un Elemento React y un Componente React](https://quickleft.com/blog/understanding-the-difference-between-react-elements-and-components) Alex Johnson

#Componentes
> Los Componentes te permiten dividir la interfaz en piezas independientes y reutilizables,y pensar en cada pieza de forma aislada. Conceptualmente, los componentes son como funciones de JavaScript. - [Documentación de React](https://facebook.github.io/react/docs/components-and-props.html)

**¿Cuáles son las mejores prácticas al trabajar con componentes?**

> * Keep it (F)ocused. (Mantenlo enFocado)
* Keep it (I)ndependent. (Mantenlo Independiente)
* Keep it (R)eusable. (Mantenlo Reutilizable)
* Keep it (S)mall. (Mantenlo Pequeño)
* Keep it (T)estable. (Mantenlo Testeable)
* en definitiva, `FIRST`.

> — Addy Osmani https://addyosmani.com/first

Ver :  https://twitter.com/mxstbr/status/790084862954864640 Max Stoiber @mxstbr

#Métodos del Ciclo de Vida

>Los componentes tienen varios "métodos de ciclo de vida" que le permiten anular / ejecutar código en momentos concretos.

**¿Qué son los métodos del ciclo de vida?**

* [Diagrama de los Ciclos de vida de los Componentes de React](http://codepen.io/eduardoboucas/full/jqWbdb) Eduardo Bouças @eduardoboucas
* [Ir más allá con los métodos del ciclo de vida de React](https://medium.com/@notrab/going-further-with-react-lifecycle-methods-2ffdc5bdf52c#.bu0ufrosb) Jamie Barton
* [Especificaciones de los Componentes y los Ciclos de Vida](https://facebook.github.io/react/docs/component-specs.html)
* [My #reactjs component lifecycle cheatsheet for quick reference](https://twitter.com/pbesh/status/738008776805060608) Peter Beshai @pbesh
* [Los Ciclos de Vida de los Componentes React](https://medium.com/react-ecosystem/react-components-lifecycle-ce09239010df#.w7v5cw6tk) Osmel Mora @osmel_mora

#Tipos de Componentes
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

* [React.Component vs React.createClass](https://reactjsnews.com/composing-components) Naman Goel & Zach Silveira
* [React.createClass vs extends React.Component](https://toddmotto.com/react-create-class-versus-component) Todd Motto
* [4 tipos de Componentes React diferentes](https://www.peterbe.com/plog/4-different-kinds-of-react-component-styles) Peter Bengtsson @peterbe
* [Functions as Child Components and Higher Order Components](http://rea.tech/functions-as-child-components-and-higher-order-components) Ken Ding

**Functiones sin Estado** [```<Código />```](http://reactpatterns.com/#Stateless%20function)

* [Componentes React Funcionales sin Estado: Nueve puntos que pudo haber pasado por alto](https://medium.com/@housecor/react-stateless-functional-components-nine-wins-you-might-have-overlooked-997b0d933dbc#.iydj782xq) Cory House @housecor
* [Abrazando Functiones en React](https://medium.com/javascript-inside/embracing-functions-in-react-d7d558d8bd30#.igvxagy0e) A. Sharif @sharifsbeat

**Presentational and Container Components**  [```<Código />```](http://reactpatterns.com/#Container%20component)

* [Componentes de Presentación y Componentes Contedor](https://medium.com/@dan_abramov/smart-and-dumb-components-7ca2f9a7c7d0#.xo2al5187) Dan Abramov @dan_abramov

**Higher-Order Components** [```<Código />```](http://reactpatterns.com/#Higher-order%20component)

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

**¿Qué tipos de componentes hay?**

* [React Component Jargon as of August 2016](https://blog.anthonycomito.com/react-component-jargon-as-of-august-2016-28451d8ceb1d#.a417p5u26) Anthony Comito @a_comito

#Buscando Componentes

**¿Dónde hay buenos sitios para encontrar componentes?**

* [Catálogo de Componentes React](https://github.com/brillout/awesome-react-components)
* [React Rocks](https://react.rocks)

#Propiedades

**¿Qué son las Propiedades?**
>props (abreviatura de  propiedades) son la configuración de un Componente,  sus opciones si es posible. Son recibidos desde arriba y son inmutables en lo que respecta al Componente que los recibe. - react-guide

Ver : [props vs state](https://github.com/uberVU/react-guide/blob/master/props-vs-state.md)

**¿Como puedo pasar Propiedades?**

* [Transfiriendo Props](https://facebook.github.io/react/docs/transferring-props.html)

**¿Como paso valores Booleanos?**

* [¿`<Foo bar={true} />` y `<Foo bar>` en JSX es lo mismo?](https://twitter.com/Jack_Franklin/status/768735664485568512) Jack Franklin @Jack_Franklin

**¿Debo usar import, props o context en React?**

* [Diferencias entre require() y pasar un objeto por propiedades o contexto](http://stackoverflow.com/questions/39111775/differences-between-require-and-passing-an-object-via-prop-or-context/39111942) Dan Abramov @dan_abramov

#Prototipos

>Los Prototipos (PropTypes) son esencialmente un diccionario en el que se definen qué propiedades necesita su componente y de que tipo(s) deben ser. - Niels Gerritsen

**¿Qué son los Prototipos?**
* [¿Qué son los Prototipos?](https://themeteorchef.com/snippets/what-are-proptypes) Ryan Glover @themeteorchef

**¿Por qué son importantes los Prototipos en React?**
* [Porque son importantes los Prototipos en React](http://wecodetheweb.com/2015/06/02/why-react-proptypes-are-important)  Niels Gerritsen @NielsG89

**¿Cómo puedo validar Propiedades?**
* [Mejor validación de Propiedades en React](https://medium.com/@MoeSattler/better-prop-validation-in-react-cc83590d311f#.wdhbsrlgj) Moe Sattler @travelperk

#Estado

> En un sentido, "estado" significa la representación visual actual de la aplicación en la pantalla... En el sentido React, el "estado" es un objeto que representa las partes de la aplicación que pueden cambiar. Cada componente puede mantener su propio estado, que vive en un objeto llamado this.state. - Dave Ceddia

**¿Qué es el Estado en React?**

* [Guia visual del Estado en React](https://daveceddia.com/visual-guide-to-state-in-react) Dave Ceddia @dceddia

**¿Cómo manejo el estado?**

* [Los 5 Tipos de Estado en una aplicación React](http://jamesknelson.com/5-types-react-application-state) James K Nelson @james_k_nelson
* [State of React #1: A Stateless React App?](http://jamesknelson.com/state-react-1-stateless-react-app) James K Nelson @james_k_nelson
* [A Case for setState](https://medium.com/@zackargyle/a-case-for-setstate-1f1c47cd3f73#.w89epdtmo) Zack Argyle
* [¿Donde conservo los datos de un Componente React?: state, store, static, and this](https://medium.freecodecamp.com/where-do-i-belong-a-guide-to-saving-react-component-data-in-state-store-static-and-this-c49b335e2a00#.8k7tc37cs) Sam Corcos
* [Como manejar el Estado en React. The missing FAQ](https://medium.com/react-ecosystem/how-to-handle-state-in-react-6f2d3cd73a0c#.dwz84fx9s) Osmel Mora @osmel_mora
* [Should I keep something in React component state? I made a small cheatsheet.](https://twitter.com/dan_abramov/status/749710501916139520) Dan Abramov @dan_abramov
* [Best Practices for Component State in React.js](http://brewhouse.io/blog/2015/03/24/best-practices-for-component-state-in-reactjs.html) Gabe Scholz @gabescholz
* [Exploring React’s State Propagation](https://www.sitepoint.com/exploring-reacts-state-propagation) Eric Greene @ericwgreene

**¿Cómo puedo desacoplar el estado y la interfaz de usuario?**

* [Cómo puedo desacoplar el estado y la interfaz de usuario](https://medium.com/@mweststrate/how-to-decouple-state-and-ui-a-k-a-you-dont-need-componentwillmount-cc90b787aa37#.7l8ji1wer) Michel Weststrate @mweststrate

#Binding
>El método bind de JavaScript tiene varios usos. Normalmente, se utiliza para preservar el contexto de ejecución de una función que se ejecuta en otro contexto.

**What should you use for binding methods in React classes?**
**¿Qué debe usar para conectar métodos en Clases de React?**
* [To bind or not to bind?](https://twitter.com/dan_abramov/status/790612782471319553) Dan Abramov @dan_abramov
* [fat Arrow vS Autobind VS bind](https://www.reddit.com/r/reactjs/comments/54xnao/fat_arrow_vs_autobind_vs_bindbindbindbindbind/d85wj0l) Dan Abramov @dan_abramov

**¿Qué es eso del "Binding"?**

* [No uses bind cuando pases propiedades](https://daveceddia.com/avoid-bind-when-passing-props) Dave Ceddia
* [5 maneras de manejar el Binding](https://medium.com/@housecor/react-binding-patterns-5-approaches-for-handling-this-92c651b5af56#.4z71l0kmb) Cory House @housecor
* [¿Cómo lidiar con la referencia a `this` dentro de una promesa?](https://www.toptal.com/react/tips-and-practices) Toptal Developers

#Eventos

**¿Cómo funciona el sistema de eventos en React?**

* [Los eventos de React en profundidad](https://www.youtube.com/watch?v=dRo_egw7tBc) Kent C. Dodds, Ben Alpert, & Dan Abramov

#Renderizado

**¿Qué debe ir en la función de render?**

* [Return as soon as you know the answer](https://medium.com/@SimonRadionov/return-as-soon-as-you-know-the-answer-dec6369b9b67#.82kxymyki) @SimonRadionov

#Keys
>React uses [keys](https://facebook.github.io/react/docs/reconciliation.html#keys) to help with Reconciliation (i.e. how it calculates the DOM diff for each render).
>React utiliza las [keys](https://facebook.github.io/react/docs/reconciliation.html#keys) para ayudar con la reconciliación (es decir, cómo calcula la diferencia del DOM para cada procesamiento).

```
<ul>
  <li key="2015">Duke</li>
  <li key="2016">Villanova</li>
</ul>
```

**¿Por qué no puedo poner la key en las propiedades (o definir el valor predeterminado en otro lugar)?**

* [Why can't i put key in default props](https://www.reddit.com/r/reactjs/comments/4mjdcf/why_cant_i_put_key_in_default_props_or_define_the/d3xwa6m)

**¿Qué debo utilizar para una key?**

* [Index as a key is an anti-pattern](https://medium.com/@robinpokorny/index-as-a-key-is-an-anti-pattern-e0349aece318#.y4ru46ikc) Robin Pokorný @robinpokorny

**¿Cuáles son algunos ejemplos en los que debería cambiar manualmente una key?**

* [The key is using key](https://twitter.com/timarney/status/730785238654287873) Tim Arney @timarney

#Referencias
>El atributo ref permite guardar una referencia a un elemento React específico o a un componente devuelto por la función render(). Esto puede ser valioso cuando se necesita una referencia, desde dentro de un componente, a algún elemento o componente contenido en la función render(). - reactenlightenment.com

**¿Qué son las Referencias (refs) y porqué las Referencias de tipo Sring son malas?**

* [Refs to Components](https://facebook.github.io/react/docs/more-about-refs.html)
* [Why do you use findDOMNode()?](https://twitter.com/dan_abramov/status/752936646602031104) Dan Abramov @dan_abramov
* [String refs are bad in quite a few ways](https://news.ycombinator.com/edit?id=12093234) Dan Abramov @dan_abramov

#Contexto
⚠️ El contexto es una **característica avanzada y experimental**. Es probable que la API cambie en futuras versiones. Los rumores de su existencia son verdaderos pero ten cuidado!

* [How to handle React context in a reliable way](https://medium.com/react-ecosystem/how-to-handle-react-context-a7592dfdcbc#.rtwgxxy0d) Osmel Mora @osmel_mora
* [How to safely use React context](https://medium.com/@mweststrate/how-to-safely-use-react-context-b7e343eff076#.m6v9tsgub) Michel Weststrate @mweststrate
* [Context all the things with React](https://www.youtube.com/watch?v=k9AhBMwj1w4) Stephen Rivas Jr. (@sprjrx)

#Formularios

**¿Cómo puedo crear formularios con React?**

* [Learn Raw React: Ridiculously Simple Forms](http://jamesknelson.com/learn-raw-react-ridiculously-simple-forms) James K Nelson @james_k_nelson

**¿Cómo puedo validar la entrada de formularios?**
* [Elegant Form Validation Using React](https://spin.atomicobject.com/2016/10/05/form-validation-react) Jordan Schaenzle
* [Building validated forms with great UX in React](https://youtu.be/1Urj4TZ5BLI?t=2437) Marcela Hrdá
* [react-validation](https://github.com/vacuumlabs/react-validation)


#Controlled Components

**What is a controlled component?**

Via Loren Stewart @lorenstewart111 [React.js Forms: Controlled Components](http://lorenstewart.me/2016/10/31/react-js-forms-controlled-components)

>A controlled component has two aspects:

1. Controlled components have functions to govern the data going into them on every onChange event, rather than grabbing the data only once, e.g. when a user clicks a submit button. This 'governed' data is then saved to state (in this case, the parent/container component's state).

2. Data displayed by a controlled component is received through props passed down from it's parent/container component.

> This is a one-way loop – from (1) child component input (2) to parent component state and (3) back down to the child component via props – is what is meant by unidirectional data flow in React.js application architecture.

#Ajax en React

**¿Cuál es la mejor práctica para obtener datos de servidor en los componentes de React?**
>Depende! Ver: [React AJAX Best Practices](http://andrewhfarmer.com/react-ajax-best-practices) Andrew H Farmer @ahfarmer

* [Loading and Using External Data in React](http://mediatemple.net/blog/tips/loading-and-using-external-data-in-react) Chris Coyier @chriscoyier

#Patrones

* [React Patterns](http://reactpatterns.com) @chantastic
* [React.js in patterns](http://krasimirtsonev.com/blog/article/react-js-in-design-patterns) Krasimir Tsonev
* [Patterns For Style Composition In React](http://jxnblk.com/writing/posts/patterns-for-style-composition-in-react) Brent Jackson @jxnblk
* [Make Your React Components Pretty](https://medium.com/walmartlabs/make-your-react-components-pretty-a1ae4ec0f56e#.ctwfvx379) Mark Brouch @markbrouch

#Gotchas

**What are some React Gotchas?**

* [React Gotchas](https://daveceddia.com/react-gotchas) Dave Ceddia

#PATENTES

**¿Qué es todo eso que escucho sobre la cláusula de PATENTES de Facebook?**

* [Some links to point people to when they misinterpret PATENTS clause or spread false claims](https://gist.github.com/gaearon/df0c4025e67399af72786d7ac7c819cc) Dan Abramov @dan_abramov
* [React’s license: necessary and open?](http://lu.is/blog/2016/10/31/reacts-license-necessary-and-open) Luis Villa @luis_in_140

#Mixins

**¿Por qué los Mixins se consideran perjudiciales?**

* [Mixins Considered Harmful](https://facebook.github.io/react/blog/2016/07/13/mixins-considered-harmful.html) Dan Abramov @dan_abramov

#Internacionalización

**¿Cómo debo manejar la internacionalización?**

* [Internacionalización en React](https://medium.freecodecamp.com/internationalization-in-react-7264738274a0#.bcfxgycwv) Preethi Kasireddy

**¿Qué repositorios existen para la internacionalización?**
* [react-intl](https://github.com/yahoo/react-intl)
* [react-localize](https://github.com/sprjr/react-localize) @sprjrx

#Librerías de terceros

**¿Cómo utilizo Librerías de terceros?**

* [Integration with Third Party Libraries](https://www.youtube.com/watch?v=GWVjMHDKSfU&feature=youtu.be&a) Rally Coding

#Rendimiento

**¿Cómo puedo hacer que mi aplicación sea más rápida?**

* [Component Rendering Performance in React](https://medium.com/modus-create-front-end-development/component-rendering-performance-in-react-df859b474adc#.gvyat7vkb) Grgur Grisogono
* [Don‘t use PureComponent everywhere. Measure](https://twitter.com/dan_abramov/status/759383530120110080) Dan Abramov @dan_abramov
* [React.js pure render performance anti-pattern](https://medium.com/@esamatti/react-js-pure-render-performance-anti-pattern-fb88c101332f#.hewsz120q)
* [Should I use shouldComponentUpdate?](http://jamesknelson.com/should-i-use-shouldcomponentupdate) James K Nelson @james_k_nelson
* [Reconciliation](https://facebook.github.io/react/docs/reconciliation.html)
* [Quick slides on #reactjs performance](http://presentations.survivejs.com/react-performance/#/?_k=ivqhoe) Juho Vepsäläinen @bebraw

#Animationes

**¿Cómo animo cosas en React?**

* 🔥 💯 [Animating In React](https://youtu.be/Fk--XUEorvc?t=2344 Sarah Drasner) @sarah_edo
* [UI Animations with React — The Right Way](https://medium.com/@joethedave/achieving-ui-animations-with-react-the-right-way-562fa8a91935#.g8qmlz5d6) Joe Davis
* [Animations with ReactTransitionGroup](https://medium.com/@cheapsteak/animations-with-reacttransitiongroup-4972ad7da286#.qmrksnixv) Chang Wang @CheapSteak

**¿Hay alguna API declarativa para animaciones?**

* [React Motion](https://github.com/chenglou/react-motion)
* [A gentle introduction to React Motion](https://medium.com/@nashvail/a-gentle-introduction-to-react-motion-dc50dd9f2459#.aio7blbsi)

**¿Cómo puedo animar las transiciones de página?**

* [React Page Transition Animations](https://medium.com/front-end-hacking/react-page-transition-animations-9d18c90a9831#.lc9943ajq) Huan Ji

**¿Cuáles son algunos de los mejores repositorios sobre animación en React?**
* [react-animations](https://github.com/FormidableLabs/react-animations)
* [react-anime](https://github.com/stelatech/react-anime)
* [react-motion](https://github.com/chenglou/react-motion)
* [velocity-react](https://github.com/twitter-fabric/velocity-react)
* [state-transitions](https://github.com/jacobp100/state-transitions)
* [react-tween](https://github.com/clari/react-tween)

#SVG y React

**¿Cómo trabajo con SVG en React?**

* [Icons as React Components](https://medium.com/@david.gilbertson/icons-as-react-components-de3e33cb8792#.lmbz3v9ic)
* [Creating an SVG Icon System with React](https://css-tricks.com/creating-svg-icon-system-react) @sarah_edo

#Guias de estilo para React

**¿Dónde puedo encontrar buenas guías de estilo para React?**

* [Eventbrite React & JSX Coding Style Guide](https://github.com/eventbrite/javascript/tree/master/react)
* [Airbnb React/JSX Style Guide](https://github.com/airbnb/javascript/tree/master/react)


#Redux y Mobx

**¿Qué es (Redux/Mobx)?**

* [Confundido! ¿Redux o MobX?](https://www.reddit.com/r/reactjs/comments/4npzq5/confused_redux_or_mobx)

**¿Necesito usar (Redux/Mobx)?**

* [You don’t need Redux if your data never changes. The whole point of it is managing changes.](https://twitter.com/dan_abramov/status/737036433215610880) Dan Abramov @dan_abramov
* [You Might Not Need Redux](https://medium.com/@dan_abramov/you-might-not-need-redux-be46360cf367#.kgnqdp8p6) Dan Abramov @dan_abramov
* [Redux or MobX: An attempt to dissolve the Confusion](http://www.robinwieruch.de/redux-mobx-confusion/) Robin Wieruch @rwieruch

**¿Cómo escalar aplicaciones de React-Redux?**

* [About folder structure, styling, data fetching, etc.](https://www.smashingmagazine.com/2016/09/how-to-scale-react-applications/) Max Stoiber @mxstbr

#Añadir React a una Aplicacion existente

**¿Cómo empiezo a integrar React en una aplicación existente?**

* [How to Sprinkle ReactJS into an Existing Web Application](https://scotch.io/tutorials/how-to-sprinkle-reactjs-into-an-existing-web-application) Andrew Del Prete @andrewdelprete
* [Don't Rewrite, React!](https://www.youtube.com/watch?v=BF58ZJ1ZQxY) Ryan Florence
* [Migrating Safely to React](https://www.youtube.com/watch?v=sXDZBxbRRag&list=PLNBNS7NRGKMG3uLrm5fgY02hJ87Wzb4IU&index=1) Jamis Charles

#CSS y React

**¿Qué pasa con los estilos en React?**

* [Reusable React Component with Overridable Inline CSS Styles](http://staxmanade.com/2016/06/reusable-react-component-with-overridable-inline-css-styles/)
* [Inline Styles](https://facebook.github.io/react/tips/inline-styles.html)
* [PANEL ON 'INLINE STYLES'](http://shoptalkshow.com/episodes/180-panel-on-inline-styles) @ShopTalkShow
* [CSS in JS may not be the solution to all your problems](https://blog.grommet.io/post/2016/08/10/css-in-js-may-not-be-the-solution-to-all-your-problems) Alan Souza
* [CSS in JS + CSS Modules](http://www.dadsindev.com/12)
* [CSS in JS tech chat](https://www.youtube.com/watch?v=BXOF_8jDdf8) Kent C. Dodds & Sarah Drasner

**¿Hay alguna herramienta disponible para convertir 'CSS' a 'CSS en JS'?**

* [convert 'css' to 'CSS in JS'](https://jsbin.com/dugija/edit?js,output) Kent C. Dodds

#Testing

* [Testing React Applications](https://www.youtube.com/watch?v=eWN8F_WOBAQ) Jack Franklin
* [People seem to laugh at this but I think it’s actually pretty reasonable](https://twitter.com/dan_abramov/status/762257231471579136) Dan Abramov @dan_abramov

#Vídeos de Conferencias
* [React.js Conf 2016](https://www.youtube.com/watch?v=MGuKhcnrqGA&list=PLb0IAmt7-GS0M8Q95RIc2lOM6nc77q1IY)
* [ReactEurope](https://www.youtube.com/channel/UCorlLn2oZfgOJ-FUcF2eZ1A)
* [ReactRally](https://www.youtube.com/channel/UCXBhQ05nu3L1abBUGeQ0ahw)

#Contribuyendo a React JS

**¿Dónde puedo aprender sobre como contribuir a React JS?**

* [Contributing to React JS](https://www.youtube.com/watch?v=wUpPsEcGsg8) Kent C. Dodds

#Universal React

* [React on the Server for Beginners](https://scotch.io/tutorials/react-on-the-server-for-beginners-build-a-universal-react-and-node-app) Luciano Mammino @loige

#Deep Dive
* [Implementation Notes - How React Really Works](https://facebook.github.io/react/contributing/implementation-notes.html) Dan Abramov @dan_abramov
* [Building React From Scratch](https://www.youtube.com/watch?v=_MAD4Oly9yg) Paul O'Shannessy @zpao
* [React Architecture – OSCON](http://blog.vjeux.com/2014/javascript/react-architecture-oscon.html) Christopher Chedeau @vjeux
* [ReactJS: Under The Hood](https://www.youtube.com/watch?v=xsKYAa1ZXpQ) Boris Dinkevich @BorisDinkevich
* [REACT INTERNALS](https://zackargyle.github.io/react-internals-slides/#/?_k=7f19z9) Zack Argyle @ZackArgyle

#React Fiber

**¿Qué es React Fiber?**

* Experimental - [React Fiber Architecture](https://github.com/acdlite/react-fiber-architecture) Andrew Clark @acdlite
* Experimental - [What's Next for React](https://www.youtube.com/watch?v=aV1271hd9ew) Andrew Clark @acdlite

**¿Está listo React Fiber?**
* http://isfiberreadyyet.com

**¿Cómo puedo contribuir a Fiber?**
* [Fiber Principles: Contributing To Fiber](https://github.com/facebook/react/issues/7942)

#Cursos en Video

**¿Hay buenos recursos de video/cursos para aprender React?**

* https://egghead.io/courses/react-fundamentals FREE (+ paid for others)
* https://reactforbeginners.com
* https://app.pluralsight.com/courses/react-redux-react-router-es6
* https://www.pluralsight.com/courses/react-flux-building-applications
* https://frontendmasters.com/courses/react-intro (they have a bunch)
* http://courses.reactjsprogram.com/courses/reactjsprogrambundle
* https://LearnRedux.com
* https://egghead.io/courses/manage-complex-state-in-react-apps-with-mobx

#A11Y

**¿Qué pasa con la accesibilidad?**

* [How to design for accessibility](http://www.bbc.co.uk/gel/guidelines/how-to-design-for-accessibility ) *Note:* not specific to React but a solid primer on the topic

<hr>

**¿Cómo manejo A11y en React?**
* [Excerpt from React.js Conf 2015 - Hype!](https://www.youtube.com/watch?v=z5e7kWSHWTg#t=631) Ryan Florence
* [Bringing the Web Back to the Blind by Ryan Florence ](https://www.youtube.com/watch?v=YuzS-g6Qvq8) *Note:* not specific to React

#Charlas
* [React to the Future - Slide Deck](http://elijahmanor.com/talks/react-to-the-future/dist) Elijah Manor @elijahmanor
* [React Things - PDF Slides](https://react.rocks/blog/images/React_Intro_sept_2016.pdf) Jeff Winkler @winkler1

#Entrenamiento

**¿Dónde puedo obtener entrenamiento sobre React?**
<hr>

*Micheal Jackson* @mjackson & *Ryan Florence* @ryanflorence

* https://reactjs-training.com

<hr>
*Brian Holt* @holtbt

* https://btholt.github.io/es6-react-pres
* https://btholt.github.io/complete-intro-to-react
* https://github.com/btholt/react-redux-workshop

#Libros

**¿Dónde puedo encontrar buenos libros sobre React?**

* [React Enlightenment ](http://www.reactenlightenment.com) Cody Lindley @codylindley
* [Build your first real world React.js application](http://academy.plot.ly/#react) Max Stoiber @mxstbr
* [SurviveJS React](http://survivejs.com/react/introduction)
* [Fullstack React](https://www.fullstackreact.com)

#Listas de Correo

**¿Dónde puedo encontrar listas de correo sobre de React?**

* [React.js Newsletter](http://reactjsnewsletter.com)
* [React Status](http://react.statuscode.com)
* [Fullstack React](http://newsletter.fullstackreact.com)
* [This Week In React](https://thisweekinreact.com)
* [React Digest](http://reactdigest.net)

#Preguntas de entrevistas

* [12 Essential React.js Interview Questions](https://www.toptal.com/react/interview-questions)
* [React Interview Questions](https://github.com/eltonjuan/react-interview-questions/blob/master/ReactInterviewQuestions.md)
* [quiz.md](https://gist.github.com/gaearon/8fa9fdd2c4197ee0b52894877bf587a4) Dan Abramov @dan_abramov
* [5 Essential React.js Interview Questions](https://www.codementor.io/reactjs/tutorial/5-essential-reactjs-interview-questions)
* [The Vital Guide to React.js Interviewing](https://chandanpandey.com/2016/10/27/the-vital-guide-to-react-js-interviewing)
