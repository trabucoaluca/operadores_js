## Lenguaje de Programación Interpretado

Se creo para funcionar cliente / navegador
Isomorfismo

## Caracteristicas:

Lenguaje de alto nivel
Interpretado
Dinámico
Débilmente Tipado
Multiparadigma

No necesita los puntos y comas al final de cada linea


## Gramática:

Tipos de escritura o técnicas de  escritura:
1. camelCase o lowerCamelCase -> const unObjeto = {, let unaCadena = 'Hola Mundo', function estaFuncion() {, const ajax = new XMLHttpRequest(),
2. PascalCase UpperCamelCase -> class SerHumano {
3. Snake_case -> Archivos(mi_archivo_js.js)
4. UPPER_CASE -> const UNA_CONSTANTE = 'Soy una constante' 

Ordenamiento  de código:
Importación de Módulos
Declaración de Variables
Declaración de Funciones
Ejecución de Código


## Variables js

Son espacios donde se puede guardar información y asociarla a un determinado nombre. De esta forma, cada vez que se consulte ese nombre posteriormente, te devolverá la información que contiene.

Ojo: Las mayúsculas y minúsculas en los nombres de las variables de Javascript importan. No es lo mismo una variable llamada precio que una variable llamada Precio, pueden contener valores diferentes.


Tipos de Datos
Primitivos:
- string 
- number
- boolean
- null
- undefined

Compuestos:
- Funciones
- array
- objetos
- symbols
- RegExp


## typeof
ver el tipo de dato

## Strings

En programación, cuando hablamos de una variable que posee información de texto, decimos que su tipo de dato es string. En Javascript, es muy sencillo crear una variable de texto, hay dos formas de hacerlo:

- Literales
- Objeto

### Propiedades
.length

### Metodos
- .charAt(pos)
- .indexOf(str)
- .lastIndexOIf(str)
- .repeat(n)
- .toLowerCase()
- .toUpperCase()
- .replace()
- .trim()
- .split()


## Number

En Javascript, los números son uno de los tipos de datos básicos (tipos primitivos) que para crearlos, simplemente basta con escribirlos. No obstante, en Javascript todo son objetos, como veremos más adelante, y también se pueden declarar como si fueran un objeto

- Literales
- Objeto

### Propiedades
- NaN -> El acrónimo NaN es un valor especial de Javascript que significa Not A Number (No es un número). Este valor se usa para representar valores imposibles o indeterminados, como por ejemplo, resultados matemáticos de operaciones como.

0 / 0 (Indeterminaciones)

4 - 'a' (Valores imposibles)

NaN + 4 (Operaciones con NaN como operando)

### Metodos
comprobacion de numero:
console.log(Number.isFinite(num))
console.log(Number.isInteger(num))
console.log(Number.isNaN(num))

var num2 = Number.parseInt(num)
var num2 = Number.parseFloat(num)
var num = 1.5.toFixed(4)


## boolean

El tipo boolean tiene sólo dos valores posibles: true y false.

Este tipo se utiliza comúnmente para almacenar valores de sí/no: true significa “sí, correcto, verdadero”, y false significa “no, incorrecto, falso”.

## null

El valor especial null no pertenece a ninguno de los tipos descritos anteriormente, este forma un tipo propio separado que contiene sólo el valor null.

## undefined

El valor especial undefined también se distingue ya que hace un tipo propio, igual que null.

El significado de undefined es “valor no asignado”, por ejemplo  si una variable la declaramos, pero no asignamos ningun valor, entonces el valor que tomará esta será undefined.

## funciones

En Javascript, las funciones son bloques de código, autocontenido, que se puede definir una vez y ejecutar en cualquier momento. Opcionalmente una funcione puede aceptar parámetros y devolver un valor. 
Se dice que las funciones son ciudadanos de primera clase porque pueden asignarse a un valor, y puede pasarse como argumentos y usarse como un valor de retorno.

- declaracion
  * Funcion Declarada -> function nombreFuncion(){}
  * Funcion Expresada -> var nombreFuncion = function(){}

- Ejecución
  *  nombreFuncion()

- funciones autoejecutables
  * function(){
    console.log('hola')
    }()

## Arrays

Un es una colección o agrupación de elementos en una misma variable, cada uno de ellos ubicado por la posición que ocupa en el array.

## objetos

Los objetos se puede decir que son unas variables especiales las cuales pueden contener más variables en su interior. De esta forma, tenemos la posibilidad de organizar múltiples variables de la misma temática dentro de un objeto.

En JavaScript, los objetos penetran casi todos los aspectos del lenguaje. Por lo tanto, debemos comprenderlos primero antes de profundizar en cualquier otro lugar.


## Arrays

var arr = [25, true, null, "hola", {nombre: 'Jhoswe', apellido: 'Castro'}];
var arr2 = [1, 2, 3, 4, 5, 6, 7, 8, 9];

console.log(arr[4]);

//metodos
arr.push("adios", 654);
console.log(arr);

arr.unshift("inicio", true);
console.log(arr);

arr.pop();
console.log(arr);

arr.shift();
console.log(arr);

var arr3 = arr.concat(arr2)
console.log(arr3);


## objetos

### Objeto Console
- console.log -> Muestra la información proporcionada en la consola Javascript.
- console.info()
- console.warm()
- console.error()
- console.table()
- console.clear()

### Objeto Date

### Objeto Math

var a = Math.PI;
var a = Math.E;
var a = Math.abs(-5);
var a = Math.sign(0);
var a = Math.max(0, 50, 20, 70);
var a = Math.min(0, 50, 20, 70);
var a = Math.random() * 10;
var a = Math.random() * 10;

var b = 36;
var c = Math.round(b);
var c = Math.ceil(b);
var c = Math.floor(b);

var c = Math.pow(b, 5)
var c = Math.sqrt(b);

console.log(c);


## Contexto de Ejecución (Scope - Entorno)

Tengamos en cuenta que JS es sincrono es decir que la ejecucion del codigo va linea por linea

Lexical Enviroment
Donde

contexto de ejecucion
Que