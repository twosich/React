# JSX

## Que es JSX?
JSX es una extension de React para la sintaxis de JavaScript.
este permite describir en JavaScript componentes con una 
estructura de HTML en etiquetas.

### Ventajas
Estructura sencilla de leer.
Advertencias mas utiles.

```jsx
const element = <h1>Hello World</h1>;
```
De manera literal podes combinar HTML con JavaScript

### Elementos
Estos son unidades mas pequeñas en React.
Estos definen lo que se visualiza en la pantalla.

#### Diferencias
Los componentes en React estan compuestos por Elementos, estos 
ultimos son estructuras de codigo minimas que permiten construir 
componentes mas complejos

## HTML
En JSX es importante saber que se pueden usar todas las etiquetas disponibles de HTML. a estos mismos se los cataloga de elementos, todos estos se representan con letras minusculas a diferencia de los componentes que por ley inician todos en letras mayusculas

#### Componente
```jsx
const Example() {
    return (
        <h1>Hello World</h1>
    );
}
```
#### Elemento
```jsx
const example = <h1>Hello World</h1>;
```

## Atributos
En JSX se pueden añadir atributos a las etiquetas, en lo que difiere es que en algunos casos no se declara de la forma acostumbrada, un ejemplo es el atributo class

#### JSX
```jsx
const example = <h1 className="Simply" >Hello World</h1>;
```
#### HTML
```html
<h1 class="Simply">Hello World</h1>;
```

Esto se debe a que en JavaScript la palabra class es una palabra reservada, esta a diferencia de HTML puro usa una palabra reservada escrita como className, su diferencia principal es que usa camelCase.

### Otros ejemplo:
```html
<h1 for="css">CSS</h1>;
```
```jsx
const example = <h1 htmlFor="css">Hello World</h1>;
```

## Style
El atributo style acepta un objecto de JavaScript con propiedades CSS escritas en camelCase, en su mayoria todo JSX de preferencia ocupa camelCase, esto es por una cuestion de sintaxis, asimilando la forma de un camello jorobado, en todas las propiedades o en su mayoria se utiliza esto, remplazando el background-image por ejemplo por backgroundImage.

#### JSX
```jsx
const styleDiv = {
    color: 'yellow',
    backgroundColor: 'black';
}
```

#### CSS
```css
div = {
    color: 'yellow',
    background-color: 'black';
}
```
### Uso
Para aplicar este atributo por ejemplo se utiliza de esta forma

```jsx
const styleDiv = {
    color: 'yellow',
    backgroundColor: 'black';
}

<div style={styleDiv}>Hello World</div>
```
Las llaves se deben a que en JSX los atributos funcionan como variables de JavaScript en algunos casos, y para aplicar estos atributos se aplican de esta forma(Esto se da solo en los casos donde se utilizan variables).

Alternativa en una sola linea. esta alternativa ocupa llaves dobles debido a que las primeras llaves insertan JavaScript y las segundas funcionan como un objecto de JavaScript sin necesidad de una variable.
#### JSX
```jsx
<div style={{color: 'yellow'}}>Hello World</div>
```
