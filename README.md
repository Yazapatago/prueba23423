
---

# 🚀 Fundamentos de JavaScript 🎯

Estás dando los primeros pasos y, como todo nuevo viaje, a veces necesitamos una pequeña pausa para asegurar que nuestras bases están firmes.

### ¿Cuál es el objetivo de este taller?
- Practicar con ejercicios interactivos.
- Ganar confianza para seguir avanzando con paso firme.

### ¿Cómo usar este taller?
- Este documento está compuesto por secciones de texto (como esta) y bloques de código.
- Para ejecutar un bloque de código, cópialo a la consola del navegador (presiona F12 → Console) o a un archivo `.js` en Node.js, y ejecútalo con `node archivo.js`.
- *¡Sin miedo de experimentar!* Puedes modificar el código de ejemplo y volver a ejecutarlo para ver qué sucede. Si algo se rompe, ¡no pasa nada! Así también se aprende. Usa `console.log` para ver resultados.

Recuerda: la programación es una habilidad que se construye con práctica y paciencia. ¡Este es tu espacio para practicar y preguntar!

¡Empecemos!

# Sección 1: Primeros Pasos con JavaScript 🚶‍♂️➡️🏃‍♀️

En esta sección, vamos a refrescar algunas ideas fundamentales que son la base de todo lo que haremos en JavaScript.

### Repaso de Teoría 🧠
- **¿Qué es un Algoritmo?**
  
  Piensa en un algoritmo como una receta de cocina 📜. Es una secuencia de pasos claros y ordenados que seguimos para resolver un problema o lograr un objetivo. Por ejemplo, los pasos para hacer un café, o los pasos para calcular el área de un triángulo.

- **JavaScript:** Un Lenguaje Amigable y Poderoso

  JavaScript es un lenguaje de programación conocido por ser relativamente fácil de leer y escribir, ¡casi como si estuvieras escribiendo en inglés! Es muy versátil y se usa para muchas cosas: desarrollo web interactivo, apps móviles, servidores (con Node.js), ¡y mucho más!

- **Intérprete de JavaScript:** Nuestro Traductor
  
  Cuando escribimos código en JavaScript, necesitamos un "traductor" que le explique a la computadora lo que queremos hacer. Ese es el motor de JS (como V8 en Chrome o Node.js). Lee nuestras instrucciones (nuestro código) y las ejecuta en el navegador o servidor.

- **Sintaxis Básica:** Las Reglas del Juego

  Como cualquier lenguaje, JavaScript tiene sus propias reglas gramaticales, a esto le llamamos sintaxis.

  - **Comentarios:** `// Esto es un comentario` o `/* Multilínea */`
    
    Los comentarios son notas que dejamos en nuestro código para nosotros mismos o para otros programadores. El intérprete de JavaScript los ignora por completo. Son súper útiles para:

    - Explicar qué hace una parte del código.

    - Dejar recordatorios.

    - Desactivar temporalmente una línea de código sin borrarla.

- **Bloques de Código**: ¡MUY IMPORTANTE!

  En JavaScript, usamos llaves `{}` para definir bloques de código (como funciones o condicionales). La indentación es por legibilidad (usa 2-4 espacios), pero no es obligatoria como en Python. Asegúrate de cerrar todas las llaves y usar `;` al final de declaraciones (aunque JS los infiere a veces).

## Declaraciones:
Una declaración es simplemente una instrucción que JavaScript puede ejecutar. Por ejemplo, asignar un valor a una variable (`let edad = 20;`) o imprimir algo (`console.log("Hola");`).

## Convenciones de Estilo (Airbnb/Standard JS):
Escribiendo Código Bonito y Legible
Usa `let` para variables mutables, `const` para inmutables. Nombra en camelCase (ej: `nombreAprendiz`). Organiza el código con saltos de línea. Seguir estas convenciones hace que nuestro código sea más fácil de leer y entender por otros (¡y por ti en el futuro!).

## El Zen de JavaScript: La Filosofía
JavaScript no tiene un "Zen" oficial como Python, pero principios como "Simple es mejor que complejo" aplican. Usa `console.log("import this")` para un chiste, pero enfócate en código limpio.

### Ejemplos Prácticos 💻

```javascript
// Esto es un comentario. Sirve para explicar lo que hace el código.
// A continuación, vamos a imprimir un saludo.
console.log("¡Hola, aprendiz SENA!");

// Ejemplo de una declaración (asignación de variable)
const nombreDelCurso = "Fundamentos de Programación en JavaScript";
console.log(nombreDelCurso);

// Para ver algo "zen" (ejecuta en consola)
console.log("JavaScript: 'Write less, do more' – pero con debugging.");
```

## ¡A Tu Teclado! ⌨️
Ejercicio 1.1:
Escribe un comentario que explique qué hará la siguiente línea de código. Luego, ejecuta el bloque.

```javascript
// Tu comentario aquí: realizara la suma de 5 + 3
console.log(5 + 3);
```

### Ejercicio 1.2:
El siguiente código tiene un error de sintaxis (falta `;` o llave). Corrígelo para que funcione y ejecútalo.

```javascript
// Corrige el código si es necesario
console.log("JavaScript es poderoso.");
console.log("Y las llaves {} son clave.");
```

### Ejercicio 1.3:
Crea una variable llamada `miProgramaSena` y asígnale como valor el nombre de la tecnología que estás cursando (como texto). Luego, imprime el valor de esa variable.

```javascript
// Escribe tu código aquí
const miProgramaSena = "Análisis y Desarrollo de Software";
console.log(miProgramaSena);
```

# Sección 2: Los Tipos de Datos: Los Ladrillos de Construcción 🧱
Todo lo que manejamos en JavaScript tiene un "tipo". Conocer los tipos de datos es fundamental.

## Para recordar 🧠
### Números:
  - Enteros (`Number`): Números completos, sin decimales. Se usan para contar cosas, como el número de aprendices en una clase (ej: `25`), tu edad (ej: `19`).
  - Flotantes (`Number`): Números que tienen una parte decimal. Se usan para medidas que pueden no ser exactas, como la estatura (ej: `1.75`), el precio de un producto (ej: `3500.50`).

### Texto (`string`):
Cualquier secuencia de caracteres (letras, números, símbolos) encerrada entre comillas simples (`'Hola'`) o dobles (`"Hola"`). Se usa para nombres, mensajes, direcciones, etc. (ej: `"Análisis y Desarrollo de Software"`, `'Juan Pérez'`).

### Booleanos (`boolean`):
Representan valores de verdad: o algo es `true` (Verdadero) o es `false` (Falso). Son como interruptores de luz: encendido o apagado. (ej: `let estaLloviendo = true;`).

### La Función `typeof()`: Nuestra Lupa 🔍
Si alguna vez tienes dudas sobre qué tipo de dato es algo, JavaScript te ofrece `typeof()`. Simplemente le pasas el dato o la variable y te dirá su tipo.
Ejemplo: `typeof(10)` te dirá `'number'`.

### Mención Especial (sin profundizar aún):
Existen otros tipos de datos muy útiles para agrupar varios elementos, como arrays (`[]`), objetos (`{}`), Sets y Maps. Los mencionamos para que sepas que existen, ¡pero los exploraremos en detalle más adelante! Por ahora, nos concentraremos en los básicos.

## Ejemplos Prácticos 💻

```javascript
// Ejemplos de tipos de datos y uso de typeof()
const numeroEntero = 100;
console.log(numeroEntero);
console.log(typeof numeroEntero); // 'number'

const numeroFlotante = 25.78;
console.log(numeroFlotante);
console.log(typeof numeroFlotante); // 'number'

const saludo = "Bienvenido al SENA";
console.log(saludo);
console.log(typeof saludo); // 'string'

const esMayorDeEdad = true;
console.log(esMayorDeEdad);
console.log(typeof esMayorDeEdad); // 'boolean'

// También podemos usar typeof directamente con un valor
console.log(typeof 5); // 'number'
console.log(typeof "Python"); // 'string' (¡aunque sea "Python", es string!)
console.log(typeof false); // 'boolean'
console.log(typeof 9.0); // 'number'
```

## ¡Al Teclado! ⌨️
### Ejercicio 2.1:
Crea las siguientes variables con los valores indicados:

`miEdad` con tu edad (un número entero).

`alturaMetros` con tu altura en metros (un número flotante, ej: `1.65`).

`primerNombre` con tu primer nombre (texto).

`sabeProgramarAntes` con `false` si no tenías nociones previas de programación, o `true` si sí tenías (booleano).

Luego, para cada variable, imprime su valor y también su tipo usando `typeof()`.

```javascript
// Escribe tu código aquí
const miEdad = 25;
const alturaMetros = 1.75;
const primerNombre = 'Yeison';
const sabeProgramarAntes = true;

console.log(miEdad, typeof miEdad);
console.log(alturaMetros, typeof alturaMetros);
console.log(primerNombre, typeof primerNombre);
console.log(sabeProgramarAntes, typeof sabeProgramarAntes);
```

# ¡Desafíate! 🤯
### Reto 2.1:
JavaScript puede realizar operaciones matemáticas.

- ¿Qué tipo de dato (`number`) crees que resultará de sumar un entero con otro entero? (ej: `5 + 2`)
- ¿Qué tipo de dato crees que resultará de sumar un entero con un flotante? (ej: `5 + 2.0`)
- ¿Y si divides dos enteros, pero el resultado podría tener decimales? (ej: `7 / 2`)

Comprueba tus hipótesis usando `typeof()` sobre el resultado de estas operaciones.

```javascript
// Comprueba la suma de dos enteros
const resultado1 = 5 + 2;
console.log(`5 + 2 = ${resultado1}, Tipo: ${typeof resultado1}`);

// Comprueba la suma de un entero y un flotante
const resultado2 = 4.3 + 7;
console.log(`4.3 + 7 = ${resultado2}, Tipo: ${typeof resultado2}`);

// Comprueba la división de dos enteros
const resultado3 = 7 / 2;
console.log(`7 / 2 = ${resultado3}, Tipo: ${typeof resultado3}`);
```

# Sección 3: Hablando con JavaScript y Transformando Datos 🗣️🔄
Ahora veremos cómo podemos interactuar con nuestros programas pidiéndole datos al usuario y cómo JavaScript nos permite cambiar datos de un tipo a otro.

## Recordatorio Teórico 🧠
- La Función `console.log()`: Mostrando Información

  Ya la hemos usado bastante. `console.log()` nos permite mostrar mensajes, los valores de las variables, o los resultados de operaciones en la consola (la salida estándar).

- La Función `prompt()`: Pidiendo Datos al Usuario

  Cuando queremos que nuestro programa sea interactivo y reciba información del usuario, usamos `prompt()`.
  `prompt()` muestra un mensaje al usuario y espera a que el usuario escriba algo y presione Enter.
  ¡MUY IMPORTANTE! La función `prompt()` siempre devuelve lo que el usuario escribió como un dato de tipo texto (`string`), incluso si el usuario escribe números.

- Funciones de Conversión: Cambiando de Tipo

  Como `prompt()` siempre nos da texto, si necesitamos ese dato como un número para hacer cálculos, debemos convertirlo. JavaScript nos ofrece funciones para esto:
  - `parseInt(valorAConvertir)`: Intenta convertir `valorAConvertir` a un número entero. Si no puede (por ejemplo, si intentas convertir "hola" a int), dará `NaN`.
  - `parseFloat(valorAConvertir)`: Intenta convertir `valorAConvertir` a un número flotante.
  - `String(valorAConvertir)`: Convierte `valorAConvertir` a texto (útil si tienes un número y quieres tratarlo como texto).

- La Función `typeof()`: Ya la conocemos, pero úsala para verificar conversiones.

### Ejemplos Prácticos 💻

```javascript
// Usando console.log()
console.log("Calculadora simple de suma");

// Usando prompt() para pedir el nombre
const nombreUsuario = prompt("Por favor, dime tu nombre: ");
console.log("Hola, " + nombreUsuario + "!"); // Concatenación simple de strings

// Pidiendo números y convirtiéndolos
console.log("--- Sumadora ---");
const numero1Texto = prompt("Ingresa el primer número: ");
const numero2Texto = prompt("Ingresa el segundo número: ");

// Convertimos los textos a números enteros para poder sumarlos
const numero1Entero = parseInt(numero1Texto);
const numero2Entero = parseInt(numero2Texto);

const suma = numero1Entero + numero2Entero;
console.log("La suma de los números es:", suma);

// Ejemplo con flotantes para un precio
const precioProductoTexto = prompt("Ingresa el precio del producto (ej: 1500.50): ");
const precioProductoFlotante = parseFloat(precioProductoTexto);
console.log("El precio ingresado es:", precioProductoFlotante);
console.log(typeof precioProductoFlotante);
```

## ¡A Tu Teclado! ⌨️
### Ejercicio 3.1:
Escribe un programa que le pida al usuario su ciudad de nacimiento y luego imprima un mensaje como: "¡Qué bueno que naciste en [CIUDAD]!".

```javascript
// Escribe tu código aquí
console.log('Bienvenido');
const ciudad = prompt('Ingrese su ciudad de nacimiento: ');
console.log(`¡Qué bueno que naciste en ${ciudad}!`);
```

### Ejercicio 3.2:
Escribe un programa que le pida al usuario dos números NUMERO1 y NUMERO2 y luego imprima un mensaje como:

"La multiplicación de [NUMERO1] por [NUMERO2] es igual a [RESULTADO]."

```javascript
// Escribe tu código aquí
const numero1 = parseInt(prompt('Ingrese el 1er numero: '));
const numero2 = parseInt(prompt('Ingrese el 2do numero: '));

const multiplicacion = numero1 * numero2;

console.log(`La multiplicación de ${numero1} por ${numero2} es igual a ${multiplicacion}.`);
```

### Ejercicio 3.3:
Pide al usuario su peso en kilogramos (que podría ser un valor con decimales, ej: 65.5). Convierte este valor a float y luego imprímelo.

```javascript
// Escribe tu código aquí
const peso = parseFloat(prompt("Ingrese su peso en Kg: "));
console.log(`Su peso es: ${peso} Kg`);
```

## ¡Desafíate! 🤯
### Reto 3.1: Calculadora de Edad Aproximada
Pide al usuario su año de nacimiento. Luego, calcula su edad aproximada restando el año de nacimiento del año actual (puedes usar 2025 como año actual fijo por ahora). Imprime un mensaje que diga: "Tienes aproximadamente [EDAD] años."

**Pista:** Necesitarás convertir el año de nacimiento a int con `parseInt()`.

```javascript
// Escribe tu código aquí
const anoActual = 2025; // Puedes cambiarlo al año que desees usar

const fechaNacimiento = parseInt(prompt("Ingrese su ano de nacimiento:"));
const resta = anoActual - fechaNacimiento;

console.log(`Tienes aproximadamente ${resta} años.`);
```

# Sección 4: ¡Dando Formato Elegante a Nuestros Mensajes! (Template Literals) ✨📄
Hemos visto cómo `console.log()` puede mostrar varias cosas separadas por comas, o cómo podemos "sumar" (concatenar) textos. ¡Pero hay una forma mucho más moderna, legible y poderosa de construir mensajes que incluyen variables!

Explicación (¡Nuevo!) 🤓

  A veces queremos crear mensajes que mezclan texto fijo con los valores de nuestras variables. Por ejemplo, si tienes `nombre = "Carlos"` y `edad = 22`, y quieres imprimir "Hola, Carlos. Tienes 22 años.".

Una forma sería:
`console.log("Hola, " + nombre + ". Tienes " + edad + " años.");`
Esto funciona, pero nota que tuvimos que:
1. Usar `+` para separar los pedazos de texto.
2. Convertir la variable `edad` (que es `number`) a string implícitamente. Esto es fácil de olvidar y causa errores.

¡Aquí entran las **template literals**! 🌟

Las template literals son una manera mucho más limpia y directa de incrustar expresiones (como variables) dentro de una cadena de texto.

Sintaxis:
1. Empiezas la cadena de texto con una **backtick** (`` ` ``) en lugar de comillas.
2. Dentro de la cadena, donde quieras insertar el valor de una variable o el resultado de una expresión, lo pones entre `${ }`.

### Ejemplo:

```javascript
const nombre = "Ana";
const edad = 25;
const ciudad = "Medellín";

// Usando template literal
const mensaje = `Hola, me llamo ${nombre}, tengo ${edad} años y vivo en ${ciudad}.`;
console.log(mensaje);
// Salida: Hola, me llamo Ana, tengo 25 años y vivo en Medellín.
```

Ventajas de las template literals:
- Más legibles: Es más fácil ver cómo quedará el mensaje final.
- Menos propenso a errores: No necesitas convertir manualmente a string los números o booleanos; JS lo hace por ti.
- Más potente: Dentro de las `${ }` puedes poner no solo variables, ¡sino también expresiones y llamadas a funciones!

```javascript
// Ejemplo con expresiones dentro de la template literal
const nota1 = 4.5;
const nota2 = 3.5;
const promedio = (nota1 + nota2) / 2;
console.log(`La primera nota es ${nota1}, la segunda es ${nota2}. El promedio es ${promedio}.`);
console.log(`El doble del promedio es ${promedio * 2}.`);
console.log(`La suma de las notas es ${nota1 + nota2}.`);
```

### Ejemplos Prácticos 💻

```javascript
const articulo = "Portátil Gamer";
const precioUnitario = 200.00; // Un number
const cantidad = 210; // Un number

// Calculamos el total
const totalCompra = precioUnitario * cantidad;

// Usamos template literals para mostrar la información
console.log("--- Detalle de Compra ---");
console.log(`Producto: ${articulo}`);
console.log(`Precio por unidad: $${precioUnitario}`);
console.log(`Cantidad solicitada: ${cantidad} unidades`);
console.log(`Costo total: $${totalCompra}`);
console.log(`¿La compra supera los $5,000,000? ${totalCompra > 5000000}`); // Expresiones booleanas también
```

## ¡A Tu Teclado! ⌨️
### Ejercicio 4.1:
Retoma el Ejercicio 3.2 donde se pide al usuario dos números y calcular su multiplicación. Ahora, muestra el resultado usando una template literal con el siguiente formato:
    
"La multiplicación de [NUMERO1] por [NUMERO2] es igual a [RESULTADO]."

```javascript
// Pide los dos números al usuario (recuerda convertirlos a int)
const numero1 = parseInt(prompt("Ingresa el primer número para multiplicar: "));
const numero2 = parseInt(prompt("Ingresa el segundo número para multiplicar: "));

// Calcula la multiplicación
const multiplicacion = numero1 * numero2;

// Muestra el resultado usando una template literal
console.log(`La multiplicación de ${numero1} por ${numero2} es igual a ${multiplicacion}.`);
```

Ejercicio 4.2:
Pide al usuario su nombre completo y el nombre de su programa de formación en el SENA. Luego, muestra un mensaje de bienvenida personalizado usando una template literal, algo como:
```
"¡Bienvenido/a, [NOMBRE_COMPLETO], al excelente programa de [PROGRAMA_FORMACION] en el SENA!"
```

```javascript
// Escribe tu código aquí
const nombre = prompt("Ingrese su nombre completo: ");
const nombreFormacion = prompt("Ingrese el nombre de su programa de formacion: ");

console.log(`¡Bienvenido/a, ${nombre}, al excelente programa de ${nombreFormacion} en el SENA!`);
```

## ¡Desafíate! 🤯
## Reto 4.1: Mini Boleta de Venta
Crea un pequeño programa que haga lo siguiente:

1. Pida al usuario el nombre de un producto (texto).
2. Pida el precio unitario de ese producto (flotante).
3. Pida la cantidad que desea comprar de ese producto (entero).
4. Calcule el costo total (precio unitario * cantidad).
5. Muestre un resumen de la compra utilizando template literals, con un formato claro, por ejemplo:

```
--- Resumen de su Pedido ---
Producto: Teclado Mecánico
Precio Unitario: $150000.0
Cantidad: 2
________________________
Total a Pagar: $300000.0
¡Gracias por su compra!
```
(Los valores son ejemplos, tu programa usará los que ingrese el usuario).

```javascript
// Escribe tu código aquí
const nombreProducto = prompt("Ingrese el nombre del producto: ");
const precioProducto = parseFloat(prompt("Ingrese el valor UNITARIO del produto: "));
const cantidadProducto = parseInt(prompt("Ingrese la cantidad que quiere comprar del producto: "));

const costoTotal = precioProducto * cantidadProducto;

console.log("--- Resumen de su Pedido ---");
console.log(`Producto: ${nombreProducto}`);
console.log(`Precio Unitario: $${precioProducto}`);
console.log(`Cantidad: ${cantidadProducto}`);
console.log("________________________");
console.log(`Total a Pagar: $${costoTotal}`);
console.log("¡Gracias por su compra!");
```

# Sección 5: Mini-Proyecto: Calculadora Básica de Promedios 📊➕➖✖️➗

¡Es hora de integrar varias de las cosas que hemos repasado! En este mini-proyecto, construirás un programa que calcule el promedio de tres calificaciones.

### Descripción del Proyecto 📝
El programa deberá:

1. Saludar al usuario de forma amigable.
2. Solicitar al usuario que ingrese tres calificaciones (estas pueden ser números con decimales, así que piensa qué tipo de dato usar y cómo convertir la entrada).
3. Calcular el promedio de estas tres calificaciones.
4. Mostrar el promedio calculado al usuario, usando una template literal para que el mensaje sea claro y completo.

### Pasos Sugeridos (¡Una guía para ayudarte!) 🗺️
1. Saludo Inicial:
   - Usa `console.log()` para darle la bienvenida al usuario al programa de cálculo de promedios.
2. Pedir Calificación 1:
   - Usa `prompt()` para pedir la primera calificación.
   - Convierte la entrada del usuario a tipo number con `parseFloat()` y guárdala en una variable (ej: `nota1`).
3. Pedir Calificación 2:
   - Similar al paso anterior, pide la segunda calificación y guárdala como number (ej: `nota2`).
4. Pedir Calificación 3:
   - Pide la tercera calificación y guárdala como number (ej: `nota3`).
5. Calcular la Suma:
   - Suma las tres calificaciones (`nota1 + nota2 + nota3`) y guarda el resultado en una variable (ej: `sumaNotas`).
6. Calcular el Promedio:
   - Divide `sumaNotas` entre 3 (el número de calificaciones). Guarda este resultado en una variable (ej: `promedioFinal`).
7. Mostrar el Resultado:
   - Usa `console.log()` y una template literal para mostrar el promedio de forma clara. Por ejemplo: "Estimado/a [NOMBRE_SI_LO_PEDISTE_ANTES], el promedio de tus calificaciones [N1], [N2] y [N3] es: [PROMEDIO_FINAL]." (Puedes simplificar el mensaje si no pediste el nombre).

## ¡Manos a la Obra! 👨‍💻👩

```javascript
// Paso 1: Saludo Inicial
console.log("--- Calculadora de Promedio de 3 Notas ---\n");
const nombreUsuario = prompt("Ingrese su nombre: ");
console.log(`${nombreUsuario}, por favor ingrese las notas en orden\n`);

// Paso 2, 3, 4: Pedir Calificaciones (recuerda convertir a float)
const nota1 = parseFloat(prompt("Ingrese la nota 1: "));
const nota2 = parseFloat(prompt("Ingrese la nota 2: "));
const nota3 = parseFloat(prompt("Ingrese la nota 3: "));

console.log(`Tus notas son:\nNota 1: ${nota1}\nNota 2: ${nota2}\nNota 3: ${nota3}\n`);

// Paso 5: Calcular la Suma
const sumaNotas = nota1 + nota2 + nota3;

// Paso 6: Calcular el Promedio
const promedioFinal = sumaNotas / 3;

// Paso 7: Mostrar el Resultado (usa una template literal)
console.log(`${nombreUsuario}, el promedio de tus notas es: ${promedioFinal.toFixed(2)}`);
```

# Sección 6: ¡Siguientes Pasos y Ánimo! 💪🌟
¡Felicitaciones por haber llegado hasta aquí y completado este taller de refuerzo! 🥳

### Resumen del Viaje 🗺️
En este recorrido interactivo, hemos:
- Recordado los conceptos básicos como algoritmos, el intérprete de JavaScript y la importancia de la sintaxis (!hola, llaves `{}`!).
- Repasado los tipos de datos fundamentales: numbers, strings y booleanos.
- Practicado cómo interactuar con el usuario usando `prompt()` y cómo mostrar información con `console.log()`.
- Aprendido (o reforzado) la crucial habilidad de convertir tipos de datos (ej: de string a number con `parseFloat`).
- Descubierto el poder y la elegancia de las template literals para crear mensajes dinámicos y legibles.
- Aplicado todo esto en un mini-proyecto para calcular promedios.

### ¿Qué Sigue en Nuestro Camino? 🚀
Esta base que has reforzado es ESENCIAL para lo que viene. Próximamente en el curso, empezarás a explorar cómo:
- Hacer que tus programas tomen decisiones (usando estructuras como `if, else`).
- Lograr que tus programas repitan tareas de forma eficiente (con bucles como `for` y `while`).
- Organizar tu código de manera más estructurada con funciones.
- Y, por supuesto, ¡profundizar en esos tipos de datos para colecciones que mencionamos (arrays, objetos, etc.)!

### Un Mensaje ✨
Aprender a programar es como aprender un nuevo idioma o a tocar un instrumento musical: la práctica constante es la clave del éxito. No te desanimes si algo no sale a la primera. Los errores son parte del proceso de aprendizaje (¡incluso los programadores más experimentados los cometen!).

- Experimenta: Cambia el código de los ejemplos, prueba cosas nuevas.
- Pregunta: Si tienes dudas, ¡pregunta a tu instructor y a tus compañeros!
- Colabora: Ayudar a otros también te ayuda a ti a entender mejor.

# Sección 7: Operadores y Expresiones - Las Herramientas del Cálculo 🛠️🔢
Hasta ahora, hemos trabajado con datos y hemos visto cómo mostrarlos. Pero la verdadera magia de la programación comienza cuando podemos operar con esos datos. Para eso, usamos operadores, y cuando combinamos operadores con datos (variables o valores literales), formamos expresiones.

Piensa en los operadores como las acciones que puedes realizar (sumar, comparar, etc.) y en los datos como los objetos sobre los que actúas. Una expresión es como una frase completa que JavaScript evalúa para obtener un resultado.

## 7.1 Operadores Aritméticos: ¡Matemáticas en JavaScript! ➕➖✖️➗
Son los que ya conoces de las matemáticas. Permiten realizar cálculos numéricos.

| Operador | Nombre              | Ejemplo | Resultado (si a=10, b=3) |
|----------|---------------------|---------|--------------------------|
| `+`      | Suma                | a + b   | 13                       |
| `-`      | Resta               | a - b   | 7                        |
| `*`      | Multiplicación      | a * b   | 30                       |
| `/`      | División (real)     | a / b   | 3.333...                 |
| `**`     | División Entera (cociente) | Math.floor(a / b) | 3 |
| `%`      | Módulo (residuo)    | a % b   | 1                        |
| `**`     | Potencia (exponenciación) | a ** b | 1000 (esto es a^b = 10^3) |

**Nota:** En JS, la división entera usa `Math.floor(a / b)` o `(a / b) | 0`. No hay `//` como en Python.

**Ejemplos Prácticos:**

```javascript
// Operadores Aritméticos
const num1 = 15;
const num2 = 4;

const suma = num1 + num2;
const resta = num1 - num2;
const multiplicacion = num1 * num2;
const divisionReal = num1 / num2;
const divisionEntera = Math.floor(num1 / num2);
const residuo = num1 % num2;
const potencia = num1 ** 2; // 15 elevado al cuadrado

console.log(`La suma de ${num1} + ${num2} = ${suma}`);
console.log(`La resta de ${num1} - ${num2} = ${resta}`);
console.log(`La multiplicación de ${num1} * ${num2} = ${multiplicacion}`);
console.log(`La división de ${num1} / ${num2} = ${divisionReal} (Tipo: ${typeof divisionReal})`); // Nota: la división real siempre da number
console.log(`La división entera de ${num1} / ${num2} = ${divisionEntera} (Cociente de la división entera)`);
console.log(`El residuo es ${num1} % ${num2} = ${residuo} (Residuo de la división entera)`);
console.log(`${num1} elevado al cuadrado = ${potencia}`);

// Aplicación: convertir segundos a minutos y segundos
const totalSegundos = 135;
const minutos = Math.floor(totalSegundos / 60);
const segundosRestantes = totalSegundos % 60;
console.log(`${totalSegundos} segundos son ${minutos} minutos y ${segundosRestantes} segundos.`);
```

## ¡A Tu Teclado! ⌨️

### Ejercicio 7.1.1:
Pide al usuario dos números enteros. Calcula y muestra:

- La suma.
- La resta del primero menos el segundo.
- El producto.
- La división entera del primero sobre el segundo.
- El residuo de la división entera del primero sobre el segundo.

```javascript
// Escribe tu código aquí                                        
console.log("--- Calculadora Aritmética Básica ---");
const numero1 = parseInt(prompt("Ingrese el 1er numero: "));
const numero2 = parseInt(prompt("Ingrese el 2do numero: "));

const suma = numero1 + numero2;
const resta = numero1 - numero2;
const producto = numero1 * numero2;
const division = Math.floor(numero1 / numero2);
const residuo = numero1 % numero2;

console.log(`El resultado de las operaciones del numero ${numero1} y el numero ${numero2} son: \n`);
console.log(`Suma = ${suma}\nResta: ${resta}\nProducto: ${producto}\nDivision: ${division}\nResiduo: ${residuo}`);
```

### Ejercicio 7.1.2:
Un artículo cuesta $2500. Calcula cuánto costarían 3 artículos y cuánto si se compran 5. Muestra ambos resultados.

```javascript
// Escribe tu código aquí
const precioArticulo = 2500;
console.log(`El precio por 3 productos es de = $${precioArticulo * 3}`);
console.log(`El precio por 5 productos es de = $${precioArticulo * 5}`);
```

## 7.2 Operadores de Comparación: ¿Iguales, Mayores o Menores? 🤔⚖️
Estos operadores comparan dos valores y el resultado de la comparación es siempre un valor booleano: `true` o `false`.

| Operador | Nombre                  | Ejemplo | Resultado (si x=5, y=10) |
|----------|-------------------------|---------|--------------------------|
| `===`    | Igual a (estricto)      | x === y | false                    |
| `!==`    | Diferente de (No igual) | x !== y | true                     |
| `>`      | Mayor que               | x > y   | false                    |
| `<`      | Menor que               | x < y   | true                     |
| `>=`     | Mayor o igual que       | x >= 5  | true                     |
| `<=`     | Menor o igual que       | y <= 10 | true                     |

**Nota:** Usa `===` para comparación estricta (tipo + valor), no `==` (conversión implícita).

### Ejemplos Prácticos:

```javascript
// Operadores de Comparación
const valor1 = 100;
const valor2 = 50;
const valor3 = 100;

console.log(`¿${valor1} es igual a ${valor2}? ${valor1 === valor2}`);   // false
console.log(`¿${valor1} es igual a ${valor3}? ${valor1 === valor3}`);   // true
console.log(`¿${valor1} es diferente de ${valor2}? ${valor1 !== valor2}`); // true
console.log(`¿${valor1} es mayor que ${valor2}? ${valor1 > valor2}`);     // true
console.log(`¿${valor2} es menor que ${valor1}? ${valor2 < valor1}`);     // true
console.log(`¿${valor1} es mayor o igual que ${valor3}? ${valor1 >= valor3}`); // true
console.log(`¿${valor2} es menor o igual que 30? ${valor2 <= 30}`);     // false

// Comparando la entrada del usuario
const edadUsuarioTexto = prompt("Ingresa tu edad: ");
const edadUsuarioNumero = parseInt(edadUsuarioTexto);

const esMayorDeEdad = edadUsuarioNumero >= 18;
console.log(`¿Eres mayor de edad (>= 18 años)? ${esMayorDeEdad}`);
```

## ¡A Tu Teclado! ⌨️

### Ejercicio 7.2.1:
Pide al usuario un número. Verifica e imprime:

- Si el número es igual a 10 (`true` o `false`).
- Si el número es diferente de 0 (`true` o `false`).
- Si el número es mayor que 100 (`true` o `false`).
- Si el número es menor o igual que 50 (`true` o `false`).

```javascript
// Escribe tu código aquí
const numero = parseInt(prompt("Ingresa un número: \n"));
console.log(`El numero ingresado es: ${numero}\n`);
console.log("El numero es Igual a 10?:", numero === 10);
console.log("El numero es Diferente a 0?: ", numero !== 0);
console.log("El numero es Mayor a 100?: ", numero > 100);
console.log("El numero es Menor a 50?: ", numero <= 50);
```

## 7.3 Operadores Lógicos: Combinando Verdades y Falsedades 🔗🧠
Estos operadores trabajan con valores booleanos (`true` o `false`) y nos permiten combinar varias condiciones.

- `&&` (Y lógico): Devuelve `true` solo si ambas condiciones que conecta son `true`.
  - `true && true`  → `true`
  - `true && false` → `false`
  - `false && true` → `false`
  - `false && false` → `false`

- `||` (O lógico): Devuelve `true` si al menos una de las condiciones que conecta es `true`.
  - `true || true`   → `true`
  - `true || false`  → `true`
  - `false || true`  → `true`
  - `false || false` → `false`

- `!` (NO lógico): Invierte el valor booleano de una condición.
  - `!true`  → `false`
  - `!false` → `true`

### Ejemplos Prácticos:

```javascript
// Operadores Lógicos
const haceSol = true;
const esFinDeSemana = true;
const tengoDinero = false;

// Ejemplo con '&&'
const puedoIrALaPlaya = haceSol && esFinDeSemana && tengoDinero;
console.log(`¿Puedo ir a la playa (hace sol Y es fin de semana)? ${puedoIrALaPlaya}`);

// Ejemplo con '||'
const puedoComprarHelado = tengoDinero || esFinDeSemana; // Quizás me invitan si es finde aunque no tenga dinero
console.log(`¿Puedo comprar helado (tengo dinero O es fin de semana)? ${puedoComprarHelado}`);

// Ejemplo con '!'
const noLlueve = !true; // Si "llueve" fuera false, "noLlueve" es true
console.log(`¿No está lloviendo? ${noLlueve}`);

// Combinando con comparaciones
const edad = 20;
const tienePermisoPadres = false;

const puedeEntrarAFiestaVip = (edad >= 18 && tengoDinero) || (edad < 18 && tienePermisoPadres);
console.log(`¿Puede entrar a la fiesta VIP? ${puedeEntrarAFiestaVip}`);
```

## ¡A Tu Teclado! ⌨️

### Ejercicio 7.3.1:
Declara dos variables booleanas: `estudiaMucho` y `asisteAClase`.
Evalúa e imprime el resultado de las siguientes condiciones:

- El aprendiz aprueba si `estudiaMucho` Y `asisteAClase`.
- El aprendiz podría necesitar ayuda si NO `estudiaMucho` O NO `asisteAClase`.

```javascript
// Escribe tu código aquí
const estudiaMucho = false;
const asisteAClase = false;

const aprendizAprueba = estudiaMucho && asisteAClase;
const necesitaAyuda = !estudiaMucho || !asisteAClase;

console.log(`El aprendiz aprueba? (Si estudia mucho y asiste a clase)? ${aprendizAprueba}`);
console.log(`El aprendiz necesita ayuda? (no estudia mucho o no asiste a clase): ${necesitaAyuda}`);
```

### Ejercicio 7.3.2:
Pide al usuario un número. Verifica e imprime `true` si el número está entre `1` y `100` (ambos inclusive), y `false` en caso contrario.
Pista: Necesitarás usar `&&` para verificar que sea `>= 1` Y `<= 100`.

```javascript
// Escribe tu código aquí
const numero = parseInt(prompt("Ingresa un número para verificar si está entre 1 y 100: "));
const numeroEnRango = numero >= 1 && numero <= 100;
console.log(`¿Número está en el rango [1-100]? ${numeroEnRango}`);
```

## 7.4 Operadores de Asignación Compuesta: ¡Abreviando Operaciones! ✍️➡️ shorthand
Son una forma más corta de escribir operaciones donde una variable se modifica a sí misma.

| Operador Compuesto | Equivalente a     | Ejemplo si x=57, y=100, z=2 |
|--------------------|-------------------|-----------------------------|
| `x += y`           | `x = x + y`       | x ← 57 + 100 :. x ← 157     |
| `x -= y`           | `x = x - y`       | x ← 57 - 100 :. x ← -43     |
| `x *= y`           | `x = x * y`       | x ← 57 * 100 :. x ← 5700    |
| `x /= z`           | `x = x / 2`       | x ← 57 / 2 :. x ← 28.5      |
| `x //= z`          | No directo; usa `x = Math.floor(x / z)` | x ← 57 / 2 :. x ← 28 |
| `x %= z`           | `x = x % z`       | x ← 57 % 2 :. x ← 1         |
| `x **= z`          | `x = x ** z`      | x ← 57 ** 2 :. x ← 3249     |

### Ejemplos Prácticos:

```javascript
// Operadores de Asignación Compuesta
let contador = 0;
console.log(`Valor inicial del contador: ${contador}`);

contador += 1;  // Equivalente a: contador = contador + 1
console.log(`Después de += 1: ${contador}`);

contador += 5;
console.log(`Después de += 5: ${contador}`);

let totalCompra = 10000;
const descuento = 2000;
totalCompra -= descuento; // totalCompra = totalCompra - descuento
console.log(`Total después de descuento (-= ${descuento}): ${totalCompra}`);

let multiplicador = 3;
multiplicador *= 2; // multiplicador = multiplicador * 2
console.log(`Multiplicador después de *= 2: ${multiplicador}`);

let saldo = 50.0;
saldo /= 2; // saldo = saldo / 2
console.log(`Saldo después de /= 2: ${saldo}`);
```

## ¡A Tu Teclado! ⌨️

### Ejercicio 7.4.1:
Tienes una variable `puntosJuego` inicializada en 100.

- El jugador gana 25 puntos. Actualiza `puntosJuego` usando `+=`.
- Luego, el jugador pierde 10 puntos. Actualiza `puntosJuego` usando `-=`.
- Finalmente, los puntos se duplican. Actualiza `puntosJuego` usando `*=`.
Imprime el valor de `puntosJuego` después de cada operación.

```javascript
// Escribe tu código aquí
let puntosJuego = 100;
console.log(`Puntos iniciales: ${puntosJuego}`);

puntosJuego += 25;
console.log(`Gana 25 puntos, Puntos totales: ${puntosJuego}`);

puntosJuego -= 10;
console.log(`Pierde 10 puntos, Puntos totales: ${puntosJuego}`);

puntosJuego *= 2;
console.log(`Duplica Puntos, Puntos totales: ${puntosJuego}`);
```

## 7.5 Precedencia y Asociatividad de Operadores: ¿Quién va Primero? 🚦
Cuando tienes una expresión con múltiples operadores, JavaScript necesita saber en qué orden evaluarlos. Esto se llama precedencia de operadores. Es similar a las reglas matemáticas (PEMDAS/BODMAS).

**Precedencia y asociatividad** son dos conceptos fundamentales que JavaScript utiliza para resolver expresiones matemáticas y lógicas complejas de manera consistente. La precedencia determina qué tipo de operador tiene prioridad sobre otros cuando están mezclados en una expresión; por ejemplo, en `2 + 3 * 4`, la multiplicación tiene mayor precedencia que la suma, por lo que se evalúa primero como `2 + (3 * 4) = 14`. Por otro lado, la asociatividad entra en juego cuando tenemos operadores del mismo nivel de precedencia y define la dirección en que se evalúan: de izquierda a derecha para la mayoría de operadores como en `10 - 5 - 2 = (10 - 5) - 2 = 3`, o de derecha a izquierda para casos especiales como la potencia en `2 ** 3 ** 2 = 2 ** (3 ** 2) = 512`. En esencia, la precedencia responde "¿cuál operador hago primero?" mientras que la asociatividad responde "¿en qué dirección evalúo cuando son del mismo nivel de precedencia?", trabajando juntas para garantizar que JavaScript interprete nuestras expresiones de manera predecible y matemáticamente correcta.

| Operador | Asociatividad             | Ejemplo                  |
|----------|---------------------------|--------------------------|
| `()`     | N/A                       | (2 + 3) * 4              |
| `**`     | Derecha a izquierda       | 2 ** 3 ** 2 = 2 ** (3 ** 2) |
| `*`, `/`, `%` | Izquierda a derecha | 8 / 4 / 2 = (8 / 4) / 2  |
| `+`, `-` | Izquierda a derecha       | 10 - 5 - 2 = (10 - 5) - 2 |
| `===`, `!==`, `>`, `<`, `>=`, `<=` | Izquierda a derecha | 1 < 2 < 3 = (1 < 2) && (2 < 3) |
| `!`      | Derecha a izquierda       | ! ! true = ! (! true)    |
| `&&`     | Izquierda a derecha       | A && B && C = (A && B) && C |
| `||`     | Izquierda a derecha       | A || B || C = (A || B) || C |

**Asociatividad:** Cuando operadores tienen la misma precedencia (ej. `*` y `/`), la asociatividad define el orden. La mayoría de los operadores aritméticos en JavaScript son asociativos a la izquierda (se evalúan de izquierda a derecha). `a / b * c` es `(a / b) * c`. La potencia `**` es asociativa a la derecha: `2 ** 3 ** 2` es `2 ** (3 ** 2)`, o sea `2 ** 9`.

**Recomendación:** Cuando tengas dudas, usa paréntesis para hacer explícito el orden de evaluación. Esto hace tu código más legible y evita errores.

### Ejemplos Prácticos:

```javascript
// Precedencia de Operadores
const resultado1 = 5 + 3 * 2;  // Primero 3*2=6, luego 5+6=11
console.log(`5 + 3 * 2 = ${resultado1}`);

const resultado2 = (5 + 3) * 2; // Primero (5+3)=8, luego 8*2=16
console.log(`(5 + 3) * 2 = ${resultado2}`);

const resultado3 = 10 / 2 * 5; // Izquierda a derecha: (10/2)=5, luego 5*5=25
console.log(`10 / 2 * 5 = ${resultado3}`);

// Precedencia con lógicos y comparaciones
const edad = 25;
const ingresos = 3000000;
const esSoltero = true;

const aplicaCredito = edad >= 18 && ingresos > 2500000 || !esSoltero;
// Evaluación:
// 1. edad >= 18 -> true
// 2. ingresos > 2500000 -> true
// 3. !esSoltero -> !true -> false
// 4. true && true (de 1 y 2) -> true
// 5. true || false (de 4 y 3) -> true
console.log(`¿Aplica para crédito? ${aplicaCredito}`);

const aplicaCreditoConParenthesis = (edad >= 18 && ingresos > 2500000) || (!esSoltero);
// Mismo resultado en este caso, pero los paréntesis aclaran
console.log(`¿Aplica para crédito (con paréntesis)? ${aplicaCreditoConParenthesis}`);
```

## ¡A Tu Teclado! ⌨️

### Ejercicio 7.5.1:
Predice el resultado de las siguientes expresiones y luego compruébalo en JavaScript:
- `10 - 2 ** 3 / 4 + 1`
- `(10 - 2) ** 3 / (4 + 1)`
- `5 * 2 // 3 % 2 == 1` (Nota: Usa `Math.floor(5 * 2 / 3) % 2 === 1`)
- `true || false && !true`

```javascript
// Escribe tu código aquí para comprobar
const calculo1 = 10 - 2 ** 3 / 4 + 1; // Debería ser ~9 (2**3=8, 8/4=2, 10-2+1=9)
console.log(calculo1);

const calculo2 = (10 - 2) ** 3 / (4 + 1); // 8**3=512, 512/5=102.4
console.log(calculo2);

const calculo3 = Math.floor(5 * 2 / 3) % 2 === 1; // Math.floor(10/3)=3, 3%2=1, true
console.log(calculo3);

const calculo4 = true || false && !true; // !true=false, false&&false=false, true||false=true
console.log(calculo4);
```

## 7.6 Expresiones: Construyendo Bloques de Lógica 🧱⚙️
Una expresión es cualquier fragmento de código que JavaScript puede evaluar para producir un valor.
Puede ser tan simple como un valor literal (`5`, `"Hola"`) o una variable (`miEdad`), o tan compleja como una combinación de valores, variables y múltiples operadores (`(base * altura) / 2 + offset`).

El resultado de una expresión siempre tiene un tipo de dato (`number`, `string`, `boolean`, etc.).

### Ejemplos de Expresiones:

```javascript
// Expresiones simples
5                           // Expresión que evalúa a 5 (number)
"SENA"                      // Expresión que evalúa a "SENA" (string)
true                        // Expresión que evalúa a true (boolean)

// Expresiones con variables
const miVariable = 10;
miVariable                 // Expresión que evalúa al valor de miVariable (10)
miVariable * 2             // Expresión que evalúa a 20

// Expresiones complejas
const calificacion1 = 4.5;
const calificacion2 = 3.0;
const calificacion3 = 5.0;
const promedioExp = (calificacion1 + calificacion2 + calificacion3) / 3; // Expresión que calcula el promedio
console.log(`El promedio calculado por la expresión es: ${promedioExp}`);

const esAprobadoExp = promedioExp >= 3.0; // Expresión booleana
console.log(`¿Está aprobado según la expresión? ${esAprobadoExp}`);
```

Dominar cómo se construyen y evalúan las expresiones es clave para escribir programas que hagan cálculos y tomen decisiones.

¡Desafíate! 🤯

- Reto 7.1: Calculadora de Área y Perímetro de un Rectángulo

  1. Pide al usuario la base de un rectángulo (puede ser flotante).
  2. Pide al usuario la altura de un rectángulo (puede ser flotante).
  3. Calcula el área (`base * altura`).
  4. Calcula el perímetro (`2 * (base + altura)`).
  5. Muestra los resultados del área y el perímetro usando template literals.
  
Asegúrate de usar paréntesis en la fórmula del perímetro para garantizar el orden correcto de las operaciones.

```javascript
// Escribe tu código aquí
console.log("--- Calculadora de Rectángulos ---");
const baseRectangulo = parseFloat(prompt("Ingrese la base del rectangulo: "));
const alturaRectangulo = parseFloat(prompt("Ingrese la altura del rectangulo: "));
const sistemaUnidades = prompt("Ingrese el sistema de unidades: ");

const areaRectangulo = baseRectangulo * alturaRectangulo;
const perimetroRectangulo = 2 * (baseRectangulo + alturaRectangulo);

console.log(`La base ingresada es de: ${baseRectangulo} y la altura ingresada es de: ${alturaRectangulo}\n`);
console.log(`El area del rectangulo es: ${areaRectangulo} ${sistemaUnidades}^2 y el perimetro del rectangulo es: ${perimetroRectangulo} ${sistemaUnidades}`);
```

---
