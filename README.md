<p align="center">
  <img src="assets/logo-2582747_640.png" /> 
</p>

# La arquitectura de módulos CSS - BEM Y SMACSS

**La arquitectura de módulos CSS** es un enfoque para organizar y diseñar los estilos de un sitio web de manera más eficiente y mantenible. En lugar de tener un gran archivo CSS con todos los estilos para todo el sitio, los módulos CSS dividen el contenido en componentes más pequeños y reutilizables, cada uno con su propio archivo de estilos. Esto permite que los estilos sean más fáciles de mantener y modificar, ya que cada componente tiene su propio conjunto de estilos y no está mezclado con el resto del sitio.

Algunas ventajas de utilizar la arquitectura de módulos CSS incluyen:

- Mayor reutilización: los componentes pueden utilizarse en varias páginas o sitios web diferentes sin tener que copiar y pegar código.
- Mayor facilidad de mantenimiento: si necesitas cambiar el aspecto de un componente, solo tienes que modificar el archivo de estilos correspondiente en lugar de buscar el código en un archivo CSS grande y desorganizado.
- Mayor facilidad de colaboración: los diferentes componentes pueden ser trabajados por diferentes desarrolladores sin pisarse entre sí.

Hay varias formas de implementar la arquitectura de módulos CSS, como BEM (Block-Element-Modifier), SMACSS (Scalable and Modular Architecture for CSS) y OOCSS (Object Oriented CSS). Cada uno de estos enfoques tiene sus propias convenciones y filosofías, así que es importante elegir el que mejor se adapte a tus necesidades y preferencias.

Espero que esta explicación te haya ayudado a entender mejor qué es la arquitectura de módulos CSS. Si tienes más preguntas o necesitas más ayuda, no dudes en preguntar.

---

## BEM (Block, Element, Modifier) [![Edit CSS-BEM](https://codesandbox.io/static/img/play-codesandbox.svg)](https://codesandbox.io/s/css-bem-dqeryt?fontsize=14&hidenavigation=1&theme=dark)

Es una metodología de diseño y desarrollo web que se enfoca en la organización y reutilización del código HTML y CSS. La idea detrás de BEM es crear bloques de código reutilizables y modulares que puedan ser utilizados en diferentes partes de una aplicación web.

Para utilizar BEM, se dividen los elementos de una página web en bloques, elementos y modificadores.

- Los bloques son componentes más grandes y más genéricos, como un encabezado o un menú de navegación.

- Los elementos son partes más pequeñas de un bloque, como un título o un enlace dentro de un menú de navegación.

- Los modificadores son clases que se añaden a un bloque o elemento para modificar su apariencia o comportamiento, como una clase que cambia el color de un título.

Para utilizar BEM en su código, se utilizan nombres de clase que combinan los nombres de bloque, elemento y modificador. Por ejemplo, si tenemos un bloque llamado "menu" con un elemento llamado "enlace" y un modificador llamado "activo", el nombre de clase podría ser "menu\_\_enlace--activo".

Al utilizar BEM, es importante tener en cuenta que cada bloque, elemento y modificador debe ser independiente y no depender de su contexto en la página. Esto hace que sea más fácil reutilizar y mantener el código a medida que se desarrolla una aplicación web.

### 1. Un bloque de menú de navegación:

<p align="center">
  <img src="/assets/bloque1.png" />
</p>

### 2. Un elemento de enlace dentro del menú:

<p align="center">
  <img src="/assets/bloque2.png" />
</p>

### 3. Un modificador que cambia el color de un enlace:

<p align="center">
  <img src="/assets/bloque3.png" />
</p>

### 4. Un bloque de tarjeta con un elemento de título y un modificador que cambia el color del título:

<p align="center">
  <img src="/assets/bloque4.png" />
</p>

---

## **SMACSS (Scalable and Modular Architecture for CSS)** [![Edit CSS-SMACSS](/assets/play-codesandbox.png)](https://codi.link/PGRpdiBjbGFzcz0iY29udGFpbmVyIj4NCiAgPGRpdiBjbGFzcz0iYm94IGJveC1wcmltYXJ5Ij4NCiAgICA8aDIgY2xhc3M9ImJveC10aXRsZSI+VMOtdHVsbyBkZSBsYSBjYWphPC9oMj4NCiAgICA8cCBjbGFzcz0iYm94LXRleHQiPlRleHRvIGRlIGxhIGNhamE8L3A+DQogIDwvZGl2Pg0KICA8ZGl2IGNsYXNzPSJib3ggYm94LXNlY29uZGFyeSI+DQogICAgPGgyIGNsYXNzPSJib3gtdGl0bGUiPlTDrXR1bG8gZGUgbGEgY2FqYTwvaDI+DQogICAgPHAgY2xhc3M9ImJveC10ZXh0Ij5UZXh0byBkZSBsYSBjYWphPC9wPg0KICA8L2Rpdj4NCjwvZGl2Pg==%7CLmNvbnRhaW5lciB7DQogIHdpZHRoOiA4MCU7DQogIG1hcmdpbjogMCBhdXRvOw0KfQ0KDQouYm94IHsNCiAgcGFkZGluZzogMjBweDsNCiAgbWFyZ2luLWJvdHRvbTogMjBweDsNCn0NCg0KLmJveC1wcmltYXJ5IHsNCiAgYmFja2dyb3VuZC1jb2xvcjogI2YwZjBmMDsNCn0NCg0KLmJveC1zZWNvbmRhcnkgew0KICBiYWNrZ3JvdW5kLWNvbG9yOiAjZTVlNWU1Ow0KfQ0KDQouYm94LXRpdGxlIHsNCiAgZm9udC1zaXplOiAyNHB4Ow0KICBmb250LXdlaWdodDogYm9sZDsNCiAgbWFyZ2luLWJvdHRvbTogMTBweDsNCn0NCg0KLmJveC10ZXh0IHsNCiAgZm9udC1zaXplOiAxOHB4Ow0KfQ==%7C)

Es una metodología de diseño y desarrollo web que se enfoca en la organización y escalabilidad de los estilos CSS. La idea detrás de SMACSS es crear una arquitectura sólida y modular para el código CSS que sea fácil de mantener y extender a medida que una aplicación web se vuelve más compleja.

SMACSS se divide en cinco categorías principales:

1. Reglas base: son estilos que se aplican a elementos HTML básicos, como párrafos, encabezados y enlaces.
2. Reglas de diseño: son estilos que dan forma a una página web, como tamaños de fuente y colores.
3. Reglas de layout: son estilos que controlan la disposición de los elementos en una página web, como el ancho y el margen de un contenedor.
4. Reglas de estado: son estilos que controlan el estado de un elemento, como hover o focus.
5. Reglas de tema: son estilos que se aplican a una aplicación web en su conjunto y pueden ser utilizados para cambiar el aspecto de una aplicación completa.

Para utilizar SMACSS en su código, se deben utilizar prefijos de clase que indican a qué categoría pertenece cada estilo. Por ejemplo, una clase de regla base podría tener el prefijo "base-", una clase de regla de diseño podría tener el prefijo "design-" y así sucesivamente.

SMACSS es una metodología útil para mantener el código CSS organizado y fácil de mantener a medida que una aplicación web se vuelve más compleja. Si tienes alguna pregunta adicional, no dudes en hacerla.

1. Una regla base para párrafos:

```
Copy code
.base-p {
  /* Estilos para párrafos */
}
```

1. Una regla de diseño para encabezados:

```
Copy code
.design-h1 {
  /* Estilos para encabezados h1 */
}

```

1. Una regla de layout para un contenedor:

```
Copy code
.layout-container {
  /* Estilos para el contenedor */
}

```

1. Una regla de estado para elementos con hover:

```
Copy code
.state-hover {
  /* Estilos para elementos con hover */
}

```

1. Una regla de tema para cambiar el aspecto de una aplicación:

```
Copy code
.theme-dark {
  /* Estilos para el tema oscuro */
}

```

---

## **OOCSS (Object Oriented CSS)**

Es una metodología de diseño y desarrollo web que se enfoca en la reutilización y separación de estilos CSS. La idea detrás de OOCSS es crear estilos reutilizables y modulares que puedan ser utilizados en diferentes partes de una aplicación web.

Para utilizar OOCSS, se deben seguir dos principios clave:

1. Separar el contenido de la presentación: esto significa que los estilos deben aplicarse a elementos HTML genéricos en lugar de elementos específicos. Por ejemplo, en lugar de aplicar estilos a un elemento "p" específico, se deben aplicar estilos a un elemento "bloque" que pueda ser utilizado en cualquier parte de la aplicación.
2. Reutilizar estilos: esto significa que los estilos deben ser lo más genéricos posible para que puedan ser utilizados en diferentes contextos. Por ejemplo, en lugar de crear un estilo para cada tipo de botón, se deben crear estilos para un botón genérico que pueda ser utilizado en diferentes partes de la aplicación.

Para utilizar OOCSS en su código, se deben crear clases genéricas que puedan ser reutilizadas en diferentes partes de la aplicación. Por ejemplo, en lugar de crear una clase específica para un botón en el encabezado, se puede crear una clase genérica para botones que pueda ser utilizada en cualquier parte de la aplicación.

OOCSS es una metodología útil para mantener el código CSS organizado y fácil de mantener a medida que una aplicación web se vuelve más compleja. Si tienes alguna pregunta adicional, no dudes en hacerla.

Claro, aquí hay algunos ejemplos de clases CSS utilizando la metodología OOCSS:

1. Una clase para un contenedor genérico:

```html
<div class="container">
  <div class="box box-primary">
    <h2 class="box-title">Título de la caja</h2>
    <p class="box-text">Texto de la caja</p>
  </div>
  <div class="box box-secondary">
    <h2 class="box-title">Título de la caja</h2>
    <p class="box-text">Texto de la caja</p>
  </div>
</div>
```

```css
.container {
  width: 80%;
  margin: 0 auto;
}

.box {
  padding: 20px;
  margin-bottom: 20px;
}

.box-primary {
  background-color: #f0f0f0;
}

.box-secondary {
  background-color: #e5e5e5;
}

.box-title {
  font-size: 24px;
  font-weight: bold;
  margin-bottom: 10px;
}

.box-text {
  font-size: 18px;
}
```
