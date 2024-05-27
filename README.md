# Ejercicios JS

Empieza FORKEANDO (<svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-repo-forked mr-2">
    <path d="M5 5.372v.878c0 .414.336.75.75.75h4.5a.75.75 0 0 0 .75-.75v-.878a2.25 2.25 0 1 1 1.5 0v.878a2.25 2.25 0 0 1-2.25 2.25h-1.5v2.128a2.251 2.251 0 1 1-1.5 0V8.5h-1.5A2.25 2.25 0 0 1 3.5 6.25v-.878a2.25 2.25 0 1 1 1.5 0ZM5 3.25a.75.75 0 1 0-1.5 0 .75.75 0 0 0 1.5 0Zm6.75.75a.75.75 0 1 0 0-1.5.75.75 0 0 0 0 1.5Zm-3 8.75a.75.75 0 1 0-1.5 0 .75.75 0 0 0 1.5 0Z"></path></svg> arriba a la derecha) este repositorio. Luego clonalo en tu espacio de trabajo

## Fase 1: Acceso a arrays

Estos ejercicios te permitirán practicar y profundizar en el acceso y manipulación de arrays y matrices en JavaScript. ¡Buena suerte!

### Nivel 1: Acceder a Arrays Simples

1. **Acceder a Elementos del Array:**

- Crea un array llamado `colors` con los colores "rojo", "verde", "azul", "amarillo".
- Imprime el tercer color del array.

2. **Último Elemento del Array:**

- Imprime el último elemento del array `colors` sin usar su índice explícitamente.

### Nivel 2: Acceder a Arrays de Arrays (Matrices)

3. **Acceder a Elementos en una Matriz:**

- Crea una matriz `matrix` que represente la siguiente tabla:

- Imprime el número que se encuentra en la segunda fila y tercera columna.

4. **Cambiar Elementos en una Matriz:**

- Cambia el elemento en la primera fila y segunda columna a 20.
- Imprime la matriz modificada.

### Nivel 3: Recorrer Arrays y Matrices

5. **Recorrer un Array Simple:**

- Usa un bucle `for` para imprimir todos los elementos del array `colors`.

6. **Recorrer una Matriz:**

- Usa un bucle `for` anidado para imprimir todos los elementos de la matriz `matrix`.

### Nivel 4: Manipulación Avanzada de Matrices

7. **Sumar Todos los Elementos de una Matriz:**

- Escribe una función que reciba una matriz y devuelva la suma de todos sus elementos.

8. **Transponer una Matriz:**

- Escribe una función que reciba una matriz y devuelva su transpuesta (intercambiar filas por columnas).

### Nivel 5: Desafíos Adicionales

9. **Acceder a Elementos Diagonales de una Matriz:**

- Escribe una función que imprima los elementos en la diagonal principal de una matriz cuadrada.

10. **Rotar una Matriz 90 Grados:**

- Escribe una función que rote una matriz cuadrada 90 grados en el sentido de las agujas del reloj.

## Fase 2: Métodos avanzados

La información en [w3schools](https://www.w3schools.com/) te puede ser de ayuda

- [Arrays](https://www.w3schools.com/js/js_arrays.asp)
- [Array Methods](https://www.w3schools.com/js/js_array_methods.asp)

### Nivel 1: Fundamentos de Arrays

11. **Crear y Acceder a Arrays:**

- Crea un array llamado `fruits` que contenga las frutas "manzana", "banana" y "naranja".
- Imprime el primer y el último elemento del array.

12. **Modificar Arrays:**

- Añade "uva" al final del array `fruits`.
- Cambia el segundo elemento del array a "kiwi".
- Elimina el primer elemento del array.

### Nivel 2: Métodos de Arrays

13. **Uso de Métodos Básicos:**

- Crea un array llamado `numbers` con los números del 1 al 5.
- Usa el método `map` para crear un nuevo array que contenga el cuadrado de cada número.
- Usa el método `filter` para crear un nuevo array que contenga solo los números mayores que 2.

14. **Recorrer Arrays:**

- Usa un bucle `for` para imprimir cada elemento del array `fruits` en mayúsculas.

### Nivel 3: Manipulación Avanzada de Arrays

15. **Reducir Arrays:**

- Usa el método `reduce` para calcular la suma de todos los elementos del array `numbers`.

16. **Combinación de Arrays:**

- Crea un nuevo array combinando `fruits` y `numbers`.
- Ordena el nuevo array en orden alfabético o numérico según corresponda.

### Nivel 4: Ejercicios Prácticos

17. **Eliminar Duplicados:**

- Dado un array `randomNumbers` con números aleatorios, crea una función para eliminar los duplicados.

18. **Encontrar Elementos Comunes:**

- Dado dos arrays `array1` y `array2`, encuentra los elementos comunes entre ellos.

### Nivel 5: Algoritmos con Arrays

19. **Rotar un Array:**

- Escribe una función para rotar un array hacia la derecha `n` veces.

20. **Buscar el Elemento Mayor:**

- Escribe una función que encuentre el elemento mayor en un array de números.

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
