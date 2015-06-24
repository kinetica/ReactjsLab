ReactjsLab
=============
#Ejemplos e información básica sobre Reactjs

<ul>
<li>Es un framework javascript</li> 
<li>Soportado por Facebook</li> 
<li>Maneja es solo la vista y eventos (comparable con la directivas de angujar)</li> 
<li>No define una arquitectura (Más libertad: se puede mezclar con otros fw)</li> 
<li>Utilizar un lenguaje especial (jsx) para la declaración de la parte visual de los componentes</li> 
<li>Se puede compilar a javascript (se suele hace en producción)</li> 
<li>Todo el código es javascript (no existen templates ni bindings)</li> 
<li>No soportar two way binding</li> 
</ul>

el tag script que contiene el jsx tiene que ser del tipo text/jsx

react.js + jsxtransformer.js

Componentes:
Un componente es una clase javascript que tiene un método render que retorna un nodo (es el único método obligatorio)
Cada componente es inmutable, si cambian los datos se destruye y se vuelve a crear
La idea es analizar la aplicación y detectar los elementos más pequeños que pueden cambiar

var APP = React.createClass({
	render: function(){
         return (<h1>Hola</h1>);
         }
});

React.renderComponent(<APP />, document.body);

Flux es una arquitectura propuesta por Facebook para organizar las aplicaciones

Rendimiento:
 Comparativa con Angularjs
 
 - http://plnkr.co/edit/6zfFXU?p=preview
 - http://plnkr.co/edit/YnF7Vn?p=preview

Ventajas:
Sólo modificaría el componente que cambie y no todo (mejor performance)
Permite pensar en componentes
Permite tener el control del binding
Permite utilizar mi propia arquitectura

Problemas:
Acoplamiento de html



