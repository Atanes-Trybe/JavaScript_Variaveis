# Repositório: JavaScript_Variaveis
O que são variáveis em JavaScript e como declarar e trabalhar com elas de uma forma simples e direta!

## Em primeiro lugar, o que é uma variável?
Podemos dizer que uma variável é um container para armazenar um valor, como por exemplo um nome para apresentar na tela ou um número que podemos usar em uma operação matemática, ou ainda uma sequência de texto que podemos usar para montar um documento, e-mail, etc. 

Mas uma coisa importante sobre as variáveis é que seu conteúdo pode mudar ao longo da execução do seu código. Um exemplo simples seria:

``` javascript
let nome = 'Alexandre';
console.log(nome);

nome = 'Márcia';
console.log(nome);
```
Nesse exemplo criamos uma variável `nome`, que recebe um valor do tipo string e usamos o `console.log()` para imprimir o valor da variável `nome` no console do nosso terminal e ou no console do browser.

Na declação da variável, quando ela é criada efetivamente, colocamos o valor **Alexandre** e depois mudamos o valor da variável para **Márcia** o que é totalmente possivel e comum em programação quando falamos de variáveis! 😜

## Criando variáveis no JavaScript
Por ser uma linguagem de [tipagem dinâmica](https://pt.wikipedia.org/wiki/Sistema_de_tipos#:~:text=Tipagem%20din%C3%A2mica%20%C3%A9%20uma%20caracter%C3%ADstica,ou%20a%20execu%C3%A7%C3%A3o%20do%20programa.), no JavaScript não há necessidade de declarar o tipo da variável, pois a linguagem define o tipo da variavel de acordo com o tipo de dado que é passado para ela no momento da atribuição de um valor;

Por exemplo, na declaração da variável idade, como podemos ver abaixo:
``` javascript
let idade = 51;
```
Podemos perceber que não há uma declaração efetiva de tipo para a variável. 🧐

## Declarando variáveis
Nós podemos declarar uma variável no JavaScript de três formas diferentes:

Com a palavra chave `var`. Por exemplo, `var nome = 'Michelle'`. Esta sintaxe pode ser usada para declarar tanto variáveis locais como variáveis globais.
Obs.: De acordo com o [ECMA2015](https://262.ecma-international.org/6.0/), utilizar o operador `var` se tornou uma má pratica de programação.  
Por simples adição de valor. Por exemplo, `nome = 'Michel'`. Isso declara uma variável global. Essa declaração vai gerar um aviso de advertência no JavaScript. Você não deve usar essa variante.  
Com a palavra chave `let`. Por exemplo, `let soma = 13`. Essa sintaxe pode ser utilizada para criar uma variável local com escopo de bloco. Vamos falar sobre escopo de variáveis mais a frente! 👍🏻. 

## Tipos de variáveis em JavaScript
Os [tipos de variáveis](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Data_structures) em JS são classificados em:

[Strings](https://developer.mozilla.org/pt-BR/docs/Glossary/String) — Uma String nada mais é que texto puro.  
[Numbers](https://developer.mozilla.org/pt-BR/docs/Glossary/Number) — São os números, sejam eles inteiros e ou decimais.  
[Booleans](https://developer.mozilla.org/pt-BR/docs/Glossary/Boolean) — São os operadores booleanos (true ou false).  
[Arrays](https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Reference/Global_Objects/Array) — É uma estrutura de dados para armazenar uma coleção de valores que podem ser qualquer tipo.  
[Objects](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object) — Um objeto é uma coleção de propriedades, e uma propriedade é uma associação entre uma propriedade (ou chave) e um valor.  
[Functions](https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Guide/Functions) — Em JavaScript é possível declarar uma variável como uma função, podendo fazer operações e retornando o valor para a variável de declaração. Obs: muito utilizado no paradigma de programação funcional.  
[null](https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Reference/Global_Objects/null). Uma palavra-chave que indica valor nulo. Devido JavaScript ser case-sensitive, null não é o mesmo que Null, NULL, ou ainda outra variação.  
[undefined](https://www.w3schools.com/jsref/jsref_undefined.asp). A propriedade undefined indica que uma variável não recebeu um valor ou não foi declarada.  

### Exemplos de declaração de varivéis
```javascript
// Valores number
  let numero = 13;
  let moeda = 45.50;
// Valor string
  let classe = 'especial';
// Um array
  let animais = ['gatos', 'cachorros', 'peixes', 'aves'];
// Um objeto
  let pessoa = {
    nome: 'Alexandre',
    idade: 51,
    profissao: 'professor'
  };
// Valor boleano
  let maiorIdade = true;
// Valor nulo;
  let concluido = null;
// Se um valor não for atribuido a variável recebe um valor undefined
  let data;
```

Obs.: Para atualizar uma variável depois de um valor inicial atribuido, você pode atualizar esse valor simplesmente atribuindo um valor diferente a variável.
```javascript
  let profissao = 'professor';

  profissao = 'pesquisador';
```

## Regras de nomeação de variáveis
Não existe uma limitação em relação ao nome que podemos colocar em uma variável, mas devemos seguir algumas regras importantes na declação desses nomes.
Preferencialmente devemos nos limitar a utilizar somente os caracteres latinos (0-9, a-z, A-Z) e o caractere underline ( _ ).

Obs.: A utilização de outros caracteres pode causar erros e dificultar o seu entendimento por outros profissionais da área, o que dificulta a manutenção dos sistemas, por exemplo.  
Não devemos usar **underline ( _ )** no início do nome de variáveis — isso é utilizado em certos construtores JavaScript para significar coisas específicas, então pode deixar as coisas confusas.  
Não podemos usar números no início do nome de variáveis, isso causa um erro no código.  
Existem algumas convenções, conhecidas mundialmente, para nomear as variáveis, podemos ver as mais conhecidas e utilizadas na imagem abaixo:  

![Project Gif](./images/nomenclaturas.jpg). 

**Dicas:**. 
Faça nomes de variáveis intuitivos que descrevam exatamente o dado/informação que ela contém. Não use letras ou números únicos, ou nomes longos demais.
As variáveis são [CASE SENSITIVE](https://pt.wikipedia.org/wiki/Case-sensitive) e diferenciam letras maiúsculas e minúsculas — então `nome` é uma variável diferente de `Nome`.  
Por último, mas não menos importante, não podemos utilizar as palavras reservadas pelo JavaScript como nome das nossas variáveis, ou seja, palavras que fazem parte da sintaxe do JavaScript como `const`, `undefined`, `function`, `let` e `while` não podem ser utilizados como nome de variáveis. ‼️
