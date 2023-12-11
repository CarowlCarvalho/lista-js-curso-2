Dominar o uso de arrays é fundamental para qualquer programador, sendo uma base essencial na manipulação de dados. Praticar regularmente é a chave para se tornar mais  confiante na manipulação de arrays, capacitando-o para desenvolver soluções mais eficazes.

Para isso criamos uma lista de exercícios que não apenas ajudam a explorar os métodos de manipulação de arrays, mas também vão te preparar para lidar eficientemente com dados em aplicações reais. 

1)Crie uma função que receba 3 parâmetros: o nome de um livro, a quantidade de páginas e a autoria. Retorne um objeto no formato: {titulo: "nome do livro", paginas: "número de páginas", autoria: "nome da pessoa"}
```
function objLivro(titulo, paginas, autoria) {
  return ({
    titulo, // mesma coisa que titulo: titulo
    paginas,
    autoria
  }) // parenteses para retornar o objeto diretamente
}

console.log(objLivro('Antes do Baile Verde', 234, 'Lygia Fagundes Telles'))
```

2)Escreva uma função que receba um array de números e retorne um array contendo apenas os números pares.

```
function filterEvenNumbers(arr) {
    return arr.filter(num => num % 2 === 0); // Filtra apenas os números pares
}

const numArray = [1, 2, 3, 4, 5, 6];
const evenNumbers = filterEvenNumbers(numArray);
console.log(evenNumbers); // Saída: [2, 4, 6]
```


3)Crie uma função que receba um array de números e retorne a soma de todos os elementos.

```
function sumArrayElements(arr) {
    return arr.reduce((acc, curr) => acc + curr, 0); // Soma os elementos do array
}

const numbers = [1, 2, 3, 4, 5];
const totalSum = sumArrayElements(numbers);
console.log(totalSum); // Saída: 15
```


4)Crie uma função que filtre os números de um array que são múltiplos de 3 e maiores que 5.

```
function filterNumbers(arr) {
    return arr.filter(num => num % 3 === 0 && num > 5); // Filtra números múltiplos de 3 e maiores que 5
}

const numbersArray = [3, 6, 9, 4, 12, 2, 7];
const filteredNumbers = filterNumbers(numbersArray);
console.log(filteredNumbers); // Saída: [6, 9, 12]
```

5)Crie um array vazio chamado `minhaArray` e adicione 3 números inteiros de sua escolha utilizando o método push(). Depois, imprima no console os itens presentes no array para verificar se os números foram adicionados e substitua o primeiro elemento do array (índice 0) pelo dobro do seu valor atual. Imprima no console o array atualizado para verificar a mudança.

```
let minhaArray = []; // Criando um array vazio
minhaArray.push(5); // Adicionando números ao array
minhaArray.push(10);
minhaArray.push(15);

//Exibição dos Itens
console.log("Itens no array minhaArray:", minhaArray);

//Atualização de Itens
minhaArray[0] *= 2; // Dobrando o valor do primeiro elemento
console.log("Array após a atualização do primeiro elemento:", minhaArray);
```

 6) Crie uma função que receba uma array de números inteiros e retorne o menor valor e o maior valor da array, no seguinte formato: "o menor número é X e o maior número é Y".
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

