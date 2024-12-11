*Vítor Vieira de Souza*

**ADS040-1T**

# Resumo das aulas, </>_01 #
Neste Arquivo está exposto, em forma de um resumo detalhado, cada assunto abordado durante todo o semestre da matéria: Coding1.

Linguagem utilizada: 
![JavaScript](https://img.shields.io/badge/JavaScript-black?style=for-the-badge&logo=javascript&logoColor=yellow)


## Coding (Algoritmos)
Neste dia foi apresentado pela professora @Tereza Oliveira: como podemos operar variáveis em um programa .js, explicando detalhadamente sobre os tipos aplicáveis de variáveis (var, let, const), além disso foi mostrado a concatenação de palavras "soma de palavras" e a utilização dos operadores matemáticos: Soma, subtração, multiplicação e divisão.


## Coding (Tipos primitivos)
Na aula sobre **Tipos Primitivos**, foram explorados os conceitos fundamentais relacionados aos dados básicos e imutáveis na linguagem **JavaScript**, essenciais para o desenvolvimento de aplicações dinâmicas.

### Principais Tipos Primitivos

1. **String**  
   Representa textos, delimitados por aspas simples (`'`), duplas (`"`) ou crases (`` ` ``) para templates literais.  
   - Exemplo: `"JavaScript"`, `'Tipos Primitivos'`, `` `Texto interpolado ${variavel}` ``.

2. **Number**  
   Utilizado para números inteiros ou decimais, incluindo valores especiais como `Infinity`, `-Infinity` e `NaN` (Not a Number).  
   - Exemplo: `42`, `3.14`, `NaN`.

3. **Boolean**  
   Representa valores lógicos, sendo `true` ou `false`.  
   - Exemplo: `let isActive = true;`.

4. **Undefined**  
   Indica que uma variável foi declarada, mas não recebeu valor.  
   - Exemplo: `let valor;` (o valor de `valor` será `undefined`).

5. **Null**  
   Representa a ausência proposital de um valor.  
   - Exemplo: `let resultado = null;`.

6. **BigInt**  
   Representa números inteiros maiores do que o permitido pelo tipo `Number`.  
   - Exemplo: `const bigNumber = 123456789012345678901234567890n;`.

7. **Symbol**  
   Usado para criar identificadores únicos, principalmente em cenários que demandam propriedades exclusivas em objetos.  
   - Exemplo: `const id = Symbol('identificador');`.

### Características Gerais

- **Imutabilidade**: O valor de um tipo primitivo não pode ser alterado após sua criação.
- **Armazenamento por valor**: Diferentemente de objetos e arrays, os tipos primitivos são armazenados diretamente na memória.

### Aplicações e Contextos

A compreensão dos tipos primitivos é fundamental para:
- Construção de operações seguras;
- Validação de dados;
- Manipulação eficaz de variáveis.

A aula também destacou:
- O uso de `typeof` para verificar o tipo de uma variável;
- A distinção entre `null` e `undefined`, dois conceitos que frequentemente geram confusão.


## Coding (Estruturas condicionais)

Na aula sobre **Estruturas Condicionais em JavaScript**, foram apresentadas as bases para a criação de fluxos de controle, permitindo que o código tome decisões dinâmicas com base em condições.

### Principais Estruturas Condicionais

1. **if/else**  
   Utilizada para verificar condições e executar blocos de código diferentes com base no resultado lógico.  
   - Exemplo:
     ```javascript
     if (condicao) {
         // Bloco executado se a condição for verdadeira
     } else {
         // Bloco executado se a condição for falsa
     }
     ```

2. **else if**  
   Permite verificar múltiplas condições em sequência.  
   - Exemplo:
     ```javascript
     if (condicao1) {
         // Bloco executado se condicao1 for verdadeira
     } else if (condicao2) {
         // Bloco executado se condicao2 for verdadeira
     } else {
         // Bloco executado se nenhuma condição for verdadeira
     }
     ```

3. **switch**  
   Usada para simplificar verificações de múltiplos casos relacionados a um mesmo valor.  
   - Exemplo:
     ```javascript
     switch (expressao) {
         case valor1:
             // Bloco executado se expressao === valor1
             break;
         case valor2:
             // Bloco executado se expressao === valor2
             break;
         default:
             // Bloco executado se nenhum caso for satisfeito
     }
     ```

### Operadores Condicionais

1. **Operador Ternário (`? :`)**  
   Simplifica a verificação de condições em uma única linha.  
   - Exemplo:
     ```javascript
     const resultado = condicao ? 'Valor se verdadeiro' : 'Valor se falso';
     ```

2. **Operadores Lógicos (`&&`, `||`, `!`)**  
   São usados para combinar ou inverter condições:
   - `&&` (E): Ambos os lados precisam ser verdadeiros.
   - `||` (OU): Pelo menos um lado precisa ser verdadeiro.
   - `!` (NÃO): Inverte o valor lógico.

### Boas Práticas

- Sempre priorizar a legibilidade do código, evitando estruturas condicionais muito complexas.
- Utilizar `switch` para comparações com múltiplos valores fixos.
- Empregar o operador ternário apenas em condições simples.

### Aplicações e Contextos

Estruturas condicionais são amplamente utilizadas para:
- Controle de fluxo em sistemas interativos;
- Validações de entrada de dados;
- Respostas dinâmicas baseadas em condições variáveis.


## Coding (Arrays)
# Resumo: Aula sobre Arrays em JavaScript

Na aula sobre **Arrays em JavaScript**, foram exploradas as estruturas que permitem armazenar, manipular e iterar coleções de dados. Arrays são fundamentais no desenvolvimento de aplicações modernas devido à sua flexibilidade e poder.

## O que é um Array?

Um **Array** é uma estrutura de dados usada para armazenar uma coleção ordenada de elementos, que podem ser de diferentes tipos (números, strings, objetos, etc.). Cada elemento é acessado por meio de um índice, que começa em `0`.

- Exemplo de criação:
  ```javascript
  const numeros = [1, 2, 3, 4, 5];
  const misto = ['texto', 42, true, null];
  
Principais Operações com Arrays
Acessar Elementos
Utiliza o índice para acessar valores.

Exemplo:
javascript
Copiar código
const frutas = ['maçã', 'banana', 'laranja'];
console.log(frutas[0]); // 'maçã'
Adicionar Elementos

Push: Adiciona ao final do array.
javascript
Copiar código
frutas.push('uva'); // ['maçã', 'banana', 'laranja', 'uva']
Unshift: Adiciona ao início.
javascript
Copiar código
frutas.unshift('melancia'); // ['melancia', 'maçã', 'banana', 'laranja']
Remover Elementos

Pop: Remove o último elemento.
javascript
Copiar código
frutas.pop(); // ['maçã', 'banana', 'laranja']
Shift: Remove o primeiro elemento.
javascript
Copiar código
frutas.shift(); // ['banana', 'laranja']
Iterar sobre o Array

For:
javascript
Copiar código
for (let i = 0; i < frutas.length; i++) {
    console.log(frutas[i]);
}
ForEach:
javascript
Copiar código
frutas.forEach(fruta => console.log(fruta));
Métodos Importantes

Map: Cria um novo array transformando os elementos.
javascript
Copiar código
const numeros = [1, 2, 3];
const dobrados = numeros.map(num => num * 2); // [2, 4, 6]
Filter: Filtra elementos com base em uma condição.
javascript
Copiar código
const maiores = numeros.filter(num => num > 2); // [3]
Reduce: Reduz o array a um único valor.
javascript
Copiar código
const soma = numeros.reduce((acc, num) => acc + num, 0); // 6
Características Gerais
Arrays são mutáveis, ou seja, seus elementos podem ser alterados diretamente.
Podem armazenar valores heterogêneos, embora seja uma boa prática manter a consistência no tipo dos dados.
Suportam operações complexas com métodos nativos eficientes.
Boas Práticas
Usar métodos nativos como map, filter e reduce para evitar loops manuais sempre que possível.
Declarar arrays constantes (const) quando não houver necessidade de reatribuição.
Escolher nomes significativos para descrever o propósito do array.
Aplicações e Contextos
Arrays são usados em diversas situações, como:

Armazenar listas de itens (produtos, usuários, dados de sensores, etc.);
Manipular dados dinâmicos em aplicações interativas;
Implementar estruturas mais complexas, como filas e pilhas.

## Coding (Funções)
# Resumo: Aula sobre Funções em JavaScript

Na aula sobre **Funções em JavaScript**, foi discutido como encapsular blocos de código reutilizáveis, tornando o desenvolvimento mais modular, eficiente e organizado.

## O que é uma Função?

Uma **função** é um bloco de código projetado para executar uma tarefa específica. Ela pode receber entradas (parâmetros), realizar operações e, opcionalmente, retornar um resultado.

- Exemplo básico de uma função:
  ```javascript
  function saudacao(nome) {
      return `Olá, ${nome}!`;
  }
  console.log(saudacao('João')); // 'Olá, João!'

  Tipos de Funções
Declaração de Função
Definida com a palavra-chave function e um nome.

Exemplo:
javascript
Copiar código
function somar(a, b) {
    return a + b;
}
console.log(somar(2, 3)); // 5
Função Anônima
Função sem nome, geralmente atribuída a uma variável.

Exemplo:
javascript
Copiar código
const subtrair = function(a, b) {
    return a - b;
};
console.log(subtrair(5, 3)); // 2
Função de Flecha (Arrow Function)
Introduzida no ES6, é mais concisa e não possui seu próprio this.

Exemplo:
javascript
Copiar código
const multiplicar = (a, b) => a * b;
console.log(multiplicar(3, 4)); // 12
Função IIFE (Immediately Invoked Function Expression)
Executada imediatamente após ser definida.

Exemplo:
javascript
Copiar código
(function() {
    console.log('Executado imediatamente!');
})();
Parâmetros e Argumentos
Parâmetros são definidos na declaração da função.
Argumentos são os valores passados para a função na sua invocação.
Exemplo:
javascript
Copiar código
function dividir(a, b = 1) { // b possui valor padrão 1
    return a / b;
}
console.log(dividir(10, 2)); // 5
console.log(dividir(10)); // 10
Escopo e Hoisting
Escopo
Define onde uma variável ou função está acessível:

Escopo local: Dentro de uma função.
Escopo global: Fora de qualquer função.
Hoisting
Funções declaradas são "movidas" para o topo do código durante a execução, permitindo sua chamada antes da definição.

Exemplo:
javascript
Copiar código
saudacao('Maria'); // Funciona, devido ao hoisting.
function saudacao(nome) {
    console.log(`Olá, ${nome}!`);
}
Boas Práticas
Definir nomes claros e descritivos para as funções.
Manter funções pequenas e específicas.
Utilizar const ou let para armazenar funções anônimas.
Evitar funções muito complexas, optando por modularização.
Aplicações e Contextos
Funções são amplamente utilizadas para:

Modularizar o código e evitar duplicação.
Implementar lógica reutilizável em diferentes partes do sistema.
Facilitar testes e manutenção do código.


## Coding (Objetos)
# Resumo: Aula sobre Objetos em JavaScript

Na aula sobre **Objetos em JavaScript**, foi explorada uma das estruturas de dados mais importantes da linguagem, usada para armazenar e organizar dados de forma chave-valor.

## O que é um Objeto?

Um **objeto** é uma coleção de propriedades, onde cada propriedade é composta por um par **chave** e **valor**. Objetos são úteis para representar entidades e suas características.

- Exemplo básico:
  ```javascript
  const pessoa = {
      nome: 'João',
      idade: 30,
      profissao: 'Desenvolvedor'
  };

Principais Operações com Objetos
Acessar Propriedades

Notação de ponto:
javascript
Copiar código
console.log(pessoa.nome); // 'João'
Notação de colchetes:
javascript
Copiar código
console.log(pessoa['idade']); // 30
Adicionar ou Atualizar Propriedades

Exemplo:
javascript
Copiar código
pessoa.altura = 1.75; // Adiciona uma nova propriedade
pessoa.idade = 31; // Atualiza a propriedade existente
Remover Propriedades

Exemplo:
javascript
Copiar código
delete pessoa.profissao;
console.log(pessoa.profissao); // undefined
Iterar sobre Propriedades

Usando for...in:
javascript
Copiar código
for (let chave in pessoa) {
    console.log(`${chave}: ${pessoa[chave]}`);
}
Verificar Propriedades

Usando in:
javascript
Copiar código
console.log('nome' in pessoa); // true
Usando hasOwnProperty:
javascript
Copiar código
console.log(pessoa.hasOwnProperty('idade')); // true
Métodos em Objetos
Um método é uma função definida como uma propriedade de um objeto.

Exemplo:
javascript
Copiar código
const carro = {
    marca: 'Toyota',
    modelo: 'Corolla',
    acelerar: function() {
        console.log('O carro está acelerando!');
    }
};
carro.acelerar(); // 'O carro está acelerando!'
Objetos e Referências
Objetos são armazenados por referência, não por valor. Isso significa que alterações feitas em uma variável que aponta para um objeto afetam o objeto original.

Exemplo:
javascript
Copiar código
const obj1 = { a: 1 };
const obj2 = obj1;
obj2.a = 2;
console.log(obj1.a); // 2
Métodos Úteis para Manipulação de Objetos
Object.keys: Retorna as chaves do objeto.
javascript
Copiar código
console.log(Object.keys(pessoa)); // ['nome', 'idade']
Object.values: Retorna os valores do objeto.
javascript
Copiar código
console.log(Object.values(pessoa)); // ['João', 31]
Object.entries: Retorna um array de pares [chave, valor].
javascript
Copiar código
console.log(Object.entries(pessoa)); // [['nome', 'João'], ['idade', 31]]
Boas Práticas
Usar nomes claros e consistentes para as chaves.
Evitar aninhar objetos excessivamente, para manter a estrutura legível.
Criar métodos dentro de objetos para encapsular lógica relacionada.
Aplicações e Contextos
Objetos são amplamente usados para:

Representar entidades como usuários, produtos ou configurações.
Agrupar dados relacionados em uma estrutura lógica.
Servir como base para APIs e manipulação de dados.


*Vítor Vieira de Souza, ADS040-1T*

### 12-10-2024 ###
