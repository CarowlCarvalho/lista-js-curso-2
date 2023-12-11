Dominar o uso de arrays é fundamental para qualquer programador, sendo uma base essencial na manipulação de dados. Praticar regularmente é a chave para se tornar mais  confiante na manipulação de arrays, capacitando-o para desenvolver soluções mais eficazes.

Para isso criamos uma lista de exercícios que não apenas ajudam a explorar os métodos de manipulação de arrays, mas também vão te preparar para lidar eficientemente com dados em aplicações reais. 

1)Crie uma função que receba dois arrays e os concatene em um único array.
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

2)Crie um array chamado numeros contendo números de 1 a 10. Utilize o método slice para criar um novo array chamado parteNumeros que contenha apenas os números de índice 3 a 7 de numeros.
```
const numeros = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10];
const parteNumeros = numeros.slice(3, 8);
console.log("Parte dos números:", parteNumeros);
```

3)Dado o array frutas contendo frutas que desejamos comprar na feira `let frutas = ["Maçã", "Banana", "Laranja", "Limão", "Abacaxi"]`, utilize o método splice para remover as frutas no índice 2 e 3 e, em seguida, adicione as frutas "Kiwi" e "Pêssego" nesses mesmos índices.
```
4)Crie dois arrays chamados menuPrincipal e menuDeSobremesas contendo opções do cardápio de um restaurante. Utilize o método concat para criar um novo array chamado menuCompleto que contenha todos os elementos de menuPrincipal seguidos pelos elementos de menuDeSobremesas .
```
const menuPrincipal = ["lasanha", "feijoada", "macarronada"];
const menuDeSobremesas = ["pudim", "sorvete", "brigadeiro"];
const menuCompleto = menuPrincipal .concat(menuDeSobremesas );
console.log("Veja o menu completo: ", menuCompleto );
```
5)Crie uma lista bidimensional chamada matriz com 3 linhas e 3 colunas, onde cada elemento seja uma matriz 3x3 com valores iniciando em 1 e aumentando em 1 a cada elemento.
```
let matriz = [];
let valorInicial = 1;

for (let i = 0; i < 3; i++) {
  let linha = [];
  for (let j = 0; j < 3; j++) {
    linha.push(valorInicial++);
  }
  matriz.push(linha);
}

console.log("Matriz de duas dimensões:");
matriz.forEach(row => console.log(row));
```

6)Acesse e imprima o elemento na segunda linha e terceira coluna da lista bidimensional matriz criada no exercício anterior.
```
console.log("Elemento na segunda linha e terceira coluna:", matriz[1][2]);
```

7)Adicione um novo elemento (por exemplo,`15`) na terceira linha e segunda coluna da lista bidimensional matriz criada anteriormente.
```
matriz[2][1] = 15;
console.log("Matriz após adição de elemento:", matriz);
```
