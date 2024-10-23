## Este é um dicionário de ARRAY em JavaScript

> Join - Este método consegue juntar os elementos de uma array
```js
>const elements = ['Fire', 'Air', 'Water'];
console.log(elements.join());
// Saída: "Fire,Air,Water"
console.log(elements.join(''));
// Saída: "FireAirWater"
console.log(elements.join('-'));
// Saída: "Fire-Air-Water"
```

> slice- divide a quantidade de elementos num array.
```js
//Método .length = Contagem de elementos em uma array
const livros = ["TypeScript", "JavaScript", "Node.js",  "Python", "C", "C++", "C#", "F#"];
const TamLivros = livros.length;
const corredorA1 = livros.slice(0, TamLivros/4);
const corredorA2 = livros.slice(TamLivros/4);
console.log("Os livros do corredor A1 são: ", corredorA1);
console.log("Os livros do corredor A2 são: ", corredorA2);
```

> .concat
```js
// Concatenação de arrays (.concat) - Juntando a lista livros com a lista HQ. 
// Método .sort() (Parâmetro vazio), posiciona os elementos em ordem alfabética.
const livros = ["TypeScript", "JavaScript", "Node.js",  "Python", "C", "C++", "C#", "F#"];
const HQ = ["Batman: Ano Um", "Watchmen", "Sandman", "V de Vingança", "Maus", "Spider-Man"];
const juncao = livros.concat(HQ);
console.log(juncao.sort());
```

> Array2D.js - livro e prateleira
```js
//Lista de 2 dimensões
// O 1° [index] (LivrosePrateleiras) Representa os itens da lista, o 2° representa o que existe dentro do item da lista.
const Livros = ["JavaScript Assertivo", "Angular", "Clean code"];
const Prateleira = [3, 4, 1];
const LivrosePrateleiras = [Livros, Prateleira];
console.log(`O livro ${LivrosePrateleiras[0][2]}, está na prateleira: ${LivrosePrateleiras[1][2]}`);
```
