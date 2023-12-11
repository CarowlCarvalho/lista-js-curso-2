Dominar o uso de arrays é fundamental para qualquer programador, sendo uma base essencial na manipulação de dados. Praticar regularmente é a chave para se tornar mais  confiante na manipulação de arrays, capacitando-o para desenvolver soluções mais eficazes.

Para isso criamos uma lista de exercícios que não apenas ajudam a explorar os métodos de manipulação de arrays, mas também vão te preparar para lidar eficientemente com dados em aplicações reais. 

Laço de Repetição (for/of):
1)Escreva um código que utilize o loop for/of para iterar e imprimir cada elemento de um array.

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

2)Crie uma função que receba uma array e imprima no console o número do índice e o elemento.

```
const listinha = ["banana", "gatinho", "brócolis"]

function imprimeIndiceEElemento(arr) {
  for (let i = 0; i < arr.length; i++) {
    console.log(`índice ${i}, elemento ${arr[i]}`)
  }
}

imprimeIndiceEElemento(listinha )
```
3) Crie uma função que receba uma array de números inteiros e retorne a soma dos elementos.
```
const arrNums = [10,11,12,10,11,12,10,11,12,10,11,12]

function soma(arr) {
  let total = 0
  for (let i = 0; i < arr.length; i++) {
    total += arr[i]
  }
  return total
}

console.log(soma(arrNums))
```

4)Crie uma função que receba uma array de números inteiros e retorne o menor valor e o maior valor da array, no seguinte formato: "o menor número é X e o maior número é Y".
```
const arrMenoresMaiores = [5, 37, 18, 59, 12, -5]

function imprimeMaiorEMenor(arr) {

  let maior = 0
  let menor = 0

  for(let i = 0; i < arr.length; i++) {
    if (arr[i] > maior) {
      maior = arr[i]
    }
    if (arr[i] < menor) {
      menor = arr[i]
    }
  }
  return `o maior número é ${maior} e o menor número é ${menor}`
}

console.log(imprimeMaiorEMenor(arrMenoresMaiores))
```

5)Crie um programa que utilize um laço for para percorrer uma array `const numeros = [3, 8, 12, 5, 6, 10, 7, 2, 9, 14]` e exibir apenas os números pares contidos nesse array no console.

```
const numeros = [3, 8, 12, 5, 6, 10, 7, 2, 9, 14];
console.log("Números pares do array:");

for (let i = 0; i < numeros.length; i++) {
  if (numeros[i] % 2 === 0) {
    console.log(numeros[i]);
  }
}
```

6)Crie um programa que calcule a média dos números presentes em um array utilizando um loop for.

```
const numeros = [10, 8, 6, 9, 7, 5];
let soma = 0;

for (let i = 0; i < numeros.length; i++) {
  soma += numeros[i];
}

const media = soma / numeros.length;
console.log("Array:", numeros);
console.log("Média dos números:", media);


```

