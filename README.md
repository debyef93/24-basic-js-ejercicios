# Ejercicios JS

Empieza FORKEANDO (<svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-repo-forked mr-2">
    <path d="M5 5.372v.878c0 .414.336.75.75.75h4.5a.75.75 0 0 0 .75-.75v-.878a2.25 2.25 0 1 1 1.5 0v.878a2.25 2.25 0 0 1-2.25 2.25h-1.5v2.128a2.251 2.251 0 1 1-1.5 0V8.5h-1.5A2.25 2.25 0 0 1 3.5 6.25v-.878a2.25 2.25 0 1 1 1.5 0ZM5 3.25a.75.75 0 1 0-1.5 0 .75.75 0 0 0 1.5 0Zm6.75.75a.75.75 0 1 0 0-1.5.75.75 0 0 0 0 1.5Zm-3 8.75a.75.75 0 1 0-1.5 0 .75.75 0 0 0 1.5 0Z"></path></svg> arriba a la derecha) este repositorio. Luego clonalo en tu espacio de trabajo

## Fase 1: Acceso a arrays

Estos ejercicios te permitirán practicar y profundizar en el acceso y manipulación de arrays y matrices en JavaScript. ¡Buena suerte!

### Nivel 1: Acceder a Arrays Simples

1. **Acceder a Elementos del Array:**

- Crea un array llamado `colors` con los colores "rojo", "verde", "azul", "amarillo".
- Imprime el tercer color del array.

```javascript
let colors = ["rojo", "verde", "azul", "amarillo"];
console.log(colors[2]); // azul
```

2. **Último Elemento del Array:**

- Imprime el último elemento del array `colors` sin usar su índice explícitamente.

```javascript
console.log(colors[colors.length - 1]); // amarillo
```

### Nivel 2: Acceder a Arrays de Arrays (Matrices)

3. **Acceder a Elementos en una Matriz:**

- Crea una matriz `matrix` que represente la siguiente tabla:

``` javascript
    1 2 3
    4 5 6
    7 8 9
```

- Imprime el número que se encuentra en la segunda fila y tercera columna.

```javascript
let matrix = [
    [1, 2, 3],
    [4, 5, 6],
    [7, 8, 9]
];
console.log(matrix[1][2]); // 6
```

4. **Cambiar Elementos en una Matriz:**

- Cambia el elemento en la primera fila y segunda columna a 20.
- Imprime la matriz modificada.

```javascript
matrix[0][1] = 20;
console.log(matrix);
// [
//   [1, 20, 3],
//   [4, 5, 6],
//   [7, 8, 9]
// ]
```

### Nivel 3: Recorrer Arrays y Matrices

5. **Recorrer un Array Simple:**

- Usa un bucle `for` para imprimir todos los elementos del array `colors`.

```javascript
for (let i = 0; i < colors.length; i++) {
    console.log(colors[i]);
}
```

6. **Recorrer una Matriz:**

- Usa un bucle `for` anidado para imprimir todos los elementos de la matriz `matrix`.

```javascript
for (let i = 0; i < matrix.length; i++) {
    for (let j = 0; j < matrix[i].length; j++) {
        console.log(matrix[i][j]);
    }
}
```

### Nivel 4: Manipulación Avanzada de Matrices

7. **Sumar Todos los Elementos de una Matriz:**

- Escribe una función que reciba una matriz y devuelva la suma de todos sus elementos.

```javascript
function sumMatrix(matrix) {
    let sum = 0;
    for (let i = 0; i < matrix.length; i++) {
        for (let j = 0; j < matrix[i].length; j++) {
            sum += matrix[i][j];
        }
    }
    return sum;
}

console.log(sumMatrix(matrix)); // 45
```

8. **Transponer una Matriz:**

- Escribe una función que reciba una matriz y devuelva su transpuesta (intercambiar filas por columnas).

```javascript
function transpose(matrix) {
    let transposed = [];
    for (let i = 0; i < matrix[0].length; i++) {
        transposed[i] = [];
        for (let j = 0; j < matrix.length; j++) {
            transposed[i][j] = matrix[j][i];
        }
    }
    return transposed;
}

let transposedMatrix = transpose(matrix);
console.log(transposedMatrix);
// [
//   [1, 4, 7],
//   [20, 5, 8],
//   [3, 6, 9]
// ]
```

### Nivel 5: Desafíos Adicionales

9. **Acceder a Elementos Diagonales de una Matriz:**

- Escribe una función que imprima los elementos en la diagonal principal de una matriz cuadrada.

```javascript
function printDiagonal(matrix) {
    for (let i = 0; i < matrix.length; i++) {
        console.log(matrix[i][i]);
    }
}

printDiagonal(matrix);
// 1
// 5
// 9
```

10. **Rotar una Matriz 90 Grados:**

- Escribe una función que rote una matriz cuadrada 90 grados en el sentido de las agujas del reloj.

```javascript
function rotateMatrix(matrix) {
    let n = matrix.length;
    let rotated = [];
    for (let i = 0; i < n; i++) {
        rotated[i] = [];
        for (let j = 0; j < n; j++) {
            rotated[i][j] = matrix[n - j - 1][i];
        }
    }
    return rotated;
}

let rotatedMatrix = rotateMatrix(matrix);
console.log(rotatedMatrix);
// [
//   [7, 4, 1],
//   [8, 5, 20],
//   [9, 6, 3]
// ]
```

## Fase 2: Métodos avanzados

La información en [w3schools](https://www.w3schools.com/) te puede ser de ayuda

- [Arrays](https://www.w3schools.com/js/js_arrays.asp)
- [Array Methods](https://www.w3schools.com/js/js_array_methods.asp)

### Nivel 1: Fundamentos de Arrays

11. **Crear y Acceder a Arrays:**

- Crea un array llamado `fruits` que contenga las frutas "manzana", "banana" y "naranja".
- Imprime el primer y el último elemento del array.

```javascript
let fruits = ["manzana", "banana", "naranja"];
console.log(fruits[0]); // manzana
console.log(fruits[2]); // naranja
```

12. **Modificar Arrays:**

- Añade "uva" al final del array `fruits`.
- Cambia el segundo elemento del array a "kiwi".
- Elimina el primer elemento del array.

```javascript
fruits.push("uva");
fruits[1] = "kiwi";
fruits.shift();
console.log(fruits); // ["kiwi", "naranja", "uva"]
```

### Nivel 2: Métodos de Arrays

13. **Uso de Métodos Básicos:**

- Crea un array llamado `numbers` con los números del 1 al 5.
- Usa el método `map` para crear un nuevo array que contenga el cuadrado de cada número.
- Usa el método `filter` para crear un nuevo array que contenga solo los números mayores que 2.

```javascript
let numbers = [1, 2, 3, 4, 5];
let squares = numbers.map((num) => num * num);
let greaterThanTwo = numbers.filter((num) => num > 2);
console.log(squares); // [1, 4, 9, 16, 25]
console.log(greaterThanTwo); // [3, 4, 5]
```

14. **Recorrer Arrays:**

- Usa un bucle `for` para imprimir cada elemento del array `fruits` en mayúsculas.

```javascript
for (let i = 0; i < fruits.length; i++) {
  console.log(fruits[i].toUpperCase());
}
```

### Nivel 3: Manipulación Avanzada de Arrays

15. **Reducir Arrays:**

- Usa el método `reduce` para calcular la suma de todos los elementos del array `numbers`.

```javascript
let sum = numbers.reduce((acc, num) => acc + num, 0);
console.log(sum); // 15
```

16. **Combinación de Arrays:**

- Crea un nuevo array combinando `fruits` y `numbers`.
- Ordena el nuevo array en orden alfabético o numérico según corresponda.

```javascript
let combined = fruits.concat(numbers);
combined.sort(); // Esto ordenará en orden lexicográfico
console.log(combined);
```

### Nivel 4: Ejercicios Prácticos

17. **Eliminar Duplicados:**

- Dado un array `randomNumbers` con números aleatorios, crea una función para eliminar los duplicados.

```javascript
let randomNumbers = [1, 2, 3, 3, 4, 5, 5, 6];
let uniqueNumbers = [...new Set(randomNumbers)];
console.log(uniqueNumbers); // [1, 2, 3, 4, 5, 6]
```

18. **Encontrar Elementos Comunes:**

- Dado dos arrays `array1` y `array2`, encuentra los elementos comunes entre ellos.

```javascript
let array1 = [1, 2, 3, 4];
let array2 = [3, 4, 5, 6];
let commonElements = array1.filter((value) => array2.includes(value));
console.log(commonElements); // [3, 4]
```

### Nivel 5: Algoritmos con Arrays

19. **Rotar un Array:**

- Escribe una función para rotar un array hacia la derecha `n` veces.

```javascript
function rotateArray(arr, n) {
  n = n % arr.length;
  return arr.slice(-n).concat(arr.slice(0, -n));
}
let rotated = rotateArray([1, 2, 3, 4, 5], 2);
console.log(rotated); // [4, 5, 1, 2, 3]
```

20. **Buscar el Elemento Mayor:**

- Escribe una función que encuentre el elemento mayor en un array de números.

```javascript
function findMax(arr) {
  return Math.max(...arr);
}
let max = findMax([1, 2, 3, 4, 5]);
console.log(max); // 5
```

### Ejercicio Final

Fácil de explicar, dificil de hacer:

Empieza un nuevo repositorio. Implementa el [juego del ahorcado](https://es.wikipedia.org/wiki/Ahorcado_(juego))

Puedes hacrlo tan solo con JS, o añadirle un frontend con HTML y CSS

*Esta funcion para elegir un numero al azar te puede resultar util:*

```javascript
let max = 10;
let randomInt = Math.floor(Math.random() \* max);
console.log(randomInt); // Por ejemplo, un número entre 0 y 9
```
