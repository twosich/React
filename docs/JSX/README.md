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

## Elementos
Estos son unidades mas pequeñas en React.
Estos definen lo que se visualiza en la pantalla.

### Diferencias
Los componentes en React estan compuestos por Elementos, estos 
ultimos son estructuras de codigo minimas que permiten construir 
componentes mas complejos

# HTML
En JSX es importante saber que se pueden usar todas las etiquetas disponibles de HTML. a estos mismos se los cataloga de elementos, todos estos se representan con letras minusculas a diferencia de los componentes que por ley inician todos en letas mayusculas

### Componente
```jsx
const Example() {
    return (
        <h1>Hello World</h1>
    );
}
```
### Elemento
```jsx
const example = <h1>Hello World</h1>;
```

## Atributos
En JSX se pueden añadir atributos a las etiquetas, en lo que difiere es que en algunos casos no se declara de la forma acostumbrada, un ejemplo es el atributo class

### JSX
```jsx
const example = <h1 className="Simply" >Hello World</h1>;
```
### HTML
```html
<h1 class="Simply" >Hello World</h1>;
```