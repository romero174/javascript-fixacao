Exercício de Fixação JavaScript

Nome: Romero

Data: 29/09/2025

*   **1\. Variáveis e Tipos**
*   **2\. Operadores e Expressões**
*   **3\. Estruturas de Controle**
*   **4\. Loops e Repetições**
*   **5\. Funções**
*   **6\. Mini-casos práticos**
*   **7\. Reflexão**  
    

### 1.1 Variáveis e Tipos

*   Qual a diferença entre var, let e const?
Var É uma declaração antiga de variável, que não é mais recomendada atualmente.

Let: É uma variável mutável, pode mudar de valor durante o código.

Const: É uma variável constante, que não pode mudar depois de criada, indicada para conteúdos imutáveis como nome ou CPF.

  

*   Liste os tipos primitivos do JavaScript com exemplos.  
    **number**: Representa valores numéricos, tanto inteiros quanto decimais.

let idade = 30;

*   **string**: Uma sequência de caracteres, utilizada para texto.

let nome = "Maria";

*   **boolean**: Um valor lógico que pode ser true (verdadeiro) ou false (falso).

let v= true;

*   **array**: Uma coleção de elementos, que podem ser de tipos diferentes, armazenados em uma única variável.

let numeros = \[1, 2, 3, 4\];

numeros\[0\] retorna 1.

*   **object**: Representa um objeto, com propriedades (pares chave-valor) e métodos.

let pessoa = { nome: "Ana", idade: 25 };

  

*   Qual a diferença entre null e undefined?  
    **null**: Representa a ausência intencional de um valor.

**undefined**: Indica que uma variável foi declarada, mas ainda não recebeu um valor.

  

*   Explique == e ===

\== é o operador de igualdade "ampla" (ou "aproximada") que verifica se dois valores são iguais após tentar converter seus tipos, enquanto === é o operador de igualdade "estrita" (ou "mesmo valor e tipo") que verifica se ambos os valores e seus tipos são idênticos, sem realizar conversão de tipo.

### 1.2 Operadores e Expressões

*   Liste operadores matemáticos: +, -, \*, /.  
    \+ Adição

\-Subtração

\* Multiplicação

/ Divisão

*   Liste operadores lógicos: &&, ||, !

  
&& (and): retorna true apenas se ambas as condições gerarem resultados verdadeiros; || (or): retorna true quando pelo menos uma das condições gera um resultado verdadeiro; !: significa a negação lógica no Javascript, ele inverte os valores do tipo boolean, entregando, portanto, true para casos falsos e false para condições verdadeiras

### 1.3 Estruturas de Controle

*   Explique if, else if e else.

**if**: É a primeira condição a ser testada. Se a condição dentro dos parênteses for verdadeira, o código dentro das chaves {} do if é executado. Se for falsa, o programa passa para o próximo else if ou else.

**else if**: É usado para verificar uma nova condição se a condição do if (ou do else if anterior) for falsa. É possível ter vários else if para testar múltiplas condições em sequência.

**else**: É o último bloco. Ele é executado apenas se **nenhuma** das condições anteriores (if ou else if) for verdadeira.

*   Como usar switch?

É uma estrutura condicional usada para executar diferentes blocos de código com base em diferentes valores de uma expressão.  

*   Escreva um exemplo de verificação de maioridade.

const idade = 20; // Valor de exemplo

if (idade >= 18) { console.log("Você é maior de idade.");

else { console.log("Você é menor de idade.");  

### 2.4 Loops e Repetições

*   Liste os tipos de loops: for, while, do...while.

**for**: Utilizado quando se sabe o número exato de vezes que o bloco de código deve ser executado. Sua sintaxe inclui uma inicialização, uma condição de parada e um incremento, tudo em uma única linha.

**while**: Executa um bloco de código repetidamente enquanto uma condição especificada for verdadeira. A condição é verificada antes de cada iteração.

**do...while**: Semelhante ao while, mas garante que o bloco de código seja executado pelo menos uma vez, já que a condição é verificada somente após a primeira execução.  

*   Escreva mentalmente como imprimir números de 1 a 5.

for (let i = 1; i <= 5; i++) {

console.log(i);

}

*   Explique break e quando usá-lo.

é usado para interromper um loop presente em um código. É importante para evitar execuções desnecessárias e poupar processamento ou para parar uma ação quando a condição imposta for satisfeita ao usar for, while, do…while ou mesmo a opção switch.

### 2.5 Funções

*   O que é uma função?

Uma função é um bloco de código reutilizável que executa uma tarefa específica. Ela pode receber dados de entrada, chamados de parâmetros, processá-los e, opcionalmente, retornar um valor. O uso de funções ajuda a organizar o código, torná-lo mais legível e evitar a repetição de instruções.  

*   Diferença entre função declarada e função expressa.

A **declaração de função** é nomeada e pode ser chamada antes de ser definida, enquanto a **expressão de função** é atribuída a uma variável e só pode ser usada após a sua atribuição. A expressão de função permite criar funções anônimas e tem mais flexibilidade, podendo ser passada como argumento para outras funções.

*   Crie uma função que recebe um nome e retorna saudação.

function saudacao(nome) {  
return \`Olá, ${nome}!\`;  
}  
  
_// Exemplo de uso_  
const saudacao1 = saudacao("Alice");  
console.log(saudacao1); _// Saída: Olá, Alice!_  
  
const saudacao2 = saudacao("Bob");  
console.log(saudacao2); _// Saída: Olá, Bob!_

### 2.6 Mini-casos práticos

Verificação de número par ou ímpar.  
function verificarParImpar(numero) {

if (numero % 2 === 0) {

console.log(\`${numero} é par\`);

} else {

console.log(\`${numero} é ímpar\`);

}

}

verificarParImpar(10); // Saída: 10 é par

verificarParImpar(7); // Saída: 7 é ímpar  

*   Criação mental de uma lista de compras (array)

const listaDeCompras = \["pão", "leite", "ovos", "maçãs"\];

console.log(listaDeCompras);  

*   Somar números de 1 a 10 usando loop.

let soma = 0;

for (let i = 1; i <= 10; i++) {

soma += i;

}

console.log("A soma dos números de 1 a 10 é: " + soma); // Saída: A soma dos números de 1 a 10 é: 55  

### 2.7 Reflexão

*   Por que conhecer tipos e operadores ajuda a programar melhor?  
    Tipos e operadores são fundamentais na programação porque trazem estrutura, controle e eficiência ao código. Eles permitem que o programador manipule dados de forma previsível e segura, como os operadores que permitem manipular e comparar valores, executar cálculos matemáticos e tomar decisões lógicas, e os tipos para guardar aários tipos de dados e usá-los no código.  
    
*   Por que usar console.log() é importante para debug?  
    é essencial para o debug por sua capacidade de fornecer visibilidade instantânea do que está acontecendo "por debaixo dos panos" no código. Ele permite inspecionar valores de variáveis, rastrear o fluxo de execução e identificar erros de forma simples e direta.  
    
*   Como planejar variáveis, funções e loops antes de programar?  
    Para planejar variáveis, funções e loops antes de programar, o segredo é focar na lógica do problema e não nos detalhes da sintaxe de uma linguagem específica. Usando ferramentas como algoritmos, pseudocódigo e fluxogramas, você pode organizar suas ideias e simplificar a codificação.
