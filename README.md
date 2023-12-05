Dominar o uso de arrays é fundamental para qualquer programador, sendo uma base essencial na manipulação de dados. Praticar regularmente é a chave para se tornar mais  confiante na manipulação de arrays, capacitando-o para desenvolver soluções mais eficazes.

Para isso criamos uma lista de exercícios que não apenas ajudam a explorar os métodos de manipulação de arrays, mas também vão te preparar para lidar eficientemente com dados em aplicações reais. 

Slice e Splice em Arrays:
1)Crie uma função que receba um array e retorne uma cópia dele, mas apenas com os elementos do índice 2 ao índice 4.

```
function sliceArray(arr) {
    return arr.slice(2, 5); // Retorna os elementos do índice 2 ao 4 (não inclui o índice 5)
}

const originalArray = [1, 2, 3, 4, 5, 6];
const slicedArray = sliceArray(originalArray);
console.log(slicedArray); // Saída: [3, 4, 5]
```

Concatenação de Arrays:
2)Crie uma função que receba dois arrays e os concatene em um único array.
Resolução:

```
function concatenateArrays(arr1, arr2) {
    return arr1.concat(arr2); // Concatena os dois arrays
}

const array1 = [1, 2, 3];
const array2 = [4, 5, 6];
const concatenatedArray = concatenateArrays(array1, array2);
console.log(concatenatedArray); // Saída: [1, 2, 3, 4, 5, 6]

```

Laço de Repetição (for/of):
3)Escreva um código que utilize o loop for/of para iterar e imprimir cada elemento de um array.

```
function printArrayElements(arr) {
    for (let element of arr) {
        console.log(element); // Imprime cada elemento do array
    }
}

const myArray = ['a', 'b', 'c'];
printArrayElements(myArray);
// Saída:
// a
// b
// c


```

Funções de Callback:
4)Crie uma função que receba um array e uma função de callback para executar uma operação em cada elemento do array.

```
function manipulateArray(arr, callback) {
    return arr.map(callback); // Executa a função de callback em cada elemento do array
}

function doubleNumber(num) {
    return num * 2; // Função de exemplo para dobrar o número
}

const originalNumbers = [1, 2, 3];
const doubledNumbers = manipulateArray(originalNumbers, doubleNumber);
console.log(doubledNumbers); // Saída: [2, 4, 6]
```

Somando Elementos de um Array:
5)Crie uma função que receba um array de números e retorne a soma de todos os elementos.

```
function sumArrayElements(arr) {
    return arr.reduce((acc, curr) => acc + curr, 0); // Soma os elementos do array
}

const numbers = [1, 2, 3, 4, 5];
const totalSum = sumArrayElements(numbers);
console.log(totalSum); // Saída: 15
```

6)Filtrando Elementos de um Array:
Escreva uma função que receba um array de números e retorne apenas os números pares.

```
function filterEvenNumbers(arr) {
    return arr.filter(num => num % 2 === 0); // Filtra apenas os números pares
}

const numArray = [1, 2, 3, 4, 5, 6];
const evenNumbers = filterEvenNumbers(numArray);
console.log(evenNumbers); // Saída: [2, 4, 6]
```

Trabalhando com `forEach`:

7)Utilize o método forEach para imprimir cada elemento de um array juntamente com seu índice.

```
let numero = 7;
let resultado = numero % 2 === 0 ? "Par" : "Ímpar";
console.log(resultado); // Par ou Ímpar
```

Função Callback e Modificação de Array:
8)Crie uma função que receba um array de números e aplique uma operação específica a cada elemento, utilizando uma função callback para determinar a operação.

```
function modifyArray(arr, callback) {
    return arr.map(callback); // Aplica a função de callback a cada elemento do array
}

function squareNumber(num) {
    return num * num; // Função de exemplo para elevar ao quadrado
}

const originalNums = [1, 2, 3, 4];
const squaredNums = modifyArray(originalNums, squareNumber);
console.log(squaredNums); // Saída: [1, 4, 9, 16]
```

Concatenação de Arrays usando Spread Operator:
9)Faça uma função que aceite vários arrays como argumentos e retorne um único array contendo todos os elementos dos arrays fornecidos.

```
function concatArrays(...arrays) {
    return [].concat(...arrays); // Usa o operador spread para concatenar os arrays
}

const arr1 = [1, 2];
const arr2 = [3, 4];
const arr3 = [5, 6];
const concatenated = concatArrays(arr1, arr2, arr3);
console.log(concatenated); // Saída: [1, 2, 3, 4, 5, 6]
```

Filtrando Elementos com mais de uma Condição:

10)Crie uma função que filtre os números de um array que são múltiplos de 3 e maiores que 5.

```
function filterNumbers(arr) {
    return arr.filter(num => num % 3 === 0 && num > 5); // Filtra números múltiplos de 3 e maiores que 5
}

const numbersArray = [3, 6, 9, 4, 12, 2, 7];
const filteredNumbers = filterNumbers(numbersArray);
console.log(filteredNumbers); // Saída: [6, 9, 12]
```
