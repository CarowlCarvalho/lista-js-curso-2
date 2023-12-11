Dominar o uso de arrays é fundamental para qualquer programador, sendo uma base essencial na manipulação de dados. Praticar regularmente é a chave para se tornar mais  confiante na manipulação de arrays, capacitando-o para desenvolver soluções mais eficazes.

Para isso criamos uma lista de exercícios que não apenas ajudam a explorar os métodos de manipulação de arrays, mas também vão te preparar para lidar eficientemente com dados em aplicações reais. 

1)Utilize o método forEach para imprimir cada elemento de um array juntamente com seu índice.
```
const meuArray = ['a', 'b', 'c', 'd', 'e'];

meuArray.forEach((elemento, indice) => {
  console.log(`Índice: ${indice}, Valor: ${elemento}`);
});
```

2)Crie uma função chamada `executarOperacaoEmArray` que recebe dois parâmetros: um array e uma função de callback. Essa função deve iterar por cada elemento do array e aplicar a função de callback em cada um dos elementos.

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

3)Você recebeu um array chamado numeros contendo valores. Crie um programa que verifique se um número específico está presente nesse array. Se estiver, o programa deve retornar a posição (índice) desse número. Caso contrário, se o número não estiver presente, o programa deve retornar "-1".
```
const numeros = [10, 20, 30, 40, 50];
const numeroProcurado = 30;
let posicao = -1;

for (let i = 0; i < numeros.length; i++) {
  if (numeros[i] === numeroProcurado) {
    posicao = i;
    break;
  }
}

console.log(`Posição do número ${numeroProcurado}: ${posicao}`);
```

4) Dado o array chamado frutas `const frutas = ["Maçã", "Banana", "Laranja", "Morango", "Abacaxi"];` contendo diferentes tipos de frutas. Escreva um programa que utilize o laço for para imprimir cada fruta presente no array, uma por linha.
```
const frutas = ["Maçã", "Banana", "Laranja", "Morango", "Abacaxi"];

for (let i = 0; i < frutas.length; i++) {
  console.log(frutas[i]);
}

```

5) Com base em um array chamado `notas` contendo as notas de um aluno `const notas = [8, 7, 6, 9, 8]`, crie um programa que calcule a média dessas notas e a exiba no console.
```
const notas = [8, 7, 6, 9, 8];
let soma = 0;

for (let i = 0; i < notas.length; i++) {
  soma += notas[i];
}

const media = soma / notas.length;
console.log("Média das notas:", media);
```
