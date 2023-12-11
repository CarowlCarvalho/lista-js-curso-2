Dominar o uso de arrays é fundamental para qualquer programador, sendo uma base essencial na manipulação de dados. Praticar regularmente é a chave para se tornar mais  confiante na manipulação de arrays, capacitando-o para desenvolver soluções mais eficazes.

Para isso criamos uma lista de exercícios que não apenas ajudam a explorar os métodos de manipulação de arrays, mas também vão te preparar para lidar eficientemente com dados em aplicações reais. 

1)Faça uma função que aceite vários arrays como argumentos e retorne um único array contendo todos os elementos dos arrays fornecidos utilizando Spread Operator.

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

2)Tendo como base o array `const numeros = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]`, utilize **filter** para criar um novo array chamado `numerosPares` contendo apenas os números pares do array original.

```
const numeros = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10];
const numerosPares = numeros.filter(numero => numero % 2 === 0);
console.log("Números pares:", numerosPares);
```

3)Crie um array de números chamado `valores`. Depois,escreva um programa que some todos os elementos deste array utilizando o método **reduce**.
```
const valores = [10, 20, 30, 40, 50];
const soma = valores.reduce((acumulador, valorAtual) => acumulador + valorAtual, 0);
console.log("Soma dos valores:", soma);
```
4)Considere duas listas de cores `const coresLista1 = ['Vermelho', 'Verde', 'Azul', 'Amarelo', 'Vermelho']`, `const coresLista2 = ['Laranja', 'Verde', 'Roxo', 'Azul']`. Crie um programa que una essas duas listas, removendo cores duplicadas e exiba a lista final.

Resolução:

```
const coresLista1 = ['Vermelho', 'Verde', 'Azul', 'Amarelo', 'Vermelho'];
const coresLista2 = ['Laranja', 'Verde', 'Roxo', 'Azul'];

const coresUnicas = [...new Set([...coresLista1, ...coresLista2])];
console.log("Cores sem repetir: ", coresUnicas);

```
5)Com base na lista de valores `const valores = [10.5, 20.75, 30.25, 40, 50.5]`, crie um programa que receba essa lista de valores, realize a soma de todos esses valores utilizando reduce e imprima o total no final.
```
const valores = [10.5, 20.75, 30.25, 40, 50.5];
const soma = valores.reduce((acumulador, valorAtual) => acumulador + valorAtual, 0);
console.log("Total dos valores:", soma.toFixed(2));
```
